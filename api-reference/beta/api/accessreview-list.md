---
title: 列出 accessReviews
description: 检索 businessFlowTemplate 的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46c9abdbc0a1d5dca4c4e61d423b23ed31691384
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462520"
---
# <a name="list-accessreviews"></a>列出 accessReviews

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索特定[businessFlowTemplate](../resources/businessflowtemplate.md)的[accessReview](../resources/accessreview.md)对象。 返回零个或多个**accessReview**对象的列表, 对于使用该业务流模板创建的每个一次性和定期访问评审。

>[!NOTE]
> 如果与筛选器匹配的任何访问评审是定期访问审核, 则将返回一个**accessReview**对象, 以将每个定期系列表示为一个整体。 例如, 如果每月定期访问 a 组的来宾成员、组 B 的来宾成员的定期访问审核以及组 C 的来宾成员的一次性访问审核, 并且呼叫者查询与业务流的访问审核对组的来宾成员审阅的模板, 将返回三个对象。 若要检索定期访问审核实例或为特定月份或季度计划的访问评审实例, 调用方可以随后导航到定期**accessReview**对象的**实例**关系。 指向当前或过去的定期访问审核实例的**accessReview**对象的**实例**关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview、AccessReview、成员身份、AccessReview。所有  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview、AccessReview、成员身份 |

 登录用户还必须位于允许他们阅读访问审核的目录角色中。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供请求正文。

## <a name="response"></a>响应
如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象的数组。

## <a name="examples"></a>示例
##### <a name="request"></a>请求
下面的示例演示检索业务流模板 "6E4F3D20-C5C3-407F-9695-8460952BCC68" 的所有一次性和定期访问评审的请求。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6E4F3D20-C5C3-407F-9695-8460952BCC68'
```


---


##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [获取 accessReview](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
