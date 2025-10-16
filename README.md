Absolutely — here’s a smoother, more **human and conversational** rewrite of your **Simple NASA API README**.

It keeps all the technical accuracy, but now it *reads* like you wrote it — natural, confident, and easy for recruiters or devs to follow.

---

# 🚀 Simple NASA API

> “Bringing the cosmos a click closer.”

This is a small but fun project I built to explore working with real-world APIs. It uses NASA’s **Astronomy Picture of the Day (APOD)** API to let users enter any date and instantly see NASA’s featured photo or video for that day — complete with the title and a short explanation.

The goal was to practice API integration, improve my JavaScript skills, and build something that sparks curiosity about space.

---

## 🌌 What It Does

When you open the app, you can enter any date (past or present), hit **“Get Picture,”** and NASA’s API will fetch that day’s astronomy image or video. The app then updates the page with the content, along with its name and description.

**Main features:**

* 🛰️ Pulls daily images or videos directly from NASA’s API
* 📅 Lets you search by specific date
* 🖼️ Handles both images and videos dynamically
* 💬 Displays NASA’s explanation for each post
* 📱 Works on desktop and mobile screens

---

## 🧰 Tech Stack

| Area            | Tools                                  |
| --------------- | -------------------------------------- |
| **Frontend**    | HTML, CSS, JavaScript (ES6)            |
| **API**         | [NASA APOD API](https://api.nasa.gov/) |
| **Other Tools** | Git, GitHub Pages, VS Code             |

---

## ⚙️ How It Works

The logic is straightforward — when you type in a date, the app makes a request to NASA’s API using `fetch()`. The API returns a JSON object, and the app checks whether it’s an image or a video before displaying it.

Here’s the basic idea:

```javascript
fetch(`https://api.nasa.gov/planetary/apod?date=${input}&api_key=${apiKey}`)
  .then(res => res.json())
  .then(data => {
    if (data.media_type === 'video') {
      vid.src = data.hdurl;
    } else {
      image.src = data.hdurl;
    }
    starName.innerText = data.title;
    result.innerText = data.explanation;
  })
  .catch(err => console.log(`error ${err}`));
```

This taught me how to handle asynchronous JavaScript better, structure my functions cleanly, and debug live API data like a pro.

---

## 🎨 Design

I kept the design minimal — black background, centered layout, large readable text — to match NASA’s aesthetic and keep the focus on the images.

It’s also **fully responsive**, so the layout adjusts beautifully on phones, tablets, and larger screens.

---

## 🧑🏽‍🚀 How to Use

1. **Clone this repo:**

   ```bash
   git clone https://github.com/abdirxhmxn/simple-nasa-api.git
   cd simple-nasa-api
   ```
2. **Open it:**

   ```bash
   open index.html
   ```

   *(or just drag it into your browser)*
3. Enter a date → hit **Get Picture** → enjoy the view 🌌

---

## 💡 What I’d Like to Add Next

* A “Random Day” button for surprise space discoveries
* A loading spinner while the image fetches
* Error messages for invalid or future dates
* Credit display for photographers and mission sources

---

## 👨🏽‍💻 About Me

I’m **Abdirahman Mohamed**, a **Full-Stack Software Engineer** and **Computer Science student** at the **University of Southern Maine (Class of 2025)**.
I love building projects that make learning and exploration more engaging — whether it’s in education, data, or space.

📫 **Connect with me:**
[LinkedIn](https://linkedin.com/in/abdirahmanamohamed) • [GitHub](https://github.com/abdirxhmxn) • [Email](mailto:work.amohamed@gmail.com)

---

> “The sky isn’t the limit — it’s just the API endpoint.” 🌠

---

Would you like me to make a **short, 3-line “pinned repo summary”** version for your GitHub profile grid (so it matches your Quranify and NASA projects stylistically)? It’ll make your project lineup look consistent and professional.
