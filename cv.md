## Aleksandr Tishchenko
### __Contacts:__
__E-mail:__ oleks.tish@gmail.com

__Telegram:__ [Aleksandr Tishchenko](https://t.me/oleks_tish)

__LinkedIn:__ [Aleksandr Tishchenko](https://www.linkedin.com/in/oleksandr-tishchenko-683716187/)

### About myself:
I am a self-motivated and ambitious web developer with a passion for building state-of-the-art websites and applications. With proficiency in various scripting languages and web tools, as well as solid computer skills, I am an ideal candidate for any highly skilled and goal-oriented IT team. I have strong organizational, communication, and responsibility skills, and I am eager to learn and deepen my knowledge. My ultimate goal is to secure a position in an international company by creating an impressive portfolio of projects and gaining valuable experience from professional mentors.

### Skills and Proficiency:
- HTML
- CSS (SASS)
- JavaScript 
- React
- Bootstrap
- Git, GitHub 
- VS Code
- Figma, Adobe Photoshop
- BEM
- Scrum, GTD
### Code example:
```
import { Formik, Form, Field, ErrorMessage } from 'formik';
import * as Yup from 'yup';
import s from './SumInput.module.scss';

const validationSchema = Yup.object().shape({
  amount: Yup.string()
    .required('*Введіть суму або виберіть із запропонованих сум вище')
    .test('positive', '*Введіть суму або виберіть із запропонованих сум вище', value => {
      return !isNaN(value) && parseFloat(value) > 0;
    }),
});

const SumInput = () => {
  const initialValues = {
    amount: ''
  };

  const handleSubmit = (values, { setSubmitting }) => {
    setTimeout(() => {
      alert(JSON.stringify(values, null, 2));
      setSubmitting(false);
    }, 400);
  };

  return (
    <div>
      <Formik initialValues={initialValues} validationSchema={validationSchema} onSubmit={handleSubmit}>
        {({ errors, touched }) => (
          <Form className={s.support__form}>
            <Field
              type='text'
              name='amount'
              placeholder='Запропонувати іншу сумму'
              className={`${s.support__form_input} ${errors.amount && touched.amount ? s.fieldError : ''}`}
            />
            <ErrorMessage name='amount' />
          </Form>
        )}
      </Formik>
    </div>
  );
};

export default SumInput;
```
### Experience:
I was part of the team that worked on the social project, we were developing a website for CO "CF "A-HELP UA".
### Education:
MS, Ukrainian State University of Chemical Technology – Dnipro
Equipment of chemical production and building material plants, 2015
### Courses:
__Learn Html on__ [Codecademy](https://www.codecademy.com/learn/learn-html)

__Learn CSS on__ [Codecademy](https://www.codecademy.com/learn/learn-css/)

__Learn JavaScript Basics on__ [Codecademy](https://www.codecademy.com/learn/introduction-to-javascript)

__HTML/CSS Marathon on__ [GoIt](https://goit.ua/dlya-novichkov/) 

__JAVASCRIPT 2020 Course on__ [YouTube](https://www.youtube.com/playlist?list=PLM6XATa8CAG7DDIBjNVd78Fv5Ueo930IV) 

__Front-end development on__ [Sigma Software University](https://university.sigma.software/)
### Languages:
English (B1)

Ukrainian (native)

Russian (fluent)
