The following lists the collective changes made to the specified OVAL versions to arrive at the current OVAL Language version. 

----------------------------------
UNIX 5.11.1:1.0
----------------------------------
* Fixed multiple Schematron rules referencing an incorrect Object, or using an OVAL Sandbox XML namespace. Issue #235.
* Added sunrpc_tcp and sunrpc_udp enumeration values to EntityStateEndpointType. Issue #251.
* Expanded datatype restrictions to be either string or int to remove backwards incompatibility for file_*/(group_id,user_id, a_time, c_time, m_time), password_*/(user_id, group_id), and shadow_*/(chg_lst, chg_allow, chg_req, exp_warn, exp_inact, exp_date) entities. Issue #244.


----------------------------------
Windows 5.11.1:1.0
----------------------------------
* Deprecated reg_dword_little_endian and reg_qword_little_endian registry types. Added reg_resource_list, reg_full_resource_descriptor, and reg_resource_requirements_list registry type enumerations. Issue #243.
* Fixed documentation on TIMEQ_FOREVER value. Issue #189.

----------------------------------
MacOS 5.11.1:1.0
----------------------------------
* Fixed multiple Schematron rules referencing an incorrect Object, or using an OVAL Sandbox XML namespace. Fixes duplicate Schematron pattern names. Issue #235.

----------------------------------
Linux 5.11.1:1.0
----------------------------------
* Deprecated nomd5 option for RpmVerifyFileBehaviors. Added nofiledigest and nocaps options to RpmVerifyFileBehaviors. Added filedigest_differs entities to replace md5_differs entities for rpmverifyfile_[state|item]. Issue #249.
* Fixed duplicate Schematron pattern ID. Issue #253.

----------------------------------
Independent 5.11.1:1.0
----------------------------------
* Included missing Family enumeration values in EntityItemFamilyType and EntityStateFamilyType. Issue #247.

----------------------------------
Cisco IOS-XE 5.11.1:1.0
----------------------------------
* Deprecated urpf_command and replaced with ipv4_urpf_command  and ipv6_urpf_command entities. interface* switchport_native_vlan entity type expanded to include int type. interface* switchport_access_vlan entity type expanded to include string type. acl_item config_line changed to maxOccurs="unbounded". interface_item ipv4_address entity changed to maxOccurs="1".Issue #241.

----------------------------------
Cisco IOS 5.11.1:1.0
----------------------------------
* Deprecated urpf_command and replaced with ipv4_urpf_command  and ipv6_urpf_command entities. interface* switchport_native_vlan entity type expanded to include int type. interface* switchport_access_vlan entity type expanded to include string type. acl_item config_line changed to maxOccurs="unbounded". interface_item ipv4_address entity changed to maxOccurs="1". Issue #240.

----------------------------------
Cisco ASA 5.11.1:1.0
----------------------------------
* Deprecated urpf_command and replaced with ipv4_urpf_command  and ipv6_urpf_command entities. interface_item ipv4_address entity changed to maxOccurs="1". Issue #242
* Fixed duplicate Schematron pattern name for "asa_service_policy_object_verify_filter_state". Issue #252.

----------------------------------
Apple iOS 5.11.1:1.0
----------------------------------
* Fixed erroneous variable reference in "apple-ios-def_profile_object_verify_filter_state" Schematron pattern. Issue #252.

----------------------------------
Version 5.11.0
----------------------------------
* Added new optional platform attribute to schema_version generator element to declare platform extension versions rather than incorrect usage of the xmlns attribute as previously documented. Issue #236.
* Re-implemented Notes using substitution groups that allow for backwards compatibility with Notes elements defined from oval-def. Issue #237.
* Corrected documentation for the GlobToRegexFunctionType evaluation results. Included evaluation tables and improved text formatting. Issue #245.
* Added check_existence attribute to State entities. Issue #191.
* Introduced new debian_evr_string simple datatype. This will distinguish rpm and dpkg evr values since they use different algorithms for comparison. Sandbox Repository Issue #142.