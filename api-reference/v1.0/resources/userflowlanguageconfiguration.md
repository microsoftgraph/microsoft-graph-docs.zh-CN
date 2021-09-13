---
title: userFlowLanguageConfiguration 资源类型
description: 允许用户流支持多种语言。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9af22f309ca7c93043d90ef8c0583686d7cf24f2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136318"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>userFlowLanguageConfiguration 资源类型

命名空间：microsoft.graph

允许用户流来支持多种语言的使用。

For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language)， you can only leverage the built-in languages provided by Microsoft. 用户流Azure Active Directory定义在用户通过用户流配置的旅程时向用户显示的语言和字符串。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。 这些对象表示用户流中可用的语言。|
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
|overridesPages|[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合|包含替代消息的页面集合，这些消息显示在指定语言的用户流中。 此集合仅允许修改页面内容，不允许对页面 (或删除页面进行任何其他) 。|

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
