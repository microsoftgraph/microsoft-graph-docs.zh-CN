# <a name="alert-resource-type"></a>警报资源类型

表示 Microsoft 或合作伙伴安全解决方案确定的客户租户中可能存在的安全问题。 使用警报以统一并简化所有集成解决方案的安全问题管理。 详细信息请参阅 [Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer)中的示例查询。

警报可从以下提供程序中检索： Azure 安全中心和 Azure Active Directory Identity Protection。 其他警报提供程序将在今后几个月内集成。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[获取警报](../api/alert_get.md) | [警报](alert.md) |读取警报对象的属性和关系。|
|[更新警报](../api/alert_update.md) | [警报](alert.md) |更新警报对象。 |
|[列出警报](../api/alert_list.md) | [警报](alert.md)集合 |获取警报对象集合。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|activityGroupName|字符串|此警报所属活动组 （攻击者）的名称或别名。|
|assignedTo|字符串|对指定警报实施会审、调查或修正 （支持 [更新](../api/alert_update.md)）的分析师的姓名。|
|azureSubscriptionId|字符串|Azure 订阅 ID，如果此警报与某一 Azure 资源相关，则显示。|
|azureTenantId *|字符串|Azure Active Directory 租户 ID。|
|类型|字符串|警报类别（例如 credentialTheft、勒索软件等）。|
|closedDateTime|DateTimeOffset|closedDateTime 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014年1月1日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'` （支持 [更新](../api/alert_update.md)）。|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md) 集合|由提供程序生成的安全相关有状态信息，与此警报相关的云应用程序有关。|
|评论|字符串集合|客户对于警报的评论（用于客户警报管理）（支持[更新](../api/alert_update.md)）。|
|置信度|Int32|检测逻辑 （百分比介于 1-100 之间） 的置信度。|
|createdDateTime *|DateTimeOffset|警报提供程序创建警报的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014年1月1日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|说明|字符串|警报说明。|
|detectionIds|字符串集合|此警报实体相关的一组警报 （每一警报均作为单独记录推送至 SIEM）。|
|eventDateTime*|DateTimeOffset|作为触发器生成警报的事件发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014年1月1日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|反馈|alertFeedback|分析师对警报的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。 （支持 [更新](../api/alert_update.md)）|
|fileStates|[fileSecurityState](filesecuritystate.md) 集合|由提供程序生成的安全相关有状态信息，与此警报相关的文件有关。|
|hostStates|[hostSecurityState](hostsecuritystate.md) 集合|由提供程序生成的安全相关有状态信息，与此警报相关的主机有关。|
|id *|字符串|提供程序生成的 GUID/唯一标识符。 （只读）|
|lastModifiedDateTime|DateTimeOffset|警报实体上次修改时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014年1月1日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|malwareStates|[malwareState](malwarestate.md) 集合|有关此警报相关恶意软件的威胁智能。|
|networkConnections|[networkConnection](networkconnection.md) 集合|由提供程序生成的安全相关有状态信息，与此警报相关的网络连接有关。|
|流程|[流程](process.md)集合|由提供程序生成的安全相关有状态信息，与此警报相关的一个或多个流程有关。|
|recommendedActions|字符串集合|供应商/提供程序因警报而建议实施的操作（例如隔离设备、enforce2FA、重置主机映像）。|
|registryKeyStates|[registryKeyState](registrykeystate.md) 集合|由提供程序生成的安全相关有状态信息，与此警报相关的注册表项有关。|
|严重性*|alertSeverity|警报严重性 - 供应商/提供程序设置。 可取值为：`unknown`、`informational`、`low`、`medium`、`high`。|
|sourceMaterials|字符串集合|与警报相关的源资料超链接(URI)，例如，提供程序用于警报或日志搜索等操作的用户界面。|
|状态*|alertStatus|警报生命周期状态（阶段）。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。 （支持 [更新](../api/alert_update.md)）|
|标记|字符串集合|可应用于警报并且可以充当筛选条件的用户可定义标签（例如，“HVA”、“SAW”）（支持 [更新](../api/alert_update.md) ）。|
|标题*|字符串|警报标题。|
|触发器|[alertTrigger](alerttrigger.md) 集合|有关触发警报的特定属性 （出现在警报中的属性）的安全相关信息。 警报可能包含多个用户、主机、文件、ip 地址的信息。 此字段指示哪些属性触发了警报生成。|
|userStates|[userSecurityState](usersecuritystate.md) 集合|由提供程序生成的安全相关有状态信息，与此警报相关的用户帐户有关。|
|vendorInformation *|[securityVendorInformation](securityvendorinformation.md)|包含安全产品/服务供应闪、提供程序和次级提供程序相关详细信息的复杂类型（例如，vendor=Microsoft；provider=Windows Defender ATP；subProvider=AppLocker）。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md) 集合|与一个或多个警报相关安全漏洞有关的威胁智能。|
（\*表示必填字段。）

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->