<template>
  <div>
    <section class="avatar">
      <div>
        <img src="@/assets/images/profile.jpeg" alt="profile image" />
      </div>
    </section>
    <section class="heading">
      <h1>Vahid Zafari</h1>
      <h2>Full-stack Engineer and Designer</h2>
    </section>
    <hr />
    <section class="paragraph">
      <h1>Profile Summary</h1>
      <p>
        I am a full-stack engineer and designer, a tech enthusiast, and an
        open-source advocate. I am always open to collaborating on projects and
        innovative/disruptive ideas. Find out more about me and feel free to
        connect with me. I do my best to developed good planning and
        organisational skills and am confident working independently or as part
        of the team. I am flexible regarding working hours. I dropout the
        university to raise my knowledge and skills.
      </p>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.avatar {
  width: 100px;
  height: 100px;
  border: 2px solid gray;
  border-radius: 50%;

  & > div {
    border-radius: 50%;
    padding: 7.5px;

    & > img {
      border-radius: 50%;
    }
  }
}

.heading {
  text-transform: uppercase;
  font-family: FjallaOne, sans-serif;
  font-size: 1.6rem;

  & > h1 {
    margin: 7px 0;
    letter-spacing: 5px;
  }

  & > h2 {
    margin: 7px 0;
    font-size: 1.2rem;
    letter-spacing: 3px;
  }
}

.paragraph {
  padding: 10px 0;

  & > h1 {
    margin: 5px 0;
  }

  & > p {
    margin: 5px 0;
    text-align: justify;
  }
}
</style>
