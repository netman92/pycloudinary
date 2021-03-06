
1.1.3 / 2015-07-05
==================

  * Increment version to 1.1.3
  * Add `max_length` to settings.

1.1.2 / 2015-06-22
==================

  * Update USER_AGENT. Remove max_length restriction from CloudianryField. Rename and reformat CHANGES.txt.   * Version 1.1.2   * Update `USER_AGENT` format and allow the setting of `USER_PLATFORM`   * Remove `max_length` restriction from `CloudinaryField`   * Reformat CHANGES.txt and rename it to CHANGELOG.md   * Change PyPI package classifier to "Development Status :: 5 - Production/Stable"

1.1.2 / 2015-06-22
==================

  * Increment version to 1.1.2
  * Update `USER_AGENT` format and allow the setting of `USER_PLATFORM`
  * Remove `max_length` restriction from `CloudinaryField`
  * Reformat CHANGES.txt and rename it to CHANGELOG.md
  * Change PyPI package classifier to "Development Status :: 5 - Production/Stable"

1.1.1 / 2015-04-17
==================

  * Increment to v1.1.1
  * Update README.md
  * python3 compatibility fixes. Solves #50
  * Solve resource_type default missing in CloudinaryResource

1.1.0 / 2015-04-07
==================

  * Increment to v1.1.0 - Support saving non-image resource types in CloudinaryField. Support storing type information in database. Support video tag and video thumbnail generation. Support video transformation parameters. Support eager_notification_url and eager_async in explicit. Support ftp urls in upload. upload large enhancements. Python3 compatibility fixes.
  * Make context check more resilient
  * Python3 compat for cloudinary_direct_upload_field
  * Fix video public_id cleansing pattern
  * Endpoint upload_chunked is no longer needed
  * Solve Python3 compatiblity issues
  * Support html attributes in video tag
  * upload large - test exact size
  * Simplify URL detection RE in uploader
  * Fix references to CloudinaryImage
  * Support new upload_chunked endpoint for large uploads. Fix random_public_id.
  * Support ftp urls in upload
  * Support eager_notification_url and eager_async in explicit
  * Support video tag and video thumbnail generation
  * Support saving non-image resource types in CloudinaryField. Support storing type information in database
  * Support video transformation parameters
  * signed_preloaded_image - allow integer version

1.0.21 / 2015-02-12
===================

  * Increment version to v1.0.21: Allow root path for shared CDN
  * Allow root path for shared CDN
  * Change url for test image from logo to old_logo

1.0.20 / 2015-01-01
===================

  * Increment version to v1.0.20: Solve python3 incomptibility errors
  * Solve python3 incomptibility errors

1.0.19 / 2014-12-21
===================

  * Increment version to v1.0.19: Folder listing. Support tags in upload_large. URL suffix, root URL and secure domain sharding. Support invalidate in bulk delete. GAE support. Allow uploader.upload_image to work on raw files. Support return_delete_token flag in upload. Support custom_coordinates in upload, explicit and update, coordinates flag in resource details. Update jQuery plugin to v1.0.21.
  * invalidate in bulk delete
  * folder listing. tags in upload_large, url suffix and root ur and secure domain sharding
  * add support for GAE. add sample GAE
  * Allow uploader.upload_image to work on raw files
  * Support return_delete_token flag in upload
  * Support custom_coordinates in upload, explicit and update, coordinates flag in resource details

1.0.18 / 2014-07-07
===================

  * Increment version to v1.0.18: Support for density pixel ratio (dpr) transformation parameter. Support auto width, auto dpr and responsive width. Support for background_removal parameter in upload and update. Upgrade jQuery plugin to v1.0.18. Support timeouts in API requests. Fix return_error mode when calling api. Allow user to override secure setting. Replace Exception with ValueError. Support auto-securing URLs if django request is enabled and the current page is being served over HTTPS.
  * Fix tests to reflect prefix + direction=desc is not supported
  * Support for background_removal parameter in upload and update
  * Support width auto, dpr auto and responsive width
  * Fix return_error mode when calling api
  * Merge pull request #35 from ndparker/master
  * Merge pull request #34 from MatthiasEgli/master
  * add the possibility to add timeouts to api requests
  * added transformation option DPR
  * Merge pull request #33 from Tekco/master
  * Allow user to override secure setting.
  * Added support for auto-securing URLs if django.core.context_processors.request is enabled and the current page is being served over HTTPS according to request.is_secure().
  * Issue #32 - Replace Exception with ValueError

