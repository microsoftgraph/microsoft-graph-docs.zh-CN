---
title: userFlowLanguagePage 资源类型
description: 使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 25fb1c94db9443ed67a0555d09f3859e666bed19
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155466"
---
# <a name="userflowlanguagepage-resource-type"></a>userFlowLanguagePage 资源类型

命名空间：microsoft.graph

使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。 这些语言页面包括 Microsoft 提供的默认语言翻译或可创建自定义页面以自定义语言翻译。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|检索默认或自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 的值。|
|[更新 userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|更新自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 中的值。|
|[删除 userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|无|从自定义 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中删除值。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|userFlowLanguage 页的标识符。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
