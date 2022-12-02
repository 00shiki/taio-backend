## Routing Table
1. GET '/search', 'SearchController@index'
2. GET '/following', 'HomeController@following'
3. POST '/follow', 'UserController@follow_v2'
4. POST '/unfollow', 'UserController@unfollow_v2'
5. GET '/follow/{uuid}', 'UserController@follow'
6. GET '/unfollow/{uuid}', 'UserController@unfollow'
7. GET '/doc_preview/download/{uuid}/{name?}', 'HomeController@download_doc_preview'
8. POST '/profile_photo/upload', 'UserController@upload_profile_photo'
9. GET '/intro_shown', 'HomeController@intro_shown'
10. GET '/signature/{uuid}', 'SignatureController@show_sign'
11. GET '/profile_photo/of/{username}', 'HomeController@get_user_profile_photo'
12. GET '/profile', 'HomeController@profile'
13. GET '/profile/edit', 'UserController@edit'
14. POST '/profile/edit', 'UserController@update'
15. GET '/{username?}', 'HomeController@index'

### Signature Group
1. GET '/generated', 'HomeController@generated'
2. GET '/request', 'HomeController@request'
3. GET '/requested/{filter?}', 'HomeController@requested'
4. GET '/get/description/{uuid}', 'HomeController@get_signature_description')
5. GET '/generated/download/{uuid}', 'HomeController@download_signature'
6. POST '/generate/export', 'ExportController@export_generated'
7. GET '/generate/{mode?}', 'SignatureController@gen_sign_form'
8. POST '/generate/live', 'SignatureController@generate_with_live_signature'
9. POST '/sign', 'SignatureController@sign_it'
10. POST '/live/sign' , 'SignatureController@sign_with_live_signature'
11. POST "/sign/bulk", "SignatureController@bulk_sign_with_sample"
12. POST "/sign/bulk/live", "SignatureController@bulk_sign_live_signature"
13. POST '/refuse', 'SignatureController@refuse_request'
14. POST '/submit/request', 'SignatureController@store'
15. POST '/cancel/request', 'SignatureController@cancel_request'
16. GET '/ask/{username}', 'SignatureController@ask_sign_form'
17. POST '/sample/upload', 'SignatureController@upload_sample'
18. POST '/sample/file/upload', 'SignatureController@upload_file_sample'
19. GET '/sample/preview/{signature_file_id}', 'SignatureController@sample_signature_preview'
20. GET '/pdf/edit/{signature_id}', 'SignatureController@pdf_editor'

### Auth API Documentation
Link : https://documenter.getpostman.com/view/18604848/2s8YzL56yX
