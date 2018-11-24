# <a name="alert-resource-type"></a>警报的资源类型

表示 Microsoft 或合作伙伴的安全解决方案具有标识的客户的租户中潜在的安全问题。 使用通知统一和简化安全问题管理跨所有集成的解决方案。 若要了解详细信息，请参阅[图资源管理器](https://developer.microsoft.com/graph/graph-explorer)中的示例查询。

可以从[Microsoft Graph 安全概述 （英文)](security-api-overview.md)中列出的不同的安全提供程序中检索通知。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[获取警报](../api/alert_get.md) | [通知](alert.md) |读取属性和警报对象的关系。|
|[更新警报](../api/alert_update.md) | [通知](alert.md) |更新警报对象。 |
|[列出警报](../api/alert_list.md) | [通知](alert.md)集合 |获取通知对象集合。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|activityGroupName|字符串|名称或别名活动组 （攻击） 的此警报归功于。|
|assignedTo|字符串|分析师通知的名称分配给进行会审、 调查或修复 （支持[更新](../api/alert_update.md)）。|
|azureSubscriptionId|字符串|Azure 订阅 ID，此警报与 Azure 资源如果存在此参数。|
|azureTenantId |字符串|Azure Active Directory 租户 id。 必需。|
|category|String|警报 （例如，credentialTheft、 勒索软件等） 的类别。|
|closedDateTime|DateTimeOffset|通知关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，在 2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'` （支持[更新](../api/alert_update.md)）。|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md)集合|有关与通知相关的云应用程序/s 提供程序生成的与安全相关的状态信息。|
|comments|String 集合|通知 （用于客户警报管理） 的客户提供评论 （支持[更新](../api/alert_update.md)）。|
|confidence|Int32|检测逻辑 （1-100 之间的百分比） 的信心。|
|createdDateTime |DateTimeOffset|警报的提供程序中由通知的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 必需。|
|说明|字符串|警报的说明。|
|detectionIds|String 集合|通知 （每个通知推送到作为单独的记录 SIEM） 与此警报实体集。|
|eventDateTime |DateTimeOffset|担任生成通知的触发器事件发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 必需。|
|反馈|alertFeedback|分析师通知上的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。 （支持[更新](../api/alert_update.md)）|
|fileStates|[fileSecurityState](filesecuritystate.md)集合|有关与通知相关的文件提供程序生成的与安全相关的状态信息。|
|hostStates|[hostSecurityState](hostsecuritystate.md)集合|有关与此警报主机提供程序生成的与安全相关的状态信息。|
|id |字符串|提供程序生成的 GUID/唯一标识符。 只读。 必需。|
|lastModifiedDateTime|DateTimeOffset|警报的实体的上次修改时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|malwareStates|[malwareState](malwarestate.md)集合|与此警报与相关的恶意软件的威胁智能。|
|networkConnections|[networkConnection](networkconnection.md)集合|有关与通知相关的网络连接提供程序生成的与安全相关的状态信息。|
|流程|[过程](process.md)集合|有关或多个进程与此警报提供程序生成的与安全相关的状态信息。|
|recommendedActions|String 集合|供应商/提供程序建议操作才能由于通知 （例如，隔离计算机、 enforce2FA、 重新映像主机）。|
|registryKeyStates|[registryKeyState](registrykeystate.md)集合|与此通知相关的注册表项有关提供程序生成的与安全相关的状态信息。|
|严重级别 |alertSeverity|警报严重性-供应商/服务提供商设置。 可取值为：`unknown`、`informational`、`low`、`medium`、`high`。 必需。|
|sourceMaterials|String 集合|超链接 (Uri) 的源材料相关对通知，例如，通知或日志搜索等的提供商的用户界面。|
|状态 |alertStatus|警报生命周期状态 （阶段）。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。 （支持[更新](../api/alert_update.md)）。 必需。|
|标记前添加的标记|String 集合|用户可定义标签可以应用于通知和可以充当筛选条件 （例如"HVA"、"是"等。）（支持[更新](../api/alert_update.md)）。|
|title |字符串|通知的标题。 必需。|
|触发器|[alertTrigger](alerttrigger.md)集合|有关触发通知 （出现在通知中的属性） 的特定属性与安全相关的信息。 通知可能包含多个用户、 主机、 文件、 ip 地址的信息。 此字段指示哪些属性触发警报生成。|
|userStates|[userSecurityState](usersecuritystate.md)集合|与此通知相关的用户帐户提供程序生成的与安全相关的状态信息。|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|包含有关安全产品/服务供应商、 提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。 必需。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md)集合|与一个或多个与通知相关的安全漏洞的威胁智能。|

## <a name="relationships"></a>Relationships

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