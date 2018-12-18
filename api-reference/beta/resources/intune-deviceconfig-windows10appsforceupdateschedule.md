---
title: windows10AppsForceUpdateSchedule 资源类型
description: Windows 10 强制更新计划程序
author: tfitzmac
ms.openlocfilehash: 851f22e092f2669dfc44911783df6182cda1dc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323700"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>windows10AppsForceUpdateSchedule 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 10 强制更新计划程序
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|强制的开始时间重新启动。|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|定期计划。 可取值为：`none`、`daily`、`weekly`、`monthly`。|
|runImmediatelyIfAfterStartDateTime|Boolean|如果为 true，请在过去，其他人，会在下一个定期运行开始日期时间是否立即运行任务。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```





