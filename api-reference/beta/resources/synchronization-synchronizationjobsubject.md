---
title: synchronizationJobSubject 资源类型
description: 表示将在按需预配期间预配的对象。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c9e6d83ed7024556954740e89edcc18f7b56ba04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131996"
---
# <a name="synchronizationjobsubject-resource-type"></a>synchronizationJobSubject 资源类型

命名空间：microsoft.graph

表示将在按需预配期间预配的对象。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|objectId|String|要应用 synchronizationJob 的对象的标识符。|
|objectTypeName|字符串|要应用 synchronizationJob 的对象的类型。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String"
}
```


