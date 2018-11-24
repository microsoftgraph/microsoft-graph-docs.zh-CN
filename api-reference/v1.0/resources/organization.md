# <a name="organization-resource-type"></a>组织资源类型

表示 Azure Active Directory 租户。只支持在租户上执行读取和更新操作；不支持创建和删除操作。继承自 [directoryObject](directoryobject.md)。

通过该资源可以使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取组织](../api/organization_get.md) | [组织](organization.md) |读取 organization 对象的属性和关系。|
|[更新](../api/organization_update.md) | [组织](organization.md)  |更新 organization 对象。 可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。 |
|**开放扩展**| 
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| 
|[添加架构扩展值](../../../concepts/extensibility_schema_groups.md) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性

| 属性                             | 类型                                                              | 说明                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | [assignedPlan](assignedplan.md) 集合                        | 与租户相关的服务计划的集合。不可为 null。                                                                                                                                                                                                            |
| 城市                                 | String                                                            | 组织地址所在的城市名称。                                                                                                                                                                                                                                        |
| companyLastDirSyncTime               | DateTimeOffset                                                    | 租户最后一次与本地目录同步的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'` |
| country                              | 字符串                                                            | 组织地址所在的国家/地区名称。                                                                                                                                                                                                                              |
| countryLetterCode                    | 字符串                                                            | 组织所在的国家/地区缩写                                                                                                                                                                                                                                     |
| deletionTimestamp                    | DateTimeOffset                                                    | 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`                                                                                     |
| dirSyncEnabled                       | Boolean                                                           | 如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。                        |
| displayName                          | String                                                            | 租户的显示名称。                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | 租户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。                                                                                                                                                            |
|isMultipleDataLocationsForServicesEnabled|布尔|**true**如果组织已启用，则多地理位置**false**如果组织不是多地理位置启用则**null**（默认值）。 只读。 有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。|
| marketingNotificationEmails          | String collection                                                 | 不可为 null。                                                                                                                                                                                                                                                                        |
| objectType                           | String                                                            | 一个标识对象类型的字符串。对于租户，该值始终为“Company”。                                                                                                                                                                                                 |
| postalCode                           | String                                                            | 组织地址的邮政编码。                                                                                                                                                                                                                                      |
| preferredLanguage                    | String                                                            | 组织的首选语言。 应遵循 ISO 639-1 代码；例如“en”。                                                                                                                                                                                         |
| privacyProfile                       | [privacyProfile](privacyprofile.md)                               | 组织的隐私配置文件。                                                                                                                                                                                                                                              |
| provisionedPlans                     | [ProvisionedPlan](provisionedplan.md) 集合                  | 不可为 null。                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | String                                                            | 组织地址所在的省/自治区/直辖市名称。                                                                                                                                                                                                                                       |
| street                               | String                                                            | 组织地址所在的街道名称。                                                                                                                                                                                                                                          |
| technicalNotificationMails           | String collection                                                 | 不可为 null。                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | String                                                            | 组织的电话号码                                                                                                                                                                                                                                                |
| verifiedDomains                      | [VerifiedDomain](verifieddomain.md) 集合                    | 与该租户相关联的域集合。不可为 null。                                                                                                                                                                                                                 |

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为组织定义的开放扩展集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "companyLastDirSyncTime": "2018-05-12T13:09:20.111Z",
  "country": "string",
  "countryLetterCode": "string",
  "deletionTimestamp": "2018-05-12T15:37:52.763Z",
  "dirSyncEnabled": true,
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "objectType": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "telephoneNumber": "555-555-6568",
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
