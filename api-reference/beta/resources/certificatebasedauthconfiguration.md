---
title: certificateBasedAuthConfiguration 资源类型
description: 表示证书颁发机构的集合。
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1ff4eb3e7a235a27dc9d58b9b4bd631d0aeaed0f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443144"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>certificateBasedAuthConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过基于证书的身份验证，可以在将 Exchange Online 帐户连接到 Windows、Android 或 iOS 设备上的客户端证书后，通过 Azure Active Directory 进行身份验证：

- Microsoft 移动应用程序，如 Outlook 和 Word
- Exchange ActiveSync (EAS) 客户端

配置此功能后，无需在移动设备上的某些邮件和Microsoft Office输入用户名和密码组合。

基于证书的身份验证配置通过证书颁发机构集合提供。 证书颁发机构用于建立受信任的证书链，使客户端可以通过 Azure Active Directory 使用客户端证书进行身份验证。

了解有关 Azure [Active Directory 中基于证书的身份验证的信息](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-list.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 列出 **certificateBasedAuthConfiguration 集合** 的属性。 |
| [获取 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 读取 **certificateBasedAuthConfiguration 对象** 的属性。 |
| [创建 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 创建新的 **certificateBasedAuthConfiguration** 对象。 |
| [删除 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md) | 无 | 删除 **certificateBasedAuthConfiguration** 对象。 |

>[!NOTE]
>不支持更新 cerficateBasedAuthConfiguration。 若要更改 cerficateBasedAuthConfiguration，请首先删除并创建新的 cerficateBasedAuthConfiguration。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|certificateAuthorities|[certificateAuthority](certificateauthority.md) 集合|创建受信任证书链的证书颁发机构的集合。|
|id|String|基于证书的身份验证配置的唯一标识符。 只读。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
