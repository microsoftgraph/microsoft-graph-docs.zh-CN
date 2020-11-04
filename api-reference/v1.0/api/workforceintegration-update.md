---
title: 更新 workforceIntegration
description: 更新 workforceIntegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ff45c62726c5efc986593e3e949ffacdb115a15
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849079"
---
# <a name="update-workforceintegration"></a>更新 workforceIntegration

命名空间：microsoft.graph

更新 [workforceIntegration](../resources/workforceintegration.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | WorkforceIntegration |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

> **注意** ：此 API 支持管理员权限。 全局管理员可以访问他们不是其成员的组。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|apiVersion|Int32|回调 URL 的 API 版本。 从1开始。|
|displayName|String|劳动力集成的名称。|
|技术|workforceIntegrationEncryption|劳动力集成加密资源。 |
|isActive|Boolean|指示此劳动力集成当前是否处于活动状态且可用。|
|supportedEntities|string| 可取值为：`none`、`shift`、`swapRequest`、`openshift`、`openShiftRequest`、`userShiftPreferences`。 如果选择多个值，则所有值必须以大写形式的第一个字母开头。|
|url|String| 劳动力集成 URL，用于从班次服务进行回调。 |

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workforceIntegration](../resources/workforceintegration.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supportedEntities": "supportedEntities-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supportedEntities": "supportedEntities-value"
}
```

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a>WorkforceIntegration 实体的示例用例用于按 WFM 规则资格进行筛选

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a>用例：替换现有的 WorkforceIntegration 以启用 SwapRequest 的资格筛选

### <a name="request"></a>请求

下面展示了示例请求。 
```
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationid}
{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    - "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}
```
### <a name="response"></a>响应

下面展示了示例响应。
```
HTTP/1.1 200 OK
Content-type: application/json
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}
```
若要了解如何创建具有 SwapRequest 的新 workforceintegration 以启用资格筛选，请参阅 [create](../api/workforceintegration-post.md)。

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a>EligibilityFilteringEnabledEntities 中包含 SwapRequest 时获取符合条件的班次的示例
倒班应用和劳动力集成终结点之间的交互将遵循现有模式。

### <a name="request"></a>请求

下面的示例演示了如何通过转到劳动力集成终结点来获取交换请求的符合条件的请求。

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us
{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
### <a name="response"></a>响应

以下是劳动力集成服务响应的示例。
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

