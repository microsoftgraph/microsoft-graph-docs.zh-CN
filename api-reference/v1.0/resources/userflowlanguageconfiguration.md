---
title: userFlowLanguageConfiguration 资源类型
description: 允许用户流支持多种语言。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a3291309537ea914587e0491f9340bb626e88a68
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882942"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>userFlowLanguageConfiguration 资源类型

命名空间：microsoft.graph

允许用户流来支持多种语言的使用。

对于 [Azure Active Directory 用户流](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)，只能利用 Microsoft 提供的内置语言。 Azure Active Directory 的用户流支持定义在用户通过用户流配置的旅程时向用户显示的语言和字符串。

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
