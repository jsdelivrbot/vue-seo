<script>
  import Displayer from '../mixins/displayer.vue'
  import TitleDisplayer from './titleDisplayer.vue'
  import OrgaizationDisplayer from './organizationDisplayer.vue'
  import WebsiteDisplayer from './websiteDisplayer.vue'
  import BreadcrumbsDisplayer from './breadcrumbsDisplayer.vue'
  import CanonicalDisplayer from './canonicalDisplayer.vue'
  import LangDispalyer from './langDisplayer.vue'
  import DescriptionDisplayer from './descriptionDisplayer.vue'

  export default {
    name: 'GoogleDisplayer',
    mixins: [Displayer],
    created () {
      this.supportedDisplayers = [
        TitleDisplayer,
        OrgaizationDisplayer,
        WebsiteDisplayer,
        BreadcrumbsDisplayer,
        CanonicalDisplayer,
        LangDispalyer,
        DescriptionDisplayer
      ];
    }
  }
</script>
