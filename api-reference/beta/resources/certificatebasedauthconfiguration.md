---
title: certificateBasedAuthConfiguration 资源类型
description: 表示证书颁发机构的集合。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76178d8d70225a8cf861f5ff5e1cdaf7f0f69f60
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667627"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>certificateBasedAuthConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过基于证书的身份验证, 您可以在将 Exchange Online 帐户连接到以下各项时, 使用 Windows、Android 或 iOS 设备上的客户端证书对 Azure Active Directory 进行身份验证:

- Microsoft 移动应用程序 (如 Outlook 和 Word)
- Exchange ActiveSync (EAS) 客户端

配置此功能后, 无需在移动设备上将用户名和密码组合输入到某些邮件和 Microsoft Office 应用程序中。

基于证书的身份验证配置是通过证书颁发机构的集合提供的。 证书颁发机构用于建立受信任的证书链, 使客户端能够通过具有客户端证书的 Azure Active Directory 进行身份验证。

了解有关[Azure Active Directory 中基于证书的身份验证的](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)详细信息。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-list.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 列出**certificateBasedAuthConfiguration**集合的属性。 |
| [获取 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 读取**certificateBasedAuthConfiguration**对象的属性。 |
| [创建 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 创建新的**certificateBasedAuthConfiguration**对象。 |
| [删除 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md) | 无 | 删除**certificateBasedAuthConfiguration**对象。 |

>[!NOTE]
>不支持更新 cerficateBasedAuthConfiguration。 若要更改 cerficateBasedAuthConfiguration, 请先删除, 然后创建一个新的 cerficateBasedAuthConfiguration。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|certificateAuthorities|[certificateAuthority](certificateauthority.md)集合|创建受信任的证书链的证书颁发机构的集合。|
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
  "baseType": "",
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
