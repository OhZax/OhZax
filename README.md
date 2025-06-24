[![Serknet](https://r2.fivemanage.com/f6UgsuPuvM777m0UMQiq6/image(27).png)](https://serknet.xyz/)

# Soy Zax

**Co-Proprietario y Desarrollador de Software en Serknet**

---

## ✨ Sobre mí

- 🌐 Todos mis proyectos están disponibles en [serknet.xyz](https://serknet.xyz) y [ticket-hub.app](https://ticket-hub.app/)
- 💬 Pregúntame sobre: `Lua`, `JavaScript`, `HTML`, `CSS`, `TypeScript`
- ⛹️‍♂️ Soy desarrollador front-end.
- 📫 Puedes contactarme en: **zax@serknet.xyz**

---

## 🚀 Lenguajes que utilizo:

<p align="left">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="React" width="42" height="42"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5" width="42" height="42"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="42" height="42"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="TypeScript" width="42" height="42"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3" width="42" height="42"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="42" height="42"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/lua/lua-original.svg" alt="Lua" width="42" height="42"/>
</p>

## 🌐 Conecta conmigo:

<p align="left">
  <a href="https://twitter.com/serknetpr" target="_blank">
    <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"/>
  </a>
  <a href="https://www.instagram.com/vxyxrill" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram"/>
  </a>
  <a href="https://www.youtube.com/@serknet" target="_blank">
    <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube"/>
  </a>
  <a href="https://discord.gg/serknet" target="_blank">
    <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord"/>
  </a>
</p>

---

## 📝 Uso

```jsx
import React from 'react'

import ReactDOM from 'react-dom'

import DropdownTreeSelect from 'react-dropdown-tree-select'
import 'react-dropdown-tree-select/dist/styles.css'

// Representando los servicios y la experiencia de Serknet
const data = {
  label: '¿Por qué elegir Serknet?',
  value: 'serknet',
  children: [
    {
      label: 'Líderes en programación',
      value: 'coding',
      children: [
        {
          label: 'Tecnología moderna (React, TS, Python, Lua)',
          value: 'techstack',
        },
        {
          label: 'Soluciones personalizadas a tu medida',
          value: 'customsolutions',
        },
      ],
    },
    {
      label: 'Seguridad de primer nivel',
      value: 'security',
      children: [
        {
          label: 'Protección contra DDoS e infraestructura segura',
          value: 'ddos',
        },
        {
          label: 'Confiado por plataformas líderes',
          value: 'trusted',
        },
      ],
    },
    {
      label: 'Construyamos algo grande juntos',
      value: 'contact',
      children: [
        {
          label: 'Contáctanos: zax@serknet.xyz',
          value: 'email',
        },
        {
          label: 'Visítanos: https://serknet.xyz',
          value: 'website',
        },
      ],
    },
  ],
}

const onChange = (currentNode, selectedNodes) => {
  console.log('onChange::', currentNode, selectedNodes)
}
const onAction = (node, action) => {
  console.log('onAction::', action, node)
}
const onNodeToggle = currentNode => {
  console.log('onNodeToggle::', currentNode)
}

ReactDOM.render(
  <DropdownTreeSelect
    data={data}
    onChange={onChange}
    onAction={onAction}
    onNodeToggle={onNodeToggle}
  />,
  document.getElementById('root') // Usa un elemento real del DOM, no document.body
)
