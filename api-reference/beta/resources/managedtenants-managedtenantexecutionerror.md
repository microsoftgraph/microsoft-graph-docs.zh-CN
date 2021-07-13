---
title: managedTenantExecutionError 资源类型
description: 表示托管租户操作异常。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5a1fd2d1524cad663ee6acef93ab20cc8e40fd24
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402031"
---
# <a name="managedtenantexecutionerror-resource-type"></a>managedTenantExecutionError 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户操作异常。

继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|String|异常的错误消息。 继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。 必填。 只读。|
|errorDetails|String|异常的其他错误信息。 可选。 只读。|
|nodeId|Int32|发生异常的节点标识符。 必填。 只读。|
|rawToken|String|异常的标记。 可选。 只读。|
|statementIndex|Int32|异常的语句索引。 必填。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户标识符。 继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantExecutionError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantExecutionError",
  "tenantId": "String",
  "error": "String",
  "rawToken": "String",
  "statementIndex": "Integer",
  "nodeId": "Integer",
  "errorDetails": "String"
}
```
