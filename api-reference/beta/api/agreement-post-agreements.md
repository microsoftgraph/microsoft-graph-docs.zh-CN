---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514423"
---
# <a name="create-agreement"></a>创建协议

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的[协议](../resources/agreement.md)对象。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Agreement.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | 字符串 | 持有者令牌 必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。

下表显示创建用户时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|协议中的显示名称。|
|isViewingBeforeAcceptanceRequired|Boolean|指示用户是否能够展开和查看接受之前协议。|
|文件/文件名|String|协议文件 (例如，TOU.pdf) 的名称。|
|文件/isDefault|Boolean|指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。 如果没有文件被标记为默认，第一个将被视为默认。|
|文件/语言|String|区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。 languagecode2 是小写字母双字母代码派生自 ISO 639-1。 国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。|
|文件/fileData/数据|Binary|代表使用条款 PDF 文档的数据。|

## <a name="response"></a>响应
如果成功，此方法返回`201, Created`响应正文中的响应代码和[协议](../resources/agreement.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
