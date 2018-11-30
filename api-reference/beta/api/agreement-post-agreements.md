---
title: 创建协议
description: 创建新的协议对象。
ms.openlocfilehash: bfcab53b4233d133309c99a4825e184a42670458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042702"
---
# <a name="create-agreement"></a>创建协议

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。

下表显示创建用户时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串|协议中的显示名称。|
|isViewingBeforeAcceptanceRequired|布尔|指示用户是否能够展开和查看接受之前协议。|
|文件/文件名|字符串|协议文件 (例如，TOU.pdf) 的名称。|
|文件/isDefault|布尔|指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。 如果没有文件被标记为默认，第一个将被视为默认。|
|文件/语言|字符串|区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。 languagecode2 是小写字母双字母代码派生自 ISO 639-1。 国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。|
|文件/fileData/数据|二进制数|代表使用条款 PDF 文档的数据。|

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
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
