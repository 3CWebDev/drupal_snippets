<?php
/* Remove long state names from webform address/state options */
function ccc_custom_webform_element_alter(array &$element, \Drupal\Core\Form\FormStateInterface $form_state, array $context) {

  if ($element['#admin_title'] == 'State/Province'){
    $options = $element['#options'];
    foreach ($options as $key => $value) {
      if (strlen($value) > 15) {
        unset($options[$key]);
      }
    }
    $element['#options'] = $options;
  }
}
