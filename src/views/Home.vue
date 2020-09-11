<template>
  <div class="home">
    <!-- Landing page -->
    <div class="landing">
      <div class="container">
        <div class="row landing-page">
          <div class="col">
            <p class="welcome-text">Hi!</p>
            <p class="welcome-text">I'm <span id="name">Rishav</span></p>
            <p class="tag-line">Data Science, Analytics & Web Development</p>
            <a href="https://www.linkedin.com/in/rishavsaha240" target="_blank">
              <img
                src="../assets/linkedin_icon.png"
                alt="linked_in"
                id="social-icon"
              />
            </a>
            <a href="#" target="_blank">
              <img
                src="../assets/github_icon.png"
                alt="github"
                id="social-icon"
              />
            </a>
            <br />
            <a
              href="https://github.com/rishav-saha240"
              target="_blank"
              class="btn btn-dark mt-3"
            >
              <svg
                width="1em"
                height="1em"
                viewBox="0 0 16 16"
                class="bi bi-file-earmark-arrow-down-fill"
                fill="currentColor"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M2 2a2 2 0 0 1 2-2h5.293A1 1 0 0 1 10 .293L13.707 4a1 1 0 0 1 .293.707V14a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V2zm7 2l.5-2.5 3 3L10 5a1 1 0 0 1-1-1zm-.5 3.5a.5.5 0 0 0-1 0v3.793l-1.146-1.147a.5.5 0 0 0-.708.708l2 2a.5.5 0 0 0 .708 0l2-2a.5.5 0 0 0-.708-.708L8.5 11.293V7.5z"
                />
              </svg>
              Resume
            </a>
          </div>
          <div class="col">
            <img
              src="../assets/my-image.jpeg"
              alt="my image"
              class="my-image"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Profile page -->

    <div class="profile">
      <div class="container">
        <p id="section-tag">Profile</p>
        <div class="underline-profile"></div>
        <div class="row">
          <div
            class="col-lg-4 col-md-10 col-sm-12 offset-md-1 offset-lg-0 mt-3"
          >
            <p class="profile-section">About me</p>
            <p class="profile-section-text">
              I love to play with data<br />Bringing out insights from data is
              my passion.
            </p>
          </div>
          <div
            class="col-lg-4 col-md-10 col-sm-12 offset-md-1 offset-lg-0 mt-3"
          >
            <p class="profile-section">Education</p>
            <div v-for="data in education_details" :key="data.order">
              <p class="profile-section-text" style="line-height: 1.3">
                <strong>Institute:</strong> {{ data.instituteName }}
              </p>
              <p class="profile-section-text" style="line-height: 1.3">
                <strong>Qualification:</strong> {{ data.qualification }}
              </p>
              <p class="profile-section-text" style="line-height: 1.3">
                <strong>Duration:</strong> {{ data.durationStart }} -
                {{ data.durationEnd }}
              </p>
              <br />
            </div>
          </div>
          <div
            class="col-lg-4 col-md-10 col-sm-12 offset-md-1 offset-lg-0 mt-3"
          >
            <p class="profile-section">Details</p>
            <p class="profile-section-text">
              <strong>Name:</strong> Rishav Saha
            </p>
            <p class="profile-section-text"><strong>Age:</strong> 21</p>
            <p class="profile-section-text">
              <strong>Location:</strong> West Bengal, India
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- Skills page -->
    <div class="skills">
      <div class="container">
        <p id="section-tag">Skills</p>
        <div class="underline-skills"></div>

        <!-- sample skills -->
        <div class="row">
          <div
            class="col-lg-4 col-md-4 col-sm-12 offset-md-0 offset-lg-0 text-center"
          >
            <p class="sample-skills">Data Science and Analytics</p>
          </div>
          <div
            class="col-lg-4 col-md-4 col-sm-12 offset-md-0 offset-lg-0 text-center"
          >
            <p class="sample-skills">Data Visualization</p>
          </div>
          <div
            class="col-lg-4 col-md-4 col-sm-12 offset-md-0 offset-lg-0 text-center"
          >
            <p class="sample-skills">Database Management</p>
          </div>
        </div>
        <div class="row mt-4">
          <div
            class="col-lg-4 col-md-4 col-sm-12 offset-md-0 offset-lg-0 text-center"
          >
            <p class="sample-skills">Programming</p>
          </div>
          <div
            class="col-lg-4 col-md-4 col-sm-12 offset-md-0 offset-lg-0 text-center"
          >
            <p class="sample-skills">Web Development</p>
          </div>
          <div
            class="col-lg-4 col-md-4 col-sm-12 offset-md-0 offset-lg-0 text-center"
          >
            <p class="sample-skills">Web Designing</p>
          </div>
        </div>

        <!-- Button for skills page -->
        <div class="text-center mt-5">
          <router-link to="/skills" class="skills-btn"
            >Click to see all skills</router-link
          >
        </div>
      </div>
    </div>

    <!-- Project -->
    <div class="project">
      <div class="container">
        <p id="section-tag" style="color: black;">Projects</p>
        <div class="underline-project"></div>
        <div class="text-center">
          <p style="font-size: 1.2rem; padding-bottom: 1rem;">
            Recent projects
          </p>
        </div>
        <!-- recent projects cards -->
        <div class="row p-2">
          <div class="col-md-4">
            <div class="card project-container">
              <div class="card-body">
                <h4 class="card-title">title</h4>
                <p class="card-text">
                  Brief of the project<br />How to setup VScode for competitive
                  programming
                </p>
                <router-link to="#">Detail</router-link>
              </div>
            </div>
          </div>
        </div>
        <!-- all project button -->
        <div class="text-center mt-5">
          <router-link to="/projects" class="project-btn"
            >Click to see all projects</router-link
          >
        </div>
      </div>
    </div>
    <!-- Contact me -->
    <div class="contact">
      <div class="container">
        <p id="section-tag">Contact me</p>
        <div class="underline-contact"></div>
        <form method="post">
          <div class="text-center" style="padding-bottom: 2rem;">
            <input
              type="text"
              v-model="name"
              placeholder="Name"
              class="form-style"
              required
            />
          </div>
          <div class="text-center" style="padding-bottom: 2rem;">
            <input
              type="email"
              v-model="email"
              placeholder="Email"
              class="form-style"
              required
            />
          </div>
          <div class="text-center" style="padding-bottom: 2rem;">
            <input
              type="text"
              v-model="subject"
              placeholder="Subject"
              class="form-style"
              required
            />
          </div>
          <div class="text-center" style="padding-bottom: 2rem;">
            <textarea
              rows="5"
              v-model="message"
              placeholder="Message"
              class="form-style"
              required
            />
          </div>
          <div class="text-center" style="padding-bottom: 2rem;">
            <button class="project-btn">Submit</button>
          </div>
        </form>
      </div>
      <div class="text-center footer">
        Developed by Rishav Saha - 2020
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
  data() {
    return {
      api_url: "http://localhost:3000/education-details",
      education_details: [],
      name: "",
      email: "",
      subject: "",
      message: "",
    };
  },
  methods: {
    get_education_details() {
      fetch(this.api_url, {
        method: "GET",
        headers: {
          "content-type": "application/json",
        },
      })
        .then((resp) => {
          return resp.json();
        })
        .then((resp) => {
          this.education_details = resp.data;
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
  beforeMount() {
    this.get_education_details();
  },
};
</script>

<style lang="scss" scoped>
.welcome-text {
  font-size: 4rem;
  font-family: "Josefin Sans";
  font-weight: 400;
  letter-spacing: 0.4rem;
}
#name {
  font-weight: 700;
  font-size: 4.5rem;
}
.landing-page {
  padding-top: 10rem;
}
.tag-line {
  font-family: "Comfortaa";
  font-weight: 1000;
  letter-spacing: 0.2rem;
}
.my-image {
  float: right;
  height: 22rem;
  border-radius: 50%;
  // display: none;
}
#social-icon {
  height: 1.5rem;
  padding-right: 2rem;
}
// profile
.profile {
  background-color: #0b7261;
  margin-top: 7rem;
}
#section-tag {
  color: #fff;
  font-size: 2.8rem;
  font-family: "Josefin Sans";
  letter-spacing: 0.2rem;
  padding-top: 4rem;
  font-weight: 600;
}
.underline-profile {
  padding-bottom: 3rem;
}
.underline-profile::after {
  margin-top: -1rem;
  content: "";
  display: block;
  height: 0.4rem;
  background: #2e2459;
  width: 14rem;
}
.profile-section {
  color: white;
  font-family: "Roboto", sans-serif;
  font-size: 1.6rem;
  font-weight: 500;
  letter-spacing: 0.15rem;
}
.profile-section-text {
  color: white;
}

