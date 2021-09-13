---
title: synchronizationJobSubject 资源类型
description: 表示将在按需预配期间设置的对象。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 1f4de7d4c3d518b795d739a80403903842d16a16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090960"
---
# <a name="synchronizationjobsubject-resource-type"></a>synchronizationJobSubject 资源类型

命名空间：microsoft.graph

表示将在按需预配期间设置的对象。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|objectId|String|要应用 synchronizationJob 的对象的标识符。|
|objectTypeName|String|要应用 synchronizationJob 的对象的类型。|

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


