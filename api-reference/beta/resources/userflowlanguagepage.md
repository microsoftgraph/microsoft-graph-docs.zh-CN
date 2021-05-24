---
title: userFlowLanguagePage 资源类型
description: 使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7a52d1dce81bc24809d788e8d28ef869b84c4704
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629516"
---
# <a name="userflowlanguagepage-resource-type"></a>userFlowLanguagePage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。 这些语言页面包括 Microsoft 提供的默认语言翻译或可创建用于自定义语言翻译的自定义页面。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|检索默认或自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 的值。|
|[更新 userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|更新自定义 [userFlowLanguagePage 对象中的](../resources/userflowlanguagepage.md) 值。|
|[删除 userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|无|从自定义 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中删除值。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|userFlowLanguage 页面的标识符。|

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