// skills
.skills {
  background-color: #2e2459;
  padding-bottom: 3rem;
}
.underline-skills {
  padding-bottom: 3rem;
}
.underline-skills::after {
  margin-top: -1rem;
  content: "";
  display: block;
  height: 0.4rem;
  background: #a72144;
  width: 14rem;
}
.sample-skills {
  color: white;
  border: 2px solid white;
  padding: 0.5rem;
  font-size: 1.2rem;
}
.skills-btn {
  color: white;
  font-weight: 600;
  border: 2px solid white;
  padding: 0.5rem;
  text-decoration: none;
}
.skills-btn:hover {
  color: black;
  background: white;
}

// project
.project {
  background-color: #fcfcfc;
  padding-bottom: 3rem;
}
.underline-project {
  padding-bottom: 3rem;
}
.underline-project::after {
  margin-top: -1rem;
  content: "";
  display: block;
  height: 0.4rem;
  background: #0b7261;
  width: 14rem;
}
.project-container {
  height: 12rem;
}
.project-btn {
  color: black;
  font-weight: 600;
  border: 2px solid black;
  padding: 0.5rem;
  text-decoration: none;
}
.project-btn:hover {
  color: white;
  background: black;
}
// contact
.contact {
  background: #2b3439;
}
.underline-contact {
  padding-bottom: 3rem;
}
.underline-contact::after {
  margin-top: -1rem;
  content: "";
  display: block;
  height: 0.4rem;
  background: #ffc732;
  width: 14rem;
}
.form-style {
  width: 30rem;
  padding: 0.5rem;
  border: none;
  border-radius: 5px;
}
.footer {
  color: white;
  padding-bottom: 1.5rem;
  padding-top: 1.5rem;
}
.footer::before {
  content: "";
  display: block;
  height: 0.1rem;
  width: auto;
  background: #ffc732;
}
// media query
@media screen and (max-width: 767px) {
  .my-image {
    height: 10.1rem;
  }
  .welcome-text {
    font-size: 2.5rem;
  }
  #name {
    font-size: 3rem;
  }
  .tag-line {
    font-size: 0.85rem;
  }
  .landing-page {
    padding-top: 6rem;
  }
}

@media screen and (max-width: 571px) {
  .form-style {
    width: 20rem;
  }
  .sample-skills {
    font-size: 1rem;
  }
  .card-body {
    font-size: 0.8rem;
  }
  .card-body h4 {
    font-size: 1.2rem;
  }
}

@media screen and (max-width: 410px) {
  .my-image {
    height: 9rem;
  }
  .welcome-text {
    font-size: 2.2rem;
  }
}

@media screen and (max-width: 393px) {
  .my-image {
    height: 8.8rem;
  }
}

@media screen and (max-width: 390px) {
  .my-image {
    height: 8.5rem;
  }
}

@media screen and (max-width: 385px) {
  .my-image {
    height: 8.3rem;
  }
  .welcome-text {
    font-size: 2rem;
  }
}

@media screen and (max-width: 382px) {
  .my-image {
    height: 7.3rem;
  }
}

@media screen and (max-width: 366px) {
  .my-image {
    display: none;
  }
  .welcome-text {
    font-size: 2.5rem;
  }
  .profile-section {
    font-size: 1.2rem;
  }
  .profile-section-text {
    font-size: 0.8rem;
  }
  #section-tag {
    font-size: 2.2rem;
    font-weight: 500;
  }
}
</style>
