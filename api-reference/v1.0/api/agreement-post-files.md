---
title: 创建 agreementFileLocalization
description: 创建新的本地化协议文件。
author: raprakasMSFT
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 71f5568c369e1642ac3725fcc34612de5a8c1d30
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315102"
---
# <a name="create-agreementfilelocalization"></a>创建 agreementFileLocalization
命名空间：microsoft.graph

创建新的本地化协议文件。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Agreement.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /agreements/{agreementsId}/files
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [agreementFileLocalization](../resources/agreementfilelocalization.md) 对象的 JSON 表示形式。

创建 **agreementFileLocalization** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|协议策略文件的本地化显示名称。 本地化显示名称将显示给查看协议的最终用户。|
|fileData|[agreementFileData](../resources/agreementfiledata.md)|表示使用条款 PDF 文档的数据。|
|fileName|String|例如，协议文件的名称 (TOU.pdf) 。 |
|isDefault|Boolean|如果没有语言与客户端首选项匹配，则指示这是否是默认协议文件。 如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。 只读。|
|isMajorVersion|Boolean|指示协议文件是否为主要版本更新。 主要版本更新使协议对相应语言的接受无效。|
|language|String|协议文件的语言，格式为“languagecode2-country/regioncode2”。 “languagecode2”是派生自 ISO 639-1 的小写双字母代码，而“country/regioncode2”派生自 ISO 3166，通常由两个大写字母或 BCP-47 语言标记组成。 例如，美国英语是 `en-US`.|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [agreementFileLocalization](../resources/agreementfilelocalization.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_agreementfilelocalization_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/files
Content-Type: application/json

{
    "fileName": "Contoso ToU for guest users (French)",
    "language": "fr-FR",
    "isDefault": false,
    "isMajorVersion": false,
    "displayName": "Contoso ToU for guest users (French)",
    "fileData": {
        "data": "base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data"
    }
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/termsOfUse/agreements('94410bbf-3d3e-4683-8149-f034e55c39dd')/files/$entity",
    "id": "90d1723c-52c1-40e3-a51a-da99a82c0327",
    "fileName": "Contoso ToU for guest users (French)",
    "displayName": "Contoso ToU for guest users (French)",
    "language": "fr-FR",
    "isDefault": false,
    "isMajorVersion": false,
    "createdDateTime": "2022-03-04T14:38:22.8292386Z",
    "fileData": {
        "data": "base64JVBERi0xLjUKJb/"
    }
}
```