1.0.17 / 2014-04-29
===================

  * Increment to version 1.0.17: Support upload_presets. Support unsigned uploads. Support start_at for resource listing. Support phash for upload and resource details. Support for passing filename to upload_options. Use index of version_info tuple rather than named (added in 2.7). Added introspection rule for Django South. Allow using module when django is available but not configured. Update jQuery library to v1.0.14.
  * Issue #30 - allow using module when django is available but not configured
  * Support upload_presets. Support unsigned uploads. Support start_at for resource listing. Support phash for upload and resource details
  * Support for passing filename to upload_options
  * Merge pull request #29 from Tekco/master
  * Added introspection rule for Django South
  * Use index of version_info tuple rather than named (added in 2.7)

1.0.16 / 2014-03-25
===================

  *  Increment to version 1.0.16: Support for python3, Update forms.py, Upgrade to v1.0.13 of the jQuery plugin.
  * Merge pull request #27 from Jkettler/master
  * Update forms.py
  * Python3 - Add missing conversions from bytes to unicode
  * Support for python3. Thanks to @koorgoo

1.0.15 / 2014-02-26
===================

  * Increment to version 1.0.15: Admin API update method. Admin API listing by moderation kind and status. Support moderation status in admin API listing. Support moderation flag in upload.  New upload and update API parameters: moderation, ocr, raw_conversion, categorization, detection, similarity_search and auto_tagging. Support uploading large raw files.
  * Support for update admin API. Support new moderations and resource info requests. Support uploading large raw files.

1.0.14 / 2014-02-11
===================

  * Increment to version 1.0.14: Embedding the external poster package to avoid pip 1.5.x errors. Add support for direction in resource listing.
  * add support for direction in resource listing. fix resource listing tests. add very basic sample Flask project.
  * skip delete all derived test by deault

1.0.13 / 2014-01-09
===================

  * Increment to version 1.0.13: Support overwrite upload parameter. Support tags in admin API resource listing. Support specifying face coordinates in upload API. Support specifying context (currently alt and caption) in upload API and returning context in API. Support specifying allowed image formats in upload API. Support listing resources in admin API by multiple public IDs. Send User-Agent header with client library version in API request. Support for signed-URLs to override restricted dynamic URLs. Use api.Error instead of Exception in uploader module. Support deleting all resources in Admin API.
  * add user agent
  * support for: context, allowed_formats, face_coordinates, signed_url, search by public ids, context and tags in lists
  * Merge pull request #24 from stylight/master
  * uploader module: Use api.Error instead of Exception
  * add delete_all_resources, add support for overwrite flag in upload, add support for tags flag in resources_by_tag, add support for query parameters in CLOUDINARY_URL

1.0.12 / 2013-11-04
===================

  * Increment to version 1.0.12: CloudinaryJsFileField - Handle validation errors in form by redering hidden field with previous upload result. Support unique_filename. Support color transformation parameter.
  * CloudinaryJsFileField - Handle validation errors in form by redering hidden field with previous upload result
  * add support unique fiename and correctly handle boolean upload parameters
  * Support color transformation parameter

1.0.11 / 2013-10-20
===================

  * Increment version to v1.0.11: Fix issue when CloudinaryInput with options is rendered twice.
  * Fix issue when CloudinaryInput with options is rendered twice

1.0.10 / 2013-08-07
===================

  * Increment version to v1.0.10: Support ping to Admin API, Support folder and proxy upload parameters, Escape non-http public_ids. Correct escaping of space and '-'.
  * Escape non-http public_ids. Correct escaping of space and -
  * Support folder and proxy upload parameters
  * Support ping to Admin API

1.0.9 / 2013-07-30
==================

  * Increment version to v1.0.9: Support raw data URI, Change secure urls to use *res.cloudinary.com.
  * Fix cloudinary-a.akamaihd.net links in README
  * Change secure urls to use *res.cloudinary.com
  * Support raw data URI
  * Fixing issues link
  * Adding links to Django documentation and getting started guide

