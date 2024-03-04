<template>
  <form>
    <div class="form-control">
      <label for="user-name">Your Name</label>
      <input id="user-name" name="user-name" type="text" />
    </div>
    <div class="form-control">
      <label for="age">Your Age (Years)</label>
      <input id="age" name="age" type="number" />
    </div>
    <div class="form-control">
      <label for="referrer">How did you hear about us?</label>
      <select id="referrer" name="referrer">
        <option value="google">Google</option>
        <option value="wom">Word of mouth</option>
        <option value="newspaper">Newspaper</option>
      </select>
    </div>
    <div class="form-control">
      <h2>What are you interested in?</h2>
      <div>
        <input id="interest-news" name="interest" type="checkbox" />
        <label for="interest-news">News</label>
      </div>
      <div>
        <input id="interest-tutorials" name="interest" type="checkbox" />
        <label for="interest-tutorials">Tutorials</label>
      </div>
      <div>
        <input id="interest-nothing" name="interest" type="checkbox" />
        <label for="interest-nothing">Nothing</label>
      </div>
    </div>
    <div class="form-control">
      <h2>How do you learn?</h2>
      <div>
        <input id="how-video" name="how" type="radio" />
        <label for="how-video">Video Courses</label>
      </div>
      <div>
        <input id="how-blogs" name="how" type="radio" />
        <label for="how-blogs">Blogs</label>
      </div>
      <div>
        <input id="how-other" name="how" type="radio" />
        <label for="how-other">Other</label>
      </div>
    </div>
    <div>
      <button>Save Data</button>
    </div>
  </form>
</template>

<style scoped>
form {
  max-width: 40rem;
  margin: 2rem auto;
  padding: 2rem;
  border-radius: 12px;
  background-color: #ffffff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.26);
}

.form-control {
  margin: 0.5rem 0;
}

label {
  font-weight: bold;
}

h2 {
  margin: 0.5rem 0;
  font-size: 1rem;
}

input,
select {
  display: block;
  width: 100%;
  margin-top: 0.5rem;
  font: inherit;
}

select {
  width: auto;
}

input[type='checkbox'],
input[type='radio'] {
  display: inline-block;
  width: auto;
  margin-right: 1rem;
}

input[type='checkbox'] + label,
input[type='radio'] + label {
  font-weight: normal;
}

button {
  padding: 0.75rem 2rem;
  border: 1px solid #0076bb;
  border-radius: 30px;
  color: white;
  font: inherit;
  cursor: pointer;
  background-color: #0076bb;
}

button:hover,
button:active {
  border-color: #002350;
  background-color: #002350;
}
</style>
