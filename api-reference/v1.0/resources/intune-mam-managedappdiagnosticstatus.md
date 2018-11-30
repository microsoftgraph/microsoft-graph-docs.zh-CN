---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
ms.openlocfilehash: 8a462b49231323288d66a660c769ce7359cb5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010051"
---
# <a name="managedappdiagnosticstatus-resource-type"></a>managedAppDiagnosticStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示诊断状态。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|validationName|String|验证友好名称|
|状态|String|操作状态|
|mitigationInstruction|String|有关如何降低失败验证的说明|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



