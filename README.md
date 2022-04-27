# Todos los hooks que estan presentes en SMF2.1.x 

Todo los hooks a qui https://github.com/dhayzon/SMF-hooksList/wiki
```
Admin.php   call_integration_hook('integrate_admin_search',array(&$language_files,&$include_files,&$settings_search));
Admin.php   call_integration_hook('integrate_manage_logs',array(&$log_functions));
Attachments.php   call_integration_hook('integrate_attachment_upload',array());
BoardIndex.php   call_integration_hook('integrate_mark_read_button');
Calendar.php   call_integration_hook('integrate_calendar_buttons');
Display.php   call_integration_hook('integrate_display_buttons',array(&$context['normal_buttons']));
Display.php   call_integration_hook('integrate_mod_buttons',array(&$context['mod_buttons']));
Display.php   call_integration_hook('integrate_prepare_display_context',array(&$output,&$message,$counter));
Display.php   call_integration_hook('integrate_query_message',array(&$msg_selects,&$msg_tables,&$msg_parameters));
Display.php   call_integration_hook('integrate_display_message_list',array(&$messages,&$posters));
Display.php   call_integration_hook('integrate_poll_buttons');
Display.php   call_integration_hook('integrate_display_topic',array(&$topic_selects,&$topic_tables,&$topic_parameters));
Errors.php   call_integration_hook('integrate_output_error',array($message,$error_type,$error_level,$file,$line));
Errors.php   call_integration_hook('integrate_error_types',array(&$other_error_types,&$error_type,$error_message,$file,$line));
Groups.php   call_integration_hook('integrate_manage_groups',array(&$subActions));
Help.php   call_integration_hook('integrate_helpadmin');
Help.php   call_integration_hook('integrate_manage_help',array(&$subActions));
Likes.php   call_integration_hook('integrate_issue_like',array($this));
Likes.php   call_integration_hook('integrate_likes_json_response',array(&$print));
Likes.php   call_integration_hook('integrate_valid_likes',array($this->_type,$this->_content,$this->_sa,$this->_js,$this->_extra));
Likes.php   call_integration_hook('integrate_issue_like_before',array(&$type,&$content,&$user,&$time));
Load.php   call_integration_hook('integrate_load_average',array($modSettings['load_average']));
Load.php   call_integration_hook('integrate_pre_load');
Load.php   if(count($integration_ids=call_integration_hook('integrate_verify_user'))>0)
Load.php   call_integration_hook('integrate_force_tfasetup',array(&$force_tfasetup));
Load.php   call_integration_hook('integrate_verify_tfa',array($id_member,$user_settings));
Load.php   call_integration_hook('integrate_user_info');
Load.php   call_integration_hook('integrate_load_min_user_settings_columns',array(&$columns_to_load));
Load.php   call_integration_hook('integrate_load_min_user_settings',array(&$user_info_min));
Load.php   call_integration_hook('integrate_load_board',array(&$custom_column_selects,&$custom_column_parameters));
Load.php   call_integration_hook('integrate_board_info',array(&$board_info,$row));
Load.php   call_integration_hook('integrate_load_member_data',array(&$select_columns,&$select_tables,&$set));
Load.php   call_integration_hook('integrate_member_context',array(&$memberContext[$user],$user,$display_custom_fields));
Load.php   call_integration_hook('integrate_pre_load_theme',array(&$id_theme));
Load.php   call_integration_hook('integrate_simple_actions',array(&$simpleActions,&$simpleAreas,&$simpleSubActions,&$extraParams,&$xmlActions));
Load.php   call_integration_hook('integrate_load_theme');
Load.php   if(function_exists('call_integration_hook'))
Load.php   call_integration_hook('pre_cache_quick_get',array(&$key,&$file,&$function,&$params,&$level));
Load.php   if(function_exists('call_integration_hook'))
Load.php   call_integration_hook('post_cache_quick_get',array(&$cache_block));
Load.php   if(function_exists('call_integration_hook'))
Load.php   call_integration_hook('cache_put_data',array(&$key,&$value,&$ttl));

Load.php   call_integration_hook('cache_get_data',array(&$key,&$ttl,&$value));
Load.php   call_integration_hook('integrate_clean_cache');
Load.php   call_integration_hook('integrate_set_avatar_data',array(&$image,&$data));
Logging.php   call_integration_hook('integrate_log_types',array(&$log_types,&$always_log));
LogInOut.php   if(in_array('retry',call_integration_hook('integrate_validate_login',array($_POST['user'],isset($_POST['passwrd'])?$_POST['passwrd']:null,$modSettings['cookieTime'])),true))
LogInOut.php   call_integration_hook('integrate_other_passwords',array(&$other_passwords));
LogInOut.php   call_integration_hook('integrate_login',array($user_settings['member_name'],null,$modSettings['cookieTime']));
LogInOut.php   call_integration_hook('integrate_logout',array($user_settings['member_name']));
ManageAttachments.php   call_integration_hook('integrate_manage_attachments',array(&$subActions));
ManageAttachments.php   call_integration_hook('integrate_modify_attachment_settings',array(&$config_vars));
ManageAttachments.php   call_integration_hook('integrate_save_attachment_settings');
ManageAttachments.php   call_integration_hook('integrate_modify_avatar_settings',array(&$config_vars));
ManageAttachments.php   call_integration_hook('integrate_save_avatar_settings');
ManageAttachments.php   call_integration_hook('integrate_attachments_browse',array(&$listOptions,&$titles,&$list_title));
ManageAttachments.php   call_integration_hook('integrate_attachment_remove',array(&$filesRemoved,$attachments));
ManageAttachments.php   call_integration_hook('integrate_remove_attachments',array($attach));
ManageAttachments.php   call_integration_hook('integrate_repair_attachments_nomsg',array(&$ignore_ids,$_GET['substep'],$_GET['substep']+500));
ManageAttachments.php   call_integration_hook('integrate_approve_attachments',array($attachments));
ManageBans.php   call_integration_hook('integrate_manage_bans',array(&$subActions));
ManageBans.php   call_integration_hook('integrate_ban_edit_list',array(&$listOptions));
ManageBans.php   call_integration_hook('integrate_ban_edit_new',array());
ManageBans.php   call_integration_hook('integrate_ban_list',array(&$ban_items));
ManageBans.php   call_integration_hook('integrate_load_addtional_ip_ban',array(&$search_list));
ManageBans.php   call_integration_hook('integrate_edit_bans',array(&$ban_info,empty($_REQUEST['bg'])));
ManageBans.php   call_integration_hook('integrate_edit_bans_post',array());
ManageBans.php   call_integration_hook('integrate_save_triggers',array(&$ban_triggers,&$ban_group));
ManageBans.php   call_integration_hook('integrate_remove_triggers',array(&$items_ids,$group_id));
ManageBoards.php   call_integration_hook('integrate_manage_boards',array(&$subActions));
ManageBoards.php   call_integration_hook('integrate_boards_main');
ManageBoards.php   call_integration_hook('integrate_edit_category');
ManageBoards.php   call_integration_hook('integrate_edit_board');
ManageBoards.php   call_integration_hook('integrate_modify_board_settings',array(&$config_vars));
ManageBoards.php   call_integration_hook('integrate_save_board_settings');
ManageCalendar.php   call_integration_hook('integrate_manage_calendar',array(&$subActions));
ManageCalendar.php   call_integration_hook('integrate_modify_calendar_settings',array(&$config_vars));
ManageCalendar.php   call_integration_hook('integrate_save_calendar_settings');
ManageLanguages.php   call_integration_hook('integrate_modifylanguages',array(&$themes,&$lang_dirs,&$allows_add_remove,&$additional_string_types));
ManageLanguages.php   call_integration_hook('integrate_language_edit_helptext',array(&$special_groups));
ManageLanguages.php   call_integration_hook('integrate_save_language_settings',array(&$config_vars));
ManageLanguages.php   call_integration_hook('integrate_manage_languages',array(&$subActions));
ManageLanguages.php   call_integration_hook('integrate_language_settings',array(&$config_vars));
ManageMail.php   call_integration_hook('integrate_save_mail_settings');
ManageMail.php   call_integration_hook('integrate_modify_mail_settings',array(&$config_vars));
ManageMail.php   call_integration_hook('integrate_manage_mail',array(&$subActions));
ManageMaintenance.php   call_integration_hook('integrate_convert_msgbody',array($body_type));
ManageMaintenance.php   call_integration_hook('integrate_manage_maintenance',array(&$subActions));
ManageMembergroups.php   call_integration_hook('integrate_view_membergroup');
ManageMembergroups.php   call_integration_hook('integrate_modify_membergroup_settings',array(&$config_vars));
ManageMembergroups.php   call_integration_hook('integrate_save_membergroup_settings');
ManageMembergroups.php   call_integration_hook('integrate_save_membergroup',array((int)$_REQUEST['group']));
ManageMembergroups.php   call_integration_hook('integrate_manage_membergroups',array(&$subActions));
ManageMembergroups.php   call_integration_hook('integrate_pre_add_membergroup',array());
ManageMembergroups.php   call_integration_hook('integrate_add_membergroup',array($id_group,$postCountBasedGroup));
ManageMembers.php   call_integration_hook('integrate_activate',array($member['username']));
ManageMembers.php   call_integration_hook('integrate_view_members_params',array(&$params));
ManageMembers.php   call_integration_hook('integrate_manage_members',array(&$subActions));
ManageNews.php   call_integration_hook('integrate_manage_news',array(&$subActions));
ManageNews.php   call_integration_hook('integrate_modify_news_settings',array(&$config_vars));
ManageNews.php   call_integration_hook('integrate_save_news_settings');
ManagePaid.php   call_integration_hook('integrate_manage_subscriptions',array(&$subActions));
ManagePaid.php   call_integration_hook('integrate_delete_subscription',array($context['sub_id']));
ManagePaid.php   call_integration_hook('integrate_save_subscription',array(($context['action_type']=='add'?$id_subscribe:$context['sub_id']),$_POST['name'],$_POST['desc'],$isActive,$span,$cost,$_POST['prim_group'],$addgroups,$isRepeatable,$allowpartial,$emailComplete,$reminder));
ManagePermissions.php   call_integration_hook('integrate_manage_permissions',array(&$subActions));
ManagePermissions.php   call_integration_hook('integrate_modify_permission_settings',array(&$config_vars));
ManagePermissions.php   call_integration_hook('integrate_save_permission_settings');
ManagePermissions.php   call_integration_hook('integrate_load_permission_levels',array(&$groupLevels,&$boardLevels));
ManagePermissions.php   call_integration_hook('integrate_load_permissions',array(&$permissionGroups,&$permissionList,&$leftPermissionGroups,&$hiddenPermissions,&$relabelPermissions));
ManagePermissions.php   call_integration_hook('integrate_load_illegal_permissions');
ManagePermissions.php   call_integration_hook('integrate_load_illegal_guest_permissions');
ManagePermissions.php   call_integration_hook('integrate_post_moderation_mapping',array(&$mappings));
ManagePosts.php   call_integration_hook('integrate_manage_posts',array(&$subActions));
ManagePosts.php   call_integration_hook('integrate_save_censors',array(&$updates));
ManagePosts.php   call_integration_hook('integrate_censors');
ManagePosts.php   call_integration_hook('integrate_modify_post_settings',array(&$config_vars));
ManagePosts.php   call_integration_hook('integrate_save_post_settings');
ManagePosts.php   call_integration_hook('integrate_modify_topic_settings',array(&$config_vars));
ManagePosts.php   call_integration_hook('integrate_save_topic_settings');
ManageRegistration.php   call_integration_hook('integrate_manage_registrations',array(&$subActions));
ManageRegistration.php   call_integration_hook('integrate_modify_registration_settings',array(&$config_vars));
ManageRegistration.php   call_integration_hook('integrate_save_registration_settings');
ManageScheduledTasks.php   call_integration_hook('integrate_manage_scheduled_tasks',array(&$subActions));
ManageScheduledTasks.php   call_integration_hook('integrate_scheduled_tasks_settings',array(&$config_vars));
ManageScheduledTasks.php   call_integration_hook('integrate_save_scheduled_tasks_settings',array(&$save_vars));
ManageSearch.php   call_integration_hook('integrate_manage_search',array(&$subActions));
ManageSearch.php   call_integration_hook('integrate_modify_search_settings',array(&$config_vars));
ManageSearch.php   call_integration_hook('integrate_save_search_settings');
ManageSearch.php   call_integration_hook('integrate_modify_search_weights',array(&$factors));
ManageSearch.php   call_integration_hook('integrate_save_search_weights');
ManageSearchEngines.php   call_integration_hook('integrate_manage_search_engines',array(&$subActions));
ManageSearchEngines.php   call_integration_hook('integrate_modify_search_engine_settings',array(&$config_vars));
ManageSearchEngines.php   call_integration_hook('integrate_save_search_engine_settings');
ManageServer.php   call_integration_hook('integrate_server_settings',array(&$subActions));
ManageServer.php   call_integration_hook('integrate_general_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_general_settings');
ManageServer.php   call_integration_hook('integrate_database_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_database_settings');
ManageServer.php   call_integration_hook('integrate_cookie_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_cookie_settings');
ManageServer.php   call_integration_hook('integrate_general_security_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_general_security_settings');
ManageServer.php   call_integration_hook('integrate_modify_cache_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_cache_settings');
ManageServer.php   call_integration_hook('integrate_export_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_export_settings');
ManageServer.php   call_integration_hook('integrate_loadavg_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_save_loadavg_settings');
ManageServer.php   call_integration_hook('integrate_prepare_db_settings',array(&$config_vars));
ManageServer.php   call_integration_hook('integrate_load_cache_apis',array(&$loadedApis));
ManageSettings.php   call_integration_hook('integrate_modify_features',array(&$subActions));
ManageSettings.php   call_integration_hook('integrate_modify_modifications',array(&$subActions));
ManageSettings.php   call_integration_hook('integrate_modify_basic_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_basic_settings');
ManageSettings.php   call_integration_hook('integrate_modify_bbc_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_bbc_settings',array($bbcTags));
ManageSettings.php   call_integration_hook('integrate_layout_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_layout_settings');
ManageSettings.php   call_integration_hook('integrate_likes_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_likes_settings');
ManageSettings.php   call_integration_hook('integrate_mentions_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_mentions_settings');
ManageSettings.php   call_integration_hook('integrate_warning_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_warning_settings',array(&$save_vars));
ManageSettings.php   call_integration_hook('integrate_spam_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_spam_settings',array(&$save_vars));
ManageSettings.php   call_integration_hook('integrate_signature_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_apply_signature_settings',array(&$sig,$sig_limits,$disabledTags));
ManageSettings.php   call_integration_hook('integrate_save_signature_settings',array(&$sig_limits,&$bbcTags));
ManageSettings.php   call_integration_hook('integrate_prune_settings',array(&$config_vars,&$prune_toggle,false));
ManageSettings.php   call_integration_hook('integrate_prune_settings',array(&$savevar,&$prune_toggle,true));
ManageSettings.php   call_integration_hook('integrate_general_mod_settings',array(&$config_vars));
ManageSettings.php   call_integration_hook('integrate_save_general_mod_settings',array(&$save_vars));
ManageSmileys.php   call_integration_hook('integrate_manage_smileys',array(&$subActions));
ManageSmileys.php   call_integration_hook('integrate_modify_smiley_settings',array(&$config_vars));
ManageSmileys.php   call_integration_hook('integrate_save_smiley_settings');
Memberlist.php   call_integration_hook('integrate_memberlist_buttons');
Mentions.php   call_integration_hook('mention_insert_'.$content_type,array($content_id,&$members));
MessageIndex.php   call_integration_hook('integrate_pre_messageindex',array(&$sort_methods,&$sort_methods_table));
MessageIndex.php   call_integration_hook('integrate_message_index',array(&$message_index_selects,&$message_index_tables,&$message_index_parameters,&$message_index_wheres,&$topic_ids,&$message_index_topic_wheres));
MessageIndex.php   call_integration_hook('integrate_quick_mod_actions');
MessageIndex.php   call_integration_hook('integrate_messageindex_buttons',array(&$context['normal_buttons']));
ModerationCenter.php   call_integration_hook('integrate_warning_log_actions',array(&$subActions));
ModerationCenter.php   call_integration_hook('integrate_mod_centre_blocks',array(&$valid_blocks));
Modlog.php   call_integration_hook('integrate_viewModLog',array(&$listOptions,&$moderation_menu_name));
MoveTopic.php   call_integration_hook('integrate_movetopic2_end');
News.php   call_integration_hook('integrate_fix_url',array(&$val));
News.php   call_integration_hook('integrate_xml_data',array(&$xml_data,&$feed_meta,&$namespaces,&$extraFeedTags,&$forceCdataKeys,&$nsKeys,$xml_format,$subaction,&$doctype));
News.php   call_integration_hook('integrate_xmlfeeds',array(&$subActions));
PackageGet.php   call_integration_hook('integrate_package_upload');
PackageGet.php   call_integration_hook('integrate_package_download');
PackageGet.php   call_integration_hook('integrate_package_get',array(&$subActions));
Packages.php   call_integration_hook('integrate_packages_sort_id',array(&$sort_id,&$packages));
Packages.php   call_integration_hook('integrate_modification_types');
Packages.php   call_integration_hook('integrate_manage_packages',array(&$subActions));
PersonalMessage.php   call_integration_hook('integrate_pm_post');
PersonalMessage.php   call_integration_hook('integrate_pm_error');
PersonalMessage.php   call_integration_hook('integrate_search_pm_context');
PersonalMessage.php   call_integration_hook('integrate_conversation_buttons');
PersonalMessage.php   call_integration_hook('integrate_prepare_pm_context',array(&$output,&$message,$counter));
Poll.php   call_integration_hook('integrate_poll_remove',array($pollID));
Poll.php   call_integration_hook('integrate_poll_add_edit',array($bcinfo['id_poll'],$isEdit));
Poll.php   call_integration_hook('integrate_poll_vote',array(&$row['id_poll'],&$pollOptions));
Post.php   call_integration_hook('integrate_post2_end');
Post.php   call_integration_hook('integrate_poll_add_edit',array($id_poll,false));
Post.php   call_integration_hook('integrate_getTopic_previous_post',array(&$row));
Post.php   call_integration_hook('integrate_jsmodify_xml');
Post.php   call_integration_hook('integrate_post_JavascriptModify',array(&$post_errors,$row));
Post.php   call_integration_hook('integrate_post2_pre',array(&$post_errors));
Post.php   call_integration_hook('integrate_preview_post',array(&$form_message,&$form_subject));
Post.php   call_integration_hook('integrate_post_start');
Post.php   call_integration_hook('integrate_post_errors',array(&$post_errors,&$minor_errors,$form_message,$form_subject));
Post.php   call_integration_hook('integrate_post2_start',array(&$post_errors));
Post.php   call_integration_hook('integrate_post_end');
PostModeration.php   call_integration_hook('integrate_post_moderation',array(&$subActions));
Profile.php   call_integration_hook('integrate_pre_profile_areas',array(&$profile_areas));
Profile.php   call_integration_hook('integrate_load_custom_profile_fields',array($memID,$area));
Profile.php   call_integration_hook('integrate_profile_popup',array(&$profile_items));
Profile.php   call_integration_hook('integrate_reset_pass',array($cur_profile['member_name'],$cur_profile['member_name'],$_POST['passwrd2']));
Profile.php   call_integration_hook('integrate_profile_save',array(&$profile_vars,&$post_errors,$memID,$cur_profile,$current_area));
Profile.php   $good_password=in_array(true,call_integration_hook('integrate_verify_password',array($cur_profile['member_name'],$password,false)),true);
Profile-Actions.php   call_integration_hook('integrate_activate',array($user_profile[$memID]['member_name']));
Profile-Export.php   call_integration_hook('integrate_export_xslt_variables',array(&$xslt_variables,$format));
Profile-Export.php   call_integration_hook('integrate_export_xslt_stylesheet',array(&$stylesheet,$format));
Profile-Export.php   call_integration_hook('integrate_pre_javascript_output',array(false));
Profile-Export.php   call_integration_hook('integrate_pre_css_output');
Profile-Export.php   call_integration_hook('integrate_pre_javascript_output',array(true));
Profile-Modify.php   call_integration_hook('integrate_reset_pass',array($cur_profile['member_name'],$value,$_POST['passwrd1']));
Profile-Modify.php   call_integration_hook('after_profile_save_avatar');
Profile-Modify.php   call_integration_hook('integrate_view_buddies',array($memID));
Profile-Modify.php   call_integration_hook('integrate_load_profile_fields',array(&$profile_fields));
Profile-Modify.php   call_integration_hook('integrate_setup_profile_context',array(&$fields));
Profile-Modify.php   call_integration_hook('integrate_add_buddies',array($memID,&$new_buddies));
Profile-Modify.php   call_integration_hook('integrate_theme_options');
Profile-Modify.php   call_integration_hook('integrate_remove_buddy',array($memID));
Profile-Modify.php  call_integration_hook('integrate_save_custom_profile_fields',array(&$changes,&$log_changes,&$errors,$returnErrors,$memID,$area,$sanitize,&$deletes));
Profile-Modify.php   call_integration_hook('integrate_profile_profileSaveGroups',array($value,$additional_groups));
Profile-Modify.php   call_integration_hook('before_profile_save_avatar',array(&$value));
Profile-Modify.php   call_integration_hook('integrate_alert_types',array(&$alert_types,&$group_options));
Profile-View.php   call_integration_hook('integrate_profile_trackip',array($ip_string,$ip_var));
Profile-View.php   call_integration_hook('integrate_profile_stats',array($memID,&$context['text_stats']));
Profile-View.php   call_integration_hook('integrate_profile_showPosts');
Profile-View.php   call_integration_hook('integrate_fetch_alerts',array(&$alerts,&$formats));
Recent.php   call_integration_hook('integrate_recent_RecentPosts');
Recent.php   call_integration_hook('integrate_recent_buttons');
Recent.php   call_integration_hook('integrate_unread_list');
Register.php   call_integration_hook('integrate_activate',array($regOptions['username']));
Register.php   call_integration_hook('integrate_activate',array($row['member_name']));
Reminder.php   call_integration_hook('integrate_reset_pass',array($username,$username,$_POST['passwrd1']));
Reminder.php   call_integration_hook('integrate_reset_pass',array($row['member_name'],$row['member_name'],$_POST['passwrd1']));
RemoveTopic.php   call_integration_hook('integrate_pre_remove_message',array($message,$decreasePostCount,$row));
RemoveTopic.php   call_integration_hook('integrate_remove_message',array($message,$row,$recycle));
RemoveTopic.php   call_integration_hook('integrate_remove_topics_before',array($topics,$recycle_board));
RemoveTopic.php   call_integration_hook('integrate_remove_topics',array($topics));
ReportedContent.php   call_integration_hook('integrate_reported_'.$context['report_type'],array(&$subActions));
Reports.php   call_integration_hook('integrate_reports_boardperm',array(&$disabled_permissions));
Reports.php   call_integration_hook('integrate_reports_groupperm',array(&$disabled_permissions));
Reports.php   call_integration_hook('integrate_report_types');
Reports.php   call_integration_hook('integrate_report_buttons');
ScheduledTasks.php   call_integration_hook('integrate_daily_digest_email',array(&$email,$types,$notify_types,$langtxt));
ScheduledTasks.php   call_integration_hook('integrate_weekly_maintenance');
ScheduledTasks.php   call_integration_hook('integrate_daily_maintenance');
ScheduledTasks.php   call_integration_hook('integrate_daily_digest_lang',array(&$langtxt,$lang));
Search.php   call_integration_hook('integrate_search');
Search.php   call_integration_hook('integrate_search_weights',array(&$weight_factors));
Search.php   call_integration_hook('integrate_search_sort_columns',array(&$sort_columns));
Search.php   call_integration_hook('integrate_search_params',array(&$search_params));
Search.php   call_integration_hook('integrate_search_blacklisted_words',array(&$blacklisted_words));
Search.php   call_integration_hook('integrate_search_errors');
Search.php   call_integration_hook('integrate_subject_only_search_query',array(&$subject_query,&$subject_query_params));
Search.php   call_integration_hook('integrate_subject_search_query',array(&$subject_query));
Search.php   call_integration_hook('integrate_main_search_query',array(&$main_query));
Search.php   call_integration_hook('integrate_search_message_list',array(&$msg_list,&$posters));
Search.php   call_integration_hook('integrate_quick_mod_actions_search');
Search.php   call_integration_hook('integrate_search_message_context',array(&$output,&$message,$counter));
Security.php   call_integration_hook('integrate_validateSession',array(&$types));
Security.php   $good_password=in_array(true,call_integration_hook('integrate_verify_password',array($user_info['username'],$_POST[$type.'_pass'],false)),true);
Security.php   call_integration_hook('integrate_post_ban_permissions',array(&$denied_permissions));
Security.php   call_integration_hook('integrate_warn_permissions',array(&$permission_change));
Security.php   call_integration_hook('integrate_allowed_to_general',array(&$user_permissions,$permission));
Security.php   call_integration_hook('integrate_allowed_to_board',array(&$return,$permission,$boards,$any));
Security.php   call_integration_hook('integrate_heavy_permissions_session',array(&$heavy_permissions));
Security.php   call_integration_hook('integrate_boards_allowed_to',array(&$boards,$deny_boards,$permissions,$check_access,$simple));
Security.php   call_integration_hook('integrate_spam_protection',array(&$timeOverrides));
Session.php   call_integration_hook('integrate_load_session');
Session.php   call_integration_hook('integrate_session_handlers');
ShowAttachments.php   call_integration_hook('integrate_pre_download_request');
ShowAttachments.php   call_integration_hook('integrate_download_request',array(&$attachRequest));
SplitTopics.php   call_integration_hook('integrate_merge_topic',array($merged_topic,$updated_topics,$deleted_topics,$deleted_polls));
SplitTopics.php   call_integration_hook('integrate_split_topic',array($split1,$split2,$new_subject,$id_board));
Stats.php   call_integration_hook('integrate_forum_stats');
Subs.php   call_integration_hook('integrate_pre_parsebbc',array(&$message,&$smileys,&$cache_id,&$parse_tags));
Subs.php   call_integration_hook('integrate_attach_bbc_validate',array(&$returnContext,$currentAttachment,$tag,$data,$disabled,$params));
Subs.php   call_integration_hook('integrate_bbc_codes',array(&$codes,&$no_autolink_tags));
Subs.php   call_integration_hook('integrate_bbc_print',array(&$disabled));
Subs.php   call_integration_hook('integrate_autolinker_schemes',array(&$schemes));
Subs.php   call_integration_hook('integrate_post_parsebbc',array(&$message,&$smileys,&$cache_id,&$parse_tags));
Subs.php   call_integration_hook('integrate_smileys',array(&$smileyPregSearch,&$smileyPregReplacements));
Subs.php   call_integration_hook('integrate_proxy',array($url,&$proxied_url));
Subs.php   call_integration_hook('integrate_redirect',array(&$setLocation,&$refresh,&$permanent));
Subs.php   call_integration_hook('integrate_exit',array($do_footer));
Subs.php   call_integration_hook('integrate_theme_context');
Subs.php   call_integration_hook('integrate_security_files',array(&$securityFiles));
Subs.php   call_integration_hook('integrate_pre_javascript_output',array(&$do_deferred));
Subs.php   call_integration_hook('integrate_pre_css_output');
Subs.php   call_integration_hook('integrate_menu_buttons',array(&$buttons));
Subs.php   call_integration_hook('integrate_current_action',array(&$current_action));Subs.php   call_integration_hook('integrate_change_member_data',array($member_names,$var,&$data[$var],&$knownInts,&$knownFloats));
Subs-Admin.php   call_integration_hook('integrate_update_settings_file',array(&$settings_defs));
Subs-Admin.php   if(function_exists('call_integration_hook'))
Subs-Attachments.php   call_integration_hook('integrate_pre_parseAttachBBC',array($attachID,$msgID));
Subs-Attachments.php   call_integration_hook('integrate_post_parseAttachBBC',array(&$attachContext));
Subs-Attachments.php   call_integration_hook('integrate_createAttachment',array(&$attachmentOptions,&$attachmentInserts));
Subs-Attachments.php   call_integration_hook('integrate_attachment_upload',array());
Subs-Attachments.php   call_integration_hook('integrate_assign_attachments',array(&$attachIDs,&$msgID));
Subs-Auth.php   call_integration_hook('integrate_cookie_data',array($data,&$custom_data));
Subs-Auth.php   call_integration_hook('integrate_validateSession',array(&$types));
Subs-Auth.php   call_integration_hook('integrate_mod_cache');
Subs-Auth.php   call_integration_hook('integrate_validate_username',array($username,&$errors));
Subs-Auth.php   call_integration_hook('integrate_validatePassword',array($password,$username,$restrict_in,&$pass_error));
Subs-Auth.php   call_integration_hook('integrate_reset_pass',array($old_user,$user,$newPassword));
Subs-Auth.php   call_integration_hook('integrate_cookie',array($name,$value,$expire,$path,$domain,$secure,$httponly,$samesite));
Subs-BoardIndex.php   call_integration_hook('integrate_boardindex_board',array(&$this_category,$row_board));
Subs-BoardIndex.php   call_integration_hook('integrate_getboardtree',array($board_index_options,&$this_category));
Subs-BoardIndex.php   call_integration_hook('integrate_getboardtree',array($board_index_options,&$categories));
Subs-BoardIndex.php   call_integration_hook('integrate_pre_boardindex',array(&$board_index_selects,&$board_index_parameters));
Subs-Boards.php   call_integration_hook('integrate_pre_boardtree',array(&$boardColumns,&$boardParameters,&$boardJoins,&$boardWhere,&$boardOrder));
Subs-Boards.php   call_integration_hook('integrate_modify_board',array($id,$boardOptions,&$boardUpdates,&$boardUpdateParameters));
Subs-Boards.php   call_integration_hook('integrate_create_board',array(&$boardOptions,&$board_columns,&$board_parameters));
Subs-Boards.php   call_integration_hook('integrate_boardtree_board',array($row));
Subs-Boards.php   call_integration_hook('integrate_pre_modify_board',array($id,&$boardOptions));
Subs-Boards.php   call_integration_hook('integrate_delete_board',array($boards_to_remove,&$moveChildrenTo));
Subs-Calendar.php   call_integration_hook('integrate_remove_event',array($event_id));
Subs-Calendar.php   call_integration_hook('integrate_modify_event',array($event_id,&$eventOptions,&$event_columns,&$event_parameters));
Subs-Calendar.php   call_integration_hook('integrate_create_event',array(&$eventOptions,&$event_columns,&$event_parameters));
Subs-Categories.php   call_integration_hook('integrate_delete_category',array($categories,&$moveBoardsTo));
Subs-Categories.php   call_integration_hook('integrate_create_category',array(&$catOptions,&$cat_columns,&$cat_parameters));
Subs-Categories.php   call_integration_hook('integrate_pre_modify_category',array($cat_id,&$catOptions));
Subs-Categories.php   call_integration_hook('integrate_modify_category',array($cat_id,&$catUpdates,&$catParameters));
Subs-Editor.php   call_integration_hook('integrate_bbc_buttons',array(&$context['bbc_tags'],&$editor_tag_map));
Subs-Editor.php   call_integration_hook('integrate_sceditor_options',array(&$sce_options));
Subs-Editor.php   call_integration_hook('integrate_create_control_verification_pre',array(&$verificationOptions,$do_test));
Subs-Editor.php   call_integration_hook('integrate_load_message_icons',array(&$icons));
Subs-Editor.php   call_integration_hook('integrate_create_control_verification_refresh',array($thisVerification));
Subs-Editor.php   call_integration_hook('integrate_create_control_verification_post',array(&$verification_errors,$do_test));
Subs-Editor.php   call_integration_hook('integrate_autosuggest',array(&$searchTypes));
Subs-Editor.php   call_integration_hook('integrate_create_control_verification_test',array($thisVerification,&$verification_errors));
Subs-List.php   call_integration_hook('integrate_'.$listOptions['id'],array(&$listOptions));
Subs-Membergroups.php   call_integration_hook('integrate_getMembergroupList',array(&$groupCache,$group));
Subs-Membergroups.php   call_integration_hook('integrate_add_members_to_group',array($members,$group,&$group_names));
Subs-Membergroups.php   call_integration_hook('integrate_delete_membergroups',array($groups));
Subs-Members.php   call_integration_hook('integrate_check_name',array($checkName,&$is_reserved,$current_id_member,$is_name));
Subs-Members.php   call_integration_hook('integrate_register_after',array($regOptions,$memberID));
Subs-Members.php   call_integration_hook('integrate_reattribute_posts',array($memID,$email,$membername,$post_count,&$updated));
Subs-Members.php   call_integration_hook('integrate_groups_allowed_to',array(&$member_groups,$permission,$board_id));
Subs-Members.php   call_integration_hook('integrate_register_check',array(&$regOptions,&$reg_errors));
Subs-Members.php   call_integration_hook('integrate_delete_members',array($users));
Subs-Members.php   call_integration_hook('integrate_post_register',array(&$regOptions,&$theme_vars,&$memberID));
Subs-Members.php   call_integration_hook('integrate_register',array(&$regOptions,&$theme_vars,&$knownInts,&$knownFloats));
Subs-MembersOnline.php   call_integration_hook('integrate_online_stats',array(&$membersOnlineStats));
Subs-Menu.php   call_integration_hook('integrate_'.$menu_context['current_action'].'_areas',array(&$menuData));
Subs-Post.php   call_integration_hook('integrate_create_topic',array(&$msgOptions,&$topicOptions,&$posterOptions));
Subs-Post.php   call_integration_hook('integrate_after_approve_posts',array($approve,$msgs,$topic_changes,$member_post_changes));
Subs-Post.php   call_integration_hook('integrate_modify_post',array(&$messages_columns,&$update_parameters,&$msgOptions,&$topicOptions,&$posterOptions,&$messageInts));
Subs-Post.php   call_integration_hook('integrate_before_create_topic',array(&$msgOptions,&$topicOptions,&$posterOptions,&$topic_columns,&$topic_parameters));
Subs-Post.php   call_integration_hook('integrate_after_create_post',array($msgOptions,$topicOptions,$posterOptions,$message_columns,$message_parameters));
Subs-Post.php   call_integration_hook('integrate_create_post',array(&$msgOptions,&$topicOptions,&$posterOptions,&$message_columns,&$message_parameters));
Subs-Post.php   call_integration_hook('integrate_preparsecode',array(&$message,$previewing));
Subs-Post.php   call_integration_hook('integrate_personal_message',array(&$recipients,&$from,&$subject,&$message));
Subs-Post.php   if(in_array(false,call_integration_hook('integrate_outgoing_email',array(&$subject,&$message,&$headers,&$to_array)),true))
Subs-Post.php   call_integration_hook('integrate_modify_topic',array(&$topics_columns,&$update_parameters,&$msgOptions,&$topicOptions,&$posterOptions));
Subs-Post.php   call_integration_hook('integrate_personal_message_after',array(&$id_pm,&$log,&$recipients,&$from,&$subject,&$message));
Subs-Post.php   call_integration_hook('integrate_unpreparsecode',array(&$message));
Subs-Themes.php   call_integration_hook('integrate_theme_install',array(&$context['to_install'],$id_theme));
Subs-Themes.php   call_integration_hook('integrate_get_installed_themes',array(&$themeValues));
Subs-Themes.php   call_integration_hook('integrate_get_single_theme',array(&$variables,$id));
Subs-Themes.php   call_integration_hook('integrate_get_all_themes',array(&$themeValues,$enable_only));
Subs-Timezones.php   call_integration_hook('integrate_metazones',array(&$tzid_metazones,$when));
Subs-Timezones.php   call_integration_hook('integrate_country_timezones',array(&$sorted_tzids,$country_code,$when));
Subs-Timezones.php   call_integration_hook('integrate_timezone_fallbacks',array(&$fallbacks,&$missing,$tzids,$when));
Themes.php   call_integration_hook('integrate_manage_themes',array(&$subActions));
Themes.php   call_integration_hook('integrate_theme_options');
Themes.php   call_integration_hook('integrate_theme_settings');
Themes.php   call_integration_hook('integrate_wrap_action');
ViewQuery.php   call_integration_hook('integrate_egg_nog');
Who.php   call_integration_hook('whos_online_after',array(&$urls,&$data));
Who.php   call_integration_hook('integrate_credits');
Who.php   call_integration_hook('who_allowed',array(&$allowedActions));
Who.php   if(count($integrate_actions=call_integration_hook('integrate_whos_online',array($actions)))>0)
Xml.php   call_integration_hook('integrate_XMLhttpMain_subActions',array(&$subActions));
Likes-Notify.php   call_integration_hook('integrate_find_like_author',array($this->_details['content_type'],$this->_details['content_id']));
```
# Lista de archivos donde estan presentes los hooks
<details>
  <summary>/source/</summary>
     
