FROM samerali/wodby-php:5.6

    # Install Drupal Console
RUN su-exec www-data composer global require drupal/console && \
    su-exec www-data drupal init && \

    # Install drush
    su-exec www-data composer global require drush/drush && \

    su-exec www-data composer clear-cache
