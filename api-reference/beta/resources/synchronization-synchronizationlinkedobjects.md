---
title: synchronizationLinkedObjects 资源类型
description: 表示在按需预配期间要预配的任何引用。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 27053821607e8a813c690e18aa658256c0ff1038
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645612"
---
# <a name="synchronizationlinkedobjects-resource-type"></a>synchronizationLinkedObjects 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在按需预配期间要预配的任何引用。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|成员|[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) 集合|要预配的所有组成员。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationLinkedObjects"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationLinkedObjects",
  "members": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```