1.0.8 / 2013-07-01
==================

  * Increment version to v1.0.8: Issue #18 - Support for other types in addition to 'upload', Fixed issue where a parameter may not be set to 0, Fixed bug with a couple ivars not being set in init, Support discard_original_filename, Support s3 and data:uri urls, Support for zip_download_url. Cleanup of signing code.
  * Support for zip_download_url. Cleanup of signing code
  * Support s3 and data:uri urls
  * Support discard_original_filename
  * Merge pull request #22 from spothero/master
  * Fixed bug with a couple ivars not being set in init.
  * Merge pull request #20 from spothero/master
  * quick fix.
  * Fixed issue where a parameter may not be set to 0.
  * Issue #18 - Support for other types in addition to 'upload'
  * Updating readme to link to samples

1.0.7 / 2013-05-01
==================

  * Increment version to v1.0.7: Add metadata to CloudinaryImage in upload. Support CloudinaryImage in the cloudinary_url templatetag. Invalidate flags in upload and destroy. Private download link generator. Shorten URL support. Support for folders. Support unsafe transformation update. Support rename
  * Fix handling of url_options in CloudinaryImage
  * Add metadata to CloudinaryImage in upload
  * Support CloudinaryImage in the cloudinary_url templatetag
  * Invalidate flags in upload and destroy
  * Private download link generator
  * Shorten URL support
  * Support for folders
  * Basic sample: not running cleanup in default, minor text changes
  * Merge branch 'fixes' of https://github.com/m0she/pycloudinary
  * Support unsafe transformation update
  * Support rename
  * sample/basic - Add documentations
  * sample/basic - make more first-time-user-friendly
  * Minor merge before release
  * Merge branch 'master' of github.com:cloudinary/pycloudinary
  * Issue #15 - Support blank=True in CloudinaryField

1.0.6 / 2013-03-25
==================

  * Increment version to v1.0.6: Support Django 1.5, Add cloudinary_direct_upload_field, cloudinary_js_config, cloudinary_url templatetags, Add basic sample, Update documentation
  * version 1.0.5
  * Django 1.5 support
  * Update documentation
  * add cloudinary_direct_upload_field and cloudinary_js_config templatetags
  * cloudinary templatetag - accept an options_dict arg
  * add cloudinary_url templatetag, fix build_url and image in CloudinaryImage
  * CloudinaryField - support image without format
  * samples/basic - add cleanup
  * samples - create basic sample

1.0.5 / 2013-03-14
==================

  * Increment version to v1.0.5: Akamai CDN Support
  * Akamai support

1.0.4 / 2013-03-12
==================

  * Increment version to v1.0.4: Fix tag handing methods of api, Support for sprite, multi and explode apis. Support for new async and notification params, Support for usage API call, Support js files needed for client side image processing in jquery direct upload, Support new image_metadata flag in upload and admin API, Use width/height even if crop is not given
  * Fix tag handing methods of api
  * Support for sprite, multi and explode apis. Support for new async and notification params
  * Support for usage API call
  * Fix whitespace issues after merge
  * Merge branch 'b1'
  * Support js files needed for client side image processing in jquery direct upload
  * Support new image_metadata flag in upload and admin API
  * Use width/height even if crop is not given
  * Fixing indentation
  * Fixing indentation

1.0.3 / 2013-01-20
==================

  * Increment version to v1.0.3: Open uploaded file in binary mode to solve python windows issues.
  * Open uploaded file in binary mode to solve python windows issues

1.0.2 / 2013-01-15
==================

  * Increment version to v1.0.2: Supporting opacity transformation parameter, Allow giving pages flag to resource details API.
  * Supporting opacity transformation parameter
  * Allow giving pages flag to resource details API

1.0.1 / 2012-11-22
==================

  * Increment version to v1.0.1: Fix issue 8 - error in serialization, Support for info flags in upload.
  * Support for info flags in upload
  * Issue 8 - error in serialization

