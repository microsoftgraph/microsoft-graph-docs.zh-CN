---
title: userFlowLanguageConfiguration 资源类型
description: userFlowsLanguageConfiguration 对象允许用户流支持多语言自定义。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 77e1bfe5bacac97f043c6044ea1d878eab2f1bad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442640"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>userFlowLanguageConfiguration 资源类型

命名空间：microsoft.graph

用户流语言自定义是一项允许给定用户流支持多种语言（从所有内置语言到自定义语言）的自定义的功能。

对于 [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages)用户流，可以利用内置语言或为默认情况下未内置语言提供语言自定义。 对于 [Azure Active Directory 用户流](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)，只能利用 Microsoft 提供的内置语言。 Azure Active Directory B2C 和 Azure Active Directory 的用户流都支持在用户完成使用用户流配置的旅程时自定义向用户显示的语言和字符串。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。 这些对象表示用户流中可用的语言。|
|[删除 userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|无|删除自定义 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。 这些对象表示在用户流中可用的语言，并且只有自定义语言可以从 Azure AD B2C 用户流中删除。|
|[列出 defaultPages](../api/userflowlanguageconfiguration-list-defaultpages.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|从 defaultPages 导航属性获取 userFlowLanguagePage 资源。 表示用户流中的默认用户旅程。|
|[List overridesPages](../api/userflowlanguageconfiguration-list-overridespages.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|从 overridesPages 导航属性获取 userFlowLanguagePage 资源。 表示用户流中的用户旅程的自定义体验。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|语言的标识符。 此字段与语言 ID 标记 [RFC 5646](https://tools.ietf.org/html/rfc5646) 兼容，并且必须是已记录的语言 ID。|
|isEnabled|Boolean|指示是否在用户流中启用语言。|
|displayName|String|要显示的语言名称。 此属性是只读的。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|defaultPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含默认内容的页面集合，这些页面以指定语言在用户流中显示。 此集合不允许任何类型的修改。|
|overridesPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含要以指定语言在用户流中显示的邮件的覆盖邮件的页面集合。 此集合仅允许修改页面内容，不允许任何其他修改 (或删除页面) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```
