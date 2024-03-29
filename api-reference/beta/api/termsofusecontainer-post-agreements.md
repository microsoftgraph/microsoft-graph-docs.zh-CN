---
title: 创建协议
description: 创建新的协议对象。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 03ac058dd53861502bee64f85e254be53db4ab3a
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451450"
---
# <a name="create-agreement"></a>创建协议

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [协议](../resources/agreement.md) 对象。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Agreement.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

代表用户进行呼叫时，用户需要属于以下目录角色之一。 若要了解有关目录角色Azure AD，请参阅Azure AD[角色](/azure/active-directory/roles/permissions-reference)：
+ 全局管理员
+ 条件访问管理
+ 安全管理员

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供 agreement 对象的 JSON [表示](../resources/agreement.md) 形式。

下表显示创建用户时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串|协议的显示名称。|
|isViewingBeforeAcceptanceRequired|布尔值|指示用户在接受之前是否必须展开和查看协议。|
|files/fileName|字符串|协议文件的名称 (例如，TOU.pdf) 。|
|files/isDefault|布尔值|指示当没有任何区域性与客户端首选项匹配时，这是否是默认协议文件。 如果没有文件标记为默认文件，则第一个文件将被视为默认文件。|
|文件/语言|字符串|格式为 languagecode2-country/regioncode2 的协议文件的区域性。 languagecode2 是从 ISO 639-1 派生的两个字母小写代码。 country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。|
|files/fileData/data|Binary|表示 PDF 文档的使用条款的数据。|

## <a name="response"></a>响应
如果成功，此方法在响应 `201, Created` 正文中返回 [响应](../resources/agreement.md) 代码和 agreement 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
在请求正文中，提供协议对象的 JSON [表示](../resources/agreement.md) 形式。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
Content-type: application/json

{
  "displayName": "Contoso ToU for guest users",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ=//truncated-binary"
      }
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-agreement-from-agreements-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-agreement-from-agreements-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#agreements/$entity",
    "id": "94410bbf-3d3e-4683-8149-f034e55c39dd",
    "displayName": "Contoso ToU for guest users",
    "termsExpiration": null,
    "userReacceptRequiredFrequency": null,
    "isViewingBeforeAcceptanceRequired": true,
    "isPerDeviceAcceptanceRequired": false
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


