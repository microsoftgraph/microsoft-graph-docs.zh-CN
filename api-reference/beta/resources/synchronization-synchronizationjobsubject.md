---
title: synchronizationJobSubject 资源类型
description: 表示将在按需预配期间设置的对象。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c7dea31898cb0bfb521367042401be7c583c60c2868d4805682c9d0e707fc898
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226110"
---
# <a name="synchronizationjobsubject-resource-type"></a>synchronizationJobSubject 资源类型

命名空间：microsoft.graph

表示将在按需预配期间设置的对象。

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


