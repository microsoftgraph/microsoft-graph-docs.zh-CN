---
title: 更新工作人员重新参与
description: 更新 workforceintegration 对象的属性。
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6fcfe75b2ee2d39a3142c952d6218da31c8b36df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031218"
---
# <a name="update-workforceintegration"></a>更新工作人员重新参与

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [workforceintegration 对象](../resources/workforceintegration.md) 的属性。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | WorkforceIntegration.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|apiVersion|Int32|用于回叫 URL 的 API 版本。 从 1 开始。|
|displayName|String|员工集成的名称。|
|加密|workforceIntegrationEncryption|员工集成加密资源。 |
|isActive|布尔|指示此员工集成当前是否处于活动状态且可用。|
|支持|string| 可能的值是 `none` `shift` `swapRequest` 、、、、、。 `openshift` `openShiftRequest` `userShiftPreferences` 如果选择多个值，则所有值必须以大写字母开头。|
|supportedEntities|string| 此属性 **将替换** v1.0 中的 supports。 我们建议你使用此属性，而不是 **支持**。 **目前，supports** 属性在 beta 版中仍受支持。 可能的值是 `none` `shift` `swapRequest` 、、、、、。 `openshift` `openShiftRequest` `userShiftPreferences` 如果选择多个值，则所有值必须以大写字母开头。|
|url|String| 来自 Shift 服务的回调的"员工集成"URL。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [workforceIntegration](../resources/workforceintegration.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-update-a-workforceintegration-object"></a>示例 1：更新一个 workforceIntegration 对象

以下示例更新 **一个 workforceIntegration** 对象。

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
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
  "supports": "supports-value"
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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-workforceintegration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

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
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a>示例 2：新建一个针对资格筛选启用 SwapRequest 的 workforceIntegration

以下示例创建一个新的 **workforceIntegration，** 并启用 SwapRequest 进行资格筛选。

#### <a name="request"></a>请求

下面展示了示例请求。 
```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a>响应

下面展示了示例响应。
```
HTTP/1.1 200 OK
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
若要创建新的 **workforceIntegration，** 并启用 SwapRequest 进行资格筛选，请参阅 [Create](../api/workforceintegration-post.md) 方法。

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a>示例 3：在 SwapRequest 包含在 eligiblyFilteringEnabledEntities 中时提取符合条件的班次

班次应用和员工集成终结点之间的交互将遵循现有模式。

#### <a name="request"></a>请求

下面是 Shifts 向员工集成终结点请求获取交换请求的合格班次的示例。

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
#### <a name="response"></a>响应

下面是员工集成服务的响应示例。
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

### <a name="example-4-shifts-synchronous-call-back-to-the-workforce-integration-endpoint-when-enabled-for-real-time-notifications-on-timecard-changes"></a>示例 4：启用 timeCard 更改时实时通知时，将同步调用移回员工集成终结点。

#### <a name="request"></a>请求

下面展示了示例请求。 
```
POST https://foobarWorkforceIntegration.com/foobar/v1/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/update
Accept-Language: en-us
X-MS-WFMPassthrough: foobarvalue
Content-type: application/json
{
   "requests":[
      {
         "id":"1",
         "method":"POST",
         "url":"/timecards",
         "headers":{
            "X-MS-Transaction-ID":"1"
         },
         "body":{
            "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
            "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
            "createdDateTime":"2019-03-18T00:00:00.000Z",
            "createdBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
            "lastModifiedBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "state":"onBreak",
            "clockIn":{
               "dateTime":"2019-03-18T00:00:00.000Z",
               "atApprovedLocation":true,
               "notes":null
            },
            "clockOut":null,
            "breaks":[
               {
                  "id":"string",
                  "notes":{
                     "content":"Lunch break",
                     "contentType":"text"
                  },
                  "start":{
                     "dateTime":"2019-03-18T00:00:00.000Z",
                     "atApprovedLocation":true,
                     "notes":{
                        "content":"Started my break 5 minutes early",
                        "contentType":"text"
                     }
                  },
                  "end":null
               }
            ],
            "notes":null,
            "originalEntry":{
               "clockIn":{
                  "dateTime":"2019-03-18T00:00:00.000Z",
                  "atApprovedLocation":true,
                  "notes":null
               },
               "clockOut":null,
               "breaks":[
                  {
                     "id":"4591109b-a618-3e0d-e6a0-d42b25b7231f",
                     "notes":{
                        "content":"Lunch break",
                        "contentType":"text"
                     },
                     "start":{
                        "dateTime":"2019-03-18T00:00:00.000Z",
                        "atApprovedLocation":true,
                        "notes":{
                           "content":"Started my break 5 minutes early",
                           "contentType":"text"
                        }
                     },
                     "end":null
                  }
               ]
            }
         }
      }
   ]
}

```
#### <a name="response"></a>响应

下面展示了示例响应。
```
HTTP/1.1 200 OK
Content-type: application/json
{
  "responses":[
    {
      "id": "1",
      "status": 200,
      "body":{
        "eTag": "4000ee23-0000-0700-0000-5d1415f60000",
        "error": null
      }
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


