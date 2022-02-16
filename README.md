### Hi there, I'm Kamran👋

I'm an Information Engineering Student who loves programming.
Skills: C, Java, Python (Tkinter), MySQL, SQLite

![Visitor Count](https://profile-counter.glitch.me/{Kamran-Dev}/count.svg)

![curl](https://profile-counter.glitch.me/{Kamran-Dev}/count.svg)


const express = require('express')
const app = express()

const PLACES = 7;

// no db - so global var to keep track of count
let counter = 0

function getCountImage(count) {
   ...
}

// get the image
app.get('/count.svg', (req, res) => {
  counter++;

  // This helps with GitHub's image cache 
  //   see more: https://rushter.com/counter.svg
  res.set({
  'content-type': 'image/svg+xml',
  'cache-control': 'max-age=0, no-cache, no-store, must-revalidate'
  })

  // Send the generated SVG as the result
  res.send(getCountImage(counter));
})

const listener = app.listen(process.env.PORT, () => {
  console.log('Your app is listening on port ' + listener.address().port)
})


### 📞 Contact


<!--
**Kamran-Dev/Kamran-Dev** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
