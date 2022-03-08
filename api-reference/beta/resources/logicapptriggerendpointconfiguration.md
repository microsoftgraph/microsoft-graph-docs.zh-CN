---
title: logicAppTriggerEndpointConfiguration 资源类型
description: 与自定义访问包工作流扩展关联的逻辑应用终结点的配置详细信息。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7f97d944d2dffa8103ca53e04fd455d515fd41e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338407"
---
# <a name="logicapptriggerendpointconfiguration-resource-type"></a>logicAppTriggerEndpointConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与自定义访问包工作流扩展关联的逻辑应用终结点的配置详细信息。 派生自 [customExtensionEndpointConfiguration](customextensionendpointconfiguration.md) 抽象类型。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---| 
|logicAppWorkflowName|String|逻辑应用的名称。|
|resourceGroupName|String|逻辑应用的 Azure 资源组名称。|
|subscriptionId|String|逻辑应用的 Azure 订阅的标识符。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.logicAppTriggerEndpointConfiguration",
  "baseType": "microsoft.graph.customExtensionEndpointConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration",
  "subscriptionId": "String",
  "resourceGroupName": "String",
  "logicAppWorkflowName": "String"
}
```
