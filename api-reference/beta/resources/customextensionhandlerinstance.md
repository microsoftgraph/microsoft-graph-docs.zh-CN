---
title: customExtensionHandlerInstance 资源类型
description: 用于记录在访问包分配请求上运行的自定义工作流扩展实例的状态。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d832ca092404eb3221952b0b46b720d8f0c217cc
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338298"
---
# <a name="customextensionhandlerinstance-resource-type"></a>customExtensionHandlerInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于记录对访问  [包分配](customaccesspackageworkflowextension.md) 请求运行的自定义工作流扩展 [实例的状态](accesspackageassignmentrequest.md)。

## <a name="methods"></a>方法
无

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|customExtensionId|String|在此实例中触发的 [customAccessPackageWorkflowExtension](customaccesspackageworkflowextension.md) 的标识符。|
|externalCorrelationId|String|逻辑应用的唯一运行 ID。|
|stage|accessPackageCustomExtensionStage|指示访问包自定义扩展运行时请求工作流的阶段。 可取值包括：`assignmentRequestCreated`、`assignmentRequestApproved`、`assignmentRequestGranted`、`assignmentRequestRemoved`、`assignmentFourteenDaysBeforeExpiration`、`assignmentOneDayBeforeExpiration`、`unknownFutureValue`。|
|状态|accessPackageCustomExtensionHandlerStatus|运行与逻辑应用关联的访问包自定义扩展工作流的请求的状态。 可能的值包括 `requestSent`、`requestReceived`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionHandlerInstance"
}
-->
``` json

{
  "@odata.type": "#microsoft.graph.customExtensionHandlerInstance",
  "stage": "String",
  "customExtensionId": "String",
  "externalCorrelationId": "String",
  "status": "String"
}
```

