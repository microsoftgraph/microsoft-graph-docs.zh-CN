---
title: userFlowLanguageConfiguration 资源类型
description: userFlowsLanguageConfiguration 对象允许用户流支持多种语言的自定义。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aa83d85725cbef54229cdc92246fb83888697166
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547146"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>userFlowLanguageConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户流语言自定义功能允许给定用户流支持多种语言的自定义，从所有内置语言到自定义语言。

For [Azure Active Directory B2C user flows](/azure/active-directory-b2c/user-flow-language-customization#supported-languages)， you can leverage the built-in languages or provide the language customizations for a language that is currently not built-in by default. For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language)， you can only leverage the built-in languages provided by Microsoft. B2C 和 Azure Active Directory 和 Azure Active Directory 用户流都支持自定义当用户通过用户流配置的旅程时向用户显示的语言和字符串。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。 这些对象表示用户流中可用的语言。|
|[删除 userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|无|删除自定义 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。 这些对象表示用户流中可用的语言，只有自定义语言可以从 Azure AD B2C 用户流中删除。|
|[列出 defaultPages](../api/userflowlanguageconfiguration-list-defaultpages.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|从 defaultPages 导航属性获取 userFlowLanguagePage 资源。 表示用户流中的默认用户旅程。|
|[List overridesPages](../api/userflowlanguageconfiguration-list-overridespages.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|从 overridesPages 导航属性获取 userFlowLanguagePage 资源。 表示用户流中的用户旅程的自定义体验。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|语言的标识符。 此字段与语言 ID 标记 [RFC 5646](https://tools.ietf.org/html/rfc5646) 兼容，并且必须是记录的语言 ID。|
|isEnabled|Boolean|指示语言是否在用户流中启用。|
|displayName|String|要显示的语言名称。 此属性是只读的。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|defaultPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含要以指定语言的用户流显示的默认内容的页面集合。 此集合不允许任何类型的修改。|
|overridesPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含覆盖消息的页面集合，这些消息显示在指定语言的用户流中。 此集合仅允许修改页面的内容，不允许在页面创建 (删除页面时进行任何其他) 。|

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
