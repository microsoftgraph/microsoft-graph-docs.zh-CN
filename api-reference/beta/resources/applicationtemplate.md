---
title: applicationTemplate 资源类型
description: 表示 Azure AD 应用程序库中的应用程序
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c34c083a4cfee63db724228d9390c7452ca5a92
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870944"
---
# <a name="applicationtemplate-resource-type"></a>applicationTemplate 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[AZURE AD 应用程序库](/azure/active-directory/saas-apps/tutorial-list)中的应用程序。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[列出 applicationTemplate](../api/applicationtemplate-list.md)|[applicationTemplate](applicationtemplate.md)|检索 applicationTemplate 对象的列表。|
| [获取 applicationTemplate](../api/applicationtemplate-get.md) | [applicationTemplate](applicationtemplate.md) | 读取 applicationTemplate 对象的属性和关系。 |
|[实例化 applicationTemplate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](applicationserviceprincipal.md)| 将 Azure AD 应用程序库中的应用程序实例添加到目录中。|


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|categories|String collection|应用程序的类别列表。 受支持的值可以`Collaboration`是`Business Management`： `Consumer`、`Content management`、 `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Web design & hosting`、、、、、、、、、、、、、、、、、、、、和。 `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel`|
|description|String|应用程序的说明。|
|displayName|字符串|应用程序名。|
|homePageUrl|String|应用程序的主页 URL。|
|id|字符串| 应用程序的唯一标识符。 只读。|
|logoUrl|String|用于获取此应用程序徽标的 URL。|
|发布者|String|此应用程序的发布者的名称。|
|supportedProvisioningTypes|String collection|此应用程序支持的预配模式的列表。 唯一有效的值为`sync`。|
|supportedSingleSignOnModes|String collection|此应用程序支持的单一登录模式列表。 受支持的值`password`为`saml`、 `external`、和`oidc`。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