1.0.0 / 2012-10-28
==================

  * Increment version to v1.0.0: Renamed url method of CloudinaryImage to build_url to avoid conflicts with the url property. Support keep_original in resource deletion. Support delete_resources_by_tag, Allow supplying unicode url in cloudinary.uploader.upload, Support passing parameters to cloudinary upload. Support upload parameters based on model in CloudinaryField, Support for transformation flags.
  * Support for transformation flags
  * Merge branch 'master' of github.com:cloudinary/pycloudinary
  * Support passing parameters to cloudinary upload. Support upload parameters based on model in CloudinaryField
  * Allow supplying unicode url in cloudinary.uploader.upload
  * Support delete_resources_by_tag Support keep_original in resource deletion

0.2.8 / 2012-10-08
==================

  * Increment version to v0.2.8: Change delete_resources_by_prefix to match other signatures, Support max_results in resource drilldown, Support for border and delay.
  * Change delete_resources_by_prefix to match other signatures
  * Support max_results in resource drilldown
  * Support for border and delay

0.2.7 / 2012-10-02
==================

  * Increment version to v0.2.7: Support cname, Support headers. Support format in eager. Support explicit. Support type in tags. Support unicode in CloudinaryImage.image. Depend on Django staticfiles module only if CloudinaryJsFileField is used with callback support. Fix to to_python error for submitting blank file.. Pass new flags to resource information api.
  * Pass new flags to resource information api
  * egg fix
  * fix new version
  * fix to to_python error for submitting blank file
  * Merge branch 'master' of github.com:cloudinary/pycloudinary
  * Depend on Django staticfiles module only if CloudinaryJsFileField is used with callback support
  * Support unicode in CloudinaryImage.image
  * Support headers. Support format in eager. Support explicit. Support type in tags
  * Support cname

0.2.6 / 2012-08-27
==================

  * Increment version to v0.2.6: Wrapper for Cloudinary management API, Better integration with JS library for direct uploads, Allow supplying default formfield for CloudinaryField model field, Do not pass width/height to html in case of crop fit or limit and in case of angle.
  * Do not pass width/height to html in case of crop fit or limit and in case of angle
  * Allow supplying default formfield for CloudinaryField model field
  * Helper method to initialize callback for IE CORS support
  * Better integration with JS library. Fix CloudinaryJsFormField
  * Wrapper for Cloudinary management API

0.2.5 / 2012-07-27
==================

  * Increment version to v0.2.5: Fix case in which Django is in python path but not used, Support density and page. Support http public ids in non-fetch types (e.g. vimeo)
  * Merge branch 'master' of github.com:cloudinary/pycloudinary
  * Support density and page. Support http public ids in non-fetch types (e.g. vimeo)
  * Fix case in which Django is in python path but not used

0.2.4 / 2012-07-23
==================

  * Increment version to v0.2.4: Fix bug when assigning None to CloudinaryField, Fixed handling of django based settings, Update README.md
  * Update README.md
  * Fixed handling of django based settings
  * Fix bug when assigning None to CloudinaryField

0.2.3 / 2012-07-13
==================

  * Increment version to v0.2.3: Fix serialization of CloudinaryImage when version is a number
  * Fix serialization of CloudinaryImage when version is a number

0.2.2 / 2012-07-12
==================

  * Increment version to v0.2.2: Allow saving an CloudinaryField assigned with CloudinaryImage with no format and version
  * Allow saving an CloudinaryField assigned with CloudinaryImage with no format and version
  * Updating readme to show pip install notes
  * Renaming package to 'cloudinary'
  * More config changes
  * Configuration changes for packaging
  * Support backup flag for uploads
  * Underlay support. Don't pass width/height to html if overlay/underlay are used
  * Integration with cloudinary JS library for direct upload to cloudinary
  * CloudinaryFileField which allows easy upload via the server
  * Support effect parameter. Rename effects to effect to avoid confusion
  * Merge branch 'master' of github.com:cloudinary/pycloudinary
  * Fetch format and effects parameters support
  * Update README.md
  * Markdown fixes

0.2 / 2012-05-10
================

  * Increament version to 0.2
  * Initial documentation of new features - with actual documentation
  * Initial documentation of new features
  * Support for CloudinaryField model field and form field. Direct upload helper
  * Support for CLOUDINARY_URL env variable Support text image generation Support angle and overlay
  * Switch from pycurl to poster to allow open files to be uploaded
  * Initial documentation
  * Initial commit
