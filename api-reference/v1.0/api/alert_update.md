# <a name="update-alert"></a>更新通知

更新任何集成的解决方案内的可编辑** 通知**属性，使通知状态和分配在解决方案之间保持同步。 此方法将更新具有引用的通知 ID 记录的任何解决方案。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |   SecurityEvents.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

> **注意：** 你必须随此方法一起包括**通知** ID 作为参数，并包括其中包含 `provider` 和 `vendor` 的 vendorInformation。
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。必需。|
|Prefer | return=representation |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段值的 JSON 表示形式。 正文**必须**包含 `vendorInformation` 属性及有效的`provider` 和 `vendor` 字段。 下表列出了可为通知更新的字段。 未包括在请求正文中的现有属性的值不会更改。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|assignedTo|字符串|将通知分配给其进行会审、调查或修复的分析师的姓名。|
|closedDateTime|DateTimeOffset|通知关闭的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|comments|字符串集合|分析师对通知的评论（用于客户通知管理）。|
|反馈|alertFeedback|分析师对通知的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|status|alertStatus|通知生命周期状态（阶段）。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。|
|tags|字符串集合|可应用于通知并可充当筛选条件的用户可定义标签（例如，“HVA”、“SAW”）|
|vendorInformation *|[securityVendorInformation](../resources/securityvendorinformation.md)|包含安全产品/服务提供商、供应商和次级供应商相关详细信息的复杂类型（例如，vendor=Microsoft；provider=Windows Defender ATP；subProvider=AppLocker）。 **供应商和提供商字段为必填。**|
（\* 表示必填字段。）

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选请求标头，则该方法返回 `200 OK` 响应代码和响应正文中的更新的[通知](../resources/alert.md)对象。

## <a name="example-1"></a>示例 1

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>响应

下面展示了一个成功的响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>示例 2

### <a name="request"></a>请求

下面的示例展示一个包括 `Prefer` 请求标头的请求。

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>响应

下面展示了使用可选 `Prefer: return=representation` 请求标头时的请求示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
