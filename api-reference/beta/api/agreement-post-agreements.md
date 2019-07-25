---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
ms.openlocfilehash: a9f0dd682ca09ea9723409193447c07f845e27da
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855454"
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
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中, 提供[协议](../resources/agreement.md)对象的 JSON 表示形式。

下表显示创建用户时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|协议的显示名称。|
|isViewingBeforeAcceptanceRequired|Boolean|指示用户是否必须在接受前展开并查看协议。|
|files/fileName|String|协议文件的名称 (例如, TOU)。|
|files/isDefault|Boolean|指示是否为默认协议文件 (如果没有任何区域性与客户端首选项匹配)。 如果没有任何文件被标记为默认值, 则第一项将被视为默认值。|
|文件/语言|String|协议文件的区域性 (格式为 languagecode2/regioncode2)。 languagecode2 是从 ISO 639-1 派生的一个由两个小写字母组成的代码。 国家/regioncode2 派生自 ISO 3166, 通常包含两个大写字母或一个 BCP-47 语言标记 (例如 en-us)。|
|files/fileData/data|Binary|表示使用 PDF 文档的术语的数据。|

## <a name="response"></a>响应
如果成功, 此方法在响应`201, Created`正文中返回响应代码和[协议](../resources/agreement.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中, 提供[协议](../resources/agreement.md)对象的 JSON 表示形式。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
  ]
}
-->
