Useful template tags and filters
================================

Next filters and tags can be used when `pybb_tags` loaded in template:

* `pybb_get_latest_topic` and `pybb_get_latest_posts` assigment tags you can use on
  every page for getting latest topics ans posts, for example for rendering in side block.
  Also you can pass `user` parameter (default to user from template context) for geting topics
  or posts available for specific user and `cnt` parameter for get specific count of topics
  or posts::

    {% pybb_get_latest_topic cnt=30 as topics %}
    {# operation on topics list there #}

* `pybb_get_profile` assigment tag can be used to get forum profile instance for any user
  passed as `user` argument::

    {% pybb_get_profile user=post.user as post_user_profile %}
    {# use profile fields there #}
