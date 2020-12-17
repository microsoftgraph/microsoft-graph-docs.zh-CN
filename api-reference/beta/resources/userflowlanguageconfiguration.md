---
title: userFlowLanguageConfiguration 资源类型
description: userFlowsLanguageConfiguration 对象允许用户流支持多种语言的自定义。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 69a32fbb3ec84928c9e4112134b6d771ca3149f4
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706298"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>userFlowLanguageConfiguration 资源类型

命名空间：microsoft.graph

用户流语言自定义是允许给定用户流支持多种语言（从所有内置语言到自定义语言）的自定义的功能。

对于 [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages)用户流，可以利用内置语言或为当前未默认内置语言提供语言自定义。 对于 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)用户流，只能利用 Microsoft 提供的内置语言。 Azure Active Directory B2C 和 Azure Active Directory 的用户流都支持在用户完成使用用户流配置的旅程时自定义向用户显示的语言和字符串。

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
|id|字符串|语言的标识符。 此字段符合语言 ID 标记 [RFC 5646，](https://tools.ietf.org/html/rfc5646) 并且必须是记录的语言 ID。|
|isEnabled|Boolean|指示是否在用户流中启用语言。|
|displayName|字符串|要显示的语言名称。 此属性是只读的。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|defaultPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含默认内容的页面集合，这些页面显示在指定语言的用户流中。 此集合不允许任何类型的修改。|
|overridesPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含替代消息的页面集合，这些邮件显示在指定语言的用户流中。 此集合仅允许修改页面内容，不允许任何其他修改 (或删除页面) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "baseType": "",
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
