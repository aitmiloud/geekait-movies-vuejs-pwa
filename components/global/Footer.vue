<template>
  <footer :class="$style.footer">
    <p>&copy; {{ new Date().getFullYear() }} Geekait. All rights reserved.</p>
    <p>Designed by <a target="_blank" href="#">A.Inajarin</a> and built by M.Aitmiloud, data provided by <a target="_blank" href="https://www.themoviedb.org/" rel="noopener">TMDb</a>.</p>

    <ul class="nolist">
      <li>
        <a
          href="https://www.linkedin.com/in/mohammed-aitmiloud/"
          target="_blank"
          aria-label="Link to LinkedIn account"
          rel="noopener">
          <!-- eslint-disable-next-line -->
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="#585858"><path d="M19 0H5a5 5 0 0 0-5 5v14a5 5 0 0 0 5 5h14a5 5 0 0 0 5-5V5a5 5 0 0 0-5-5zM8 19H5V8h3v11zM6.5 6.732c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zM20 19h-3v-5.604c0-3.368-4-3.113-4 0V19h-3V8h3v1.765c1.396-2.586 7-2.777 7 2.476V19z"/></svg>
        </a>
      </li>
      <li>
        <a
          href="mailto:mohammed.aitmiloud@gmail.com"
          aria-label="Link to Email"
          rel="noopener">
          <!-- eslint-disable-next-line -->
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="#585858"><path d="M0 3v18h24V3H0zm21.518 2L12 12.713 2.482 5h19.036zM2 19V7.183l10 8.104 10-8.104V19H2z"/></svg>
        </a>
      </li>
    </ul>
  </footer>
</template>

<style lang="scss" module>
@import '~/assets/css/utilities/_variables.scss';

.footer {
  padding: 2rem 1.5rem 6.5rem;
  color: $text-color-grey;

  @media (min-width: $breakpoint-small) {
    padding-right: 4rem;
    padding-left: 4rem;
  }

  @media (min-width: $breakpoint-large) {
    padding: 2rem 5rem;
  }

  p {
    margin: 0.3rem 0;
    font-size: 1.4rem;
  }

  a {
    color: $text-color-grey;
    text-decoration: underline;
  }

  ul {
    display: flex;
    margin: 2rem 0 0 -0.5rem;

    a {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 4.4rem;
      height: 4.4rem;

      svg {
        transition: all 0.3s ease-in-out;
      }

      &:hover,
      &:focus {
        svg {
          fill: #fff;
        }
      }
    }
  }
}
</style>