1. Admin.php
1. Attachments.php
1. BoardIndex.php
1. Calendar.php
1. Display.php
1. Display.php~
1. Errors.php
1. Groups.php
1. Help.php
1. Likes.php
1. Load.php
1. Logging.php
1. LogInOut.php
1. ManageAttachments.php
1. ManageBans.php
1. ManageBoards.php
1. ManageCalendar.php
1. ManageLanguages.php
1. ManageMail.php
1. ManageMaintenance.php
1. ManageMembergroups.php
1. ManageMembers.php
1. ManageNews.php
1. ManagePaid.php
1. ManagePermissions.php
1. ManagePosts.php
1. ManageRegistration.php
1. ManageScheduledTasks.php
1. ManageSearch.php
1. ManageSearchEngines.php
1. ManageServer.php
1. ManageSettings.php
1. ManageSmileys.php
1. Memberlist.php
1. Mentions.php
1. MessageIndex.php
1. ModerationCenter.php
1. Modlog.php
1. MoveTopic.php
1. News.php
1. PackageGet.php
1. Packages.php
1. PersonalMessage.php
1. Poll.php
1. Post.php
1. PostModeration.php
1. Profile.php
1. Profile-Actions.php
1. Profile-Export.php
1. Profile-Modify.php
1. Profile-View.php
1. Recent.php
1. Register.php
1. Reminder.php
1. RemoveTopic.php
1. ReportedContent.php
1. Reports.php
1. ScheduledTasks.php
1. Search.php
1. Security.php
1. Session.php
1. ShowAttachments.php
1. SplitTopics.php
1. Stats.php
1. Subs.php
1. Subs-Admin.php
1. Subs-Attachments.php
1. Subs-Auth.php
1. Subs-BoardIndex.php
1. Subs-Boards.php
1. Subs-Calendar.php
1. Subs-Categories.php
1. Subs-Editor.php
1. Subs-List.php
1. Subs-Membergroups.php
1. Subs-Members.php
1. Subs-MembersOnline.php
1. Subs-Menu.php
1. Subs-Post.php
1. Subs-Themes.php
1. Subs-Timezones.php
1. Themes.php
1. ViewQuery.php
1. Who.php
1. Xml.php 
1. tasks\Likes-Notify.php
</details>
