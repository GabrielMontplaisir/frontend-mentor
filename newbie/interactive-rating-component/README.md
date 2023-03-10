# Frontend Mentor - Interactive rating component solution

This is a solution to the [Interactive rating component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-rating-component-koxpeBUmI). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Links](#links)
- [Built with](#built-with)
- [What I learned](#what-i-learned)
- [Author](#author)

## Links

- Solution URL: [https://www.frontendmentor.io/solutions/semantic-interactive-rating-component-using-radio-buttons-oXKiQfNfPZ](https://www.frontendmentor.io/solutions/semantic-interactive-rating-component-using-radio-buttons-oXKiQfNfPZ)
- Live Site URL: [https://gabrielmontplaisir.com/frontend-mentor/newbie/interactive-rating-component](https://gabrielmontplaisir.com/frontend-mentor/newbie/interactive-rating-component)

## Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Vite](https://vitejs.dev/)
- [Google Fonts](https://fonts.google.com/)

## What I learned

This is my first challenge I tackled w/ a form. I really wanted to make this semantically accurate, so opted to use the use the `<input>` element w/ radio buttons and took advantage of `value`, `name`, `id`. Unlike previous challenges where buttons were purely aesthetic, this button actually served a purpose. I initially wrapped the inputs and buttons in a `<form>`, but noticed it refreshed my page, so removed it.

Finally, I added my `script` at the end of my page before the `</body>` because this isn't the type of page which requires heavy JS.

Next, I took advantage of `transition` in my CSS to animate the buttons a little bit. I also used `:checked` to highlight the selection. Because of the Javascript, I had to use `id`, which isn´t something I often have to do when building static websites. It was a nice change of pace.

Having considerable experience w/ JS, it wasn't too difficult for me to figure out how to go about going from one section to the next. I opted for an `Eventlistener` to wait for the `"click"` and attributed the radio button's value to my selection. For a little extra, I decided to add a prompt if no selection is made to indicate to the user that they didn't select a rating. I simply hid the `.hidden` class where necessary. Because `InnerHTML` should be avoided where possible, I opted to use `innerText` instead.

## Continued Development

**February 9, 2023**
Made the component more accessible by using semantic HTML (replaced the ratings container with a fieldset + legend), and replaced the `aria-labels` with actual labels. I believe that screen readers don't always take advantage of or are not always compatible with aria. Doing this also required me to change my CSS slightly around the label placement and input placement. Adjusted consequently and removed the `grid` / `place-content: center` hackery which was happening.

I opted to remove the prompt for the user to select a rating if they click submit first without a selection. Instead, I simply made the button `disabled`. Simpler solution altogether. That means I can also take advantage of the fact that radio buttons must be selected and cannot be de-selected. This also meant I had to adjust the JS script to read whether a rating was clicked first.

Made the component slightly more responsive to different screen sizes by adding `clamp()` to the header and paragraph, adjust paddings and margins at different sizes.

## Author

- Website - [https://gabrielmontplaisir.com](https://gabrielmontplaisir.com)
- Frontend Mentor - [@GabrielMontplaisir](https://www.frontendmentor.io/profile/GabrielMontplaisir)
- LinkedIn - [@GabrielMontplaisir](https://www.linkedin.com/in/gabriel-montplaisir/)
