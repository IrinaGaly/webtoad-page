<template>
  <section class="section-about o-wrapper">
    <div class="section-about__header">
      <h1 class="section-about__title">What we do</h1>
      <p class="section-about__description"> We help organisations and individuals to grow in the digital space and boost them to reach their goals.</p>
    </div>
    <Card v-for="(card, index) in cardsList" :key="index" :icon="card.icon" :title="card.title" :description="card.description" ></Card>
  </section>
</template>

<script>
import Card from './Card.vue'
import BusinessDrivenIcon from '@/assets/icons/businessDriven.svg';
import ProgressiveIcon from '@/assets/icons/progressive.svg';
import CmsIcon from '@/assets/icons/cms.svg';
import ConsultingIcon from '@/assets/icons/consulting.svg';
import ServiceSideIcon from '@/assets/icons/serviceSide.svg';
import SoftwareArchitectureIcon from '@/assets/icons/softwareArchitecture.svg';


export default {
  name: 'SectionAbout',
  components: {
    Card,
  },
  data() {
    return {
      cardsList: [
        {
          icon: BusinessDrivenIcon,
          title: 'Business driven websites',
          description: 'Our job is not only to <strong>write code</strong>. In the beginning of a project it is necessary to plan the whole implementation based on a business case. Database structure, <strong>front-ends</strong>, backend endpoints, data flows…'
        },
        {
          icon: ProgressiveIcon,
          title: 'Progressive web applications',
          description: 'Our job is not only to <strong>write code</strong>. In the beginning of a project it is necessary to plan the whole implementation based on a <strong>business case</strong>. Database structure, front-ends, backend endpoints, data flows…'
        },
        {
          icon: ServiceSideIcon,
          title: 'APIs & server-side applications',
          description: 'Our job is not only to <strong>write code</strong>. In the beginning of a project it is necessary to plan the whole implementation based on a business case. Database structure, <strong>front-ends</strong>, backend endpoints, data flows…'
        },
        {
          icon: CmsIcon,
          title: 'CMS integrations',
          description: 'Our job is not only to <strong>write code</strong>. In the beginning of a project it is necessary to plan the whole implementation based on a <strong>business case</strong>. Database structure, front-ends, backend endpoints, data flows…'
        },
        {
          icon: SoftwareArchitectureIcon,
          title: 'Software architecture',
          description: 'Our job is not only to <strong>write code</strong>. In the beginning of a project it is necessary to plan the whole implementation based on a business case. Database structure, <strong>front-ends</strong>, backend endpoints, data flows…'
        },
        {
          icon: ConsultingIcon,
          title: 'Consulting and audits',
          description: 'Our job is not only to <strong>write code</strong>. In the beginning of a project it is necessary to plan the whole implementation based on a <strong>business case</strong>. Database structure, front-ends, backend endpoints, data flows…'
        }
      ]
    }
  }
}
</script>
