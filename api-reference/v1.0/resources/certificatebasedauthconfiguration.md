---
title: certificateBasedAuthConfiguration 资源类型
description: 表示证书颁发机构的集合。
ms.localizationpriority: medium
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 53e56f78508131e3a08e7896095a7f986346fba2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104255"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>certificateBasedAuthConfiguration 资源类型

命名空间：microsoft.graph

使用基于证书的身份验证，Azure Active Directory在 Windows、Android 或 iOS 设备上使用客户端证书进行身份验证，Exchange Online帐户连接到：

- Microsoft 移动应用程序，如 Outlook 和 Word
- Exchange ActiveSync (EAS) 客户端

通过配置此功能，无需在移动设备上的某些邮件Microsoft Office输入用户名和密码组合。

基于证书的身份验证配置通过一组证书颁发机构提供。 证书颁发机构用于建立受信任的证书链，该链使客户端Azure Active Directory客户端证书进行身份验证。

详细了解在 Azure Active Directory 中[基于证书Azure Active Directory。](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-list.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 列出 **certificateBasedAuthConfiguration 集合** 的属性。 |
| [创建 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 创建新的 **certificateBasedAuthConfiguration** 对象。 |
| [获取 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md) | [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) | 读取 **certificateBasedAuthConfiguration 对象** 的属性。 |
| [删除 certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-delete.md) | 无 | 删除 **certificateBasedAuthConfiguration** 对象。 |

>[!NOTE]
>不支持 **更新 certificateBasedAuthConfiguration。** 若要更改 **certificateBasedAuthConfiguration，** 首先删除 ，然后创建新的 **certificateBasedAuthConfiguration**。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|certificateAuthorities|[certificateAuthority](certificateauthority.md) 集合|创建受信任证书链的证书颁发机构的集合。|
|id|String|基于证书的身份验证配置的唯一标识符。 只读。|

## <a name="relationships"></a>关系

无、

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
