---
title: applicationTemplate 资源类型
description: 表示 Azure AD 应用程序库中的应用程序
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 9080a41c1ec4e503e064e406ee4e884654618100
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078978"
---
# <a name="applicationtemplate-resource-type"></a>applicationTemplate 资源类型

命名空间：microsoft.graph

表示 Azure [AD 应用程序库中的应用程序](/azure/active-directory/saas-apps/tutorial-list)。

## <a name="methods"></a>方法

| 方法                                                                       | 返回类型                                                   | 说明                                                                                  |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| [列出 applicationTemplate](../api/applicationtemplate-list.md)               | [applicationTemplate](applicationtemplate.md)                 | 检索 applicationTemplate 对象的列表。                                              |
| [获取 applicationTemplate](../api/applicationtemplate-get.md)                 | [applicationTemplate](applicationtemplate.md)                 | 读取 applicationTemplate 对象的属性和关系。                             |
| [实例化 applicationTemplate](../api/applicationtemplate-instantiate.md) | [applicationServicePrincipal](applicationserviceprincipal.md) | 将 Azure AD 应用程序库中的应用程序实例添加到目录中。 |

## <a name="properties"></a>属性

| 属性                   | 类型              | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| categories                 | String collection | 应用程序的类别列表。 支持的值可以是：、 `Collaboration` `Business Management` `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` 和 `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools` `Travel` `Web design & hosting` 。 |
| 说明                | String            | 应用程序的说明。                                                                                                                                                                                                                                                                                                                                                                                                               |
| displayName                | String            | 应用程序名。                                                                                                                                                                                                                                                                                                                                                                                                                    |
| homePageUrl                | String            | 应用程序的主页 URL。                                                                                                                                                                                                                                                                                                                                                                                                           |
| id                         | String            | 应用程序的唯一标识符。 只读。                                                                                                                                                                                                                                                                                                                                                                                               |
| logoUrl                    | String            | 获取此应用程序徽标的 URL。                                                                                                                                                                                                                                                                                                                                                                                                   |
| 发布者                  | String            | 此应用程序的发布者的名称。                                                                                                                                                                                                                                                                                                                                                                                                 |
| supportedProvisioningTypes | 字符串集合 | 此应用程序支持的预配模式列表。 唯一有效的值为 `sync` 。                                                                                                                                                                                                                                                                                                                                                   |
| supportedSingleSignOnModes | String collection | 此应用程序支持的单一登录模式列表。 支持的值是：`oidc`、`password`、`saml` 和 `notSupported`。                                                                                                                                                                                                                                                                                                            |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "keyProperty": "id"
}-->

```json
{
  "id": "id-value",
  "displayName": "displayName-value",
  "homePageUrl": "homePageUrl-value",
  "supportedSingleSignOnModes": ["supportedSingleSignOnModes-value"],
  "logoUrl": "logoUrl-value",
  "categories": ["categories-value"],
  "publisher": "publisher-value",
  "description": "description-value"
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
