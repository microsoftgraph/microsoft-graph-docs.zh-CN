<span data-ttu-id="20bce-p114">通过导航属性公开目录中的域和其他对象之间的关系（如它们的验证记录和服务配置记录）。你可以通过在请求中定位这些导航属性来读取这些关系。</span><span class="sxs-lookup"><span data-stu-id="20bce-p114">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

通过导航属性公开目录中的域和其他对象之间的关系（如它们的验证记录和服务配置记录）。你可以通过在请求中定位这些导航属性来读取这些关系。

| <span data-ttu-id="20bce-199">关系</span><span class="sxs-lookup"><span data-stu-id="20bce-199">Relationship</span></span> | <span data-ttu-id="20bce-200">类型</span><span class="sxs-lookup"><span data-stu-id="20bce-200">Type</span></span> |<span data-ttu-id="20bce-201">说明</span><span class="sxs-lookup"><span data-stu-id="20bce-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20bce-202">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="20bce-202">domainNameReferences</span></span>|<span data-ttu-id="20bce-203">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20bce-203">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="20bce-204">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="20bce-204">Read-only, Nullable</span></span>|
|<span data-ttu-id="20bce-205">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="20bce-205">serviceConfigurationRecords</span></span>|<span data-ttu-id="20bce-206">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20bce-206">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="20bce-207">Microsoft Online Services 可以使用域之前，客户添加到域 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="20bce-207">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="20bce-208">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="20bce-208">Read-only, Nullable</span></span> |
|<span data-ttu-id="20bce-209">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="20bce-209">verificationDnsRecords</span></span>|<span data-ttu-id="20bce-210">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20bce-210">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="20bce-211">客户可以使用 Azure AD 完成域所有权验证之前，客户添加到域 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="20bce-211">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="20bce-212">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="20bce-212">Read-only, Nullable</span></span>|

## <span data-ttu-id="20bce-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20bce-213">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="20bce-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20bce-214">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->