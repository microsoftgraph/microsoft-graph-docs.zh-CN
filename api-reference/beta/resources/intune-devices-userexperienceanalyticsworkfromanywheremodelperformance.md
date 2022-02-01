---
title: userExperienceAnalyticsWorkFromAnywhereModelPerformance 资源类型
description: 用户体验分析从任何模型性能开始工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c6a21965c5f1f947b2f3d66dafcfb03cb777fc9
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292287"
---
# <a name="userexperienceanalyticsworkfromanywheremodelperformance-resource-type"></a>userExperienceAnalyticsWorkFromAnywhereModelPerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析从任何模型性能开始工作。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsWorkFromAnywhereModelPerformances](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-list.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) 集合|列出 [userExperienceAnalyticsWorkFromAnywhereModelPerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) 关系。|
|[获取 userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-get.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|读取 [userExperienceAnalyticsWorkFromAnywhereModelPerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) 关系。|
|[创建 userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-create.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|创建新的 [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) 对象。|
|[删除 userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-delete.md)|无|删除 [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)。|
|[更新 userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-update.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|更新 [userExperienceAnalyticsWorkFromAnywhereModelPerformance 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析模型性能对象的唯一标识符。|
|model|String|用户体验从任何设备的型号名称开始工作。|
|manufacturer|String|用户体验从设备的制造商名称的任何位置工作。|
|modelDeviceCount|Int32|用户体验适用于任何设备的型号计数。 有效值 -2147483648 2147483647|
|workFromAnywhereScore|双精度|用户体验从模型的整体分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|windowsScore|双精度|用户体验适用于模型的任何窗口分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudManagementScore|双精度|用户体验从模型的云管理分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudIdentityScore|双精度|用户体验从模型的云标识分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudProvisioningScore|双精度|用户体验从适用于模型的云预配分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析的运行状况从任何模型开始工作。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance",
  "id": "String (identifier)",
  "model": "String",
  "manufacturer": "String",
  "modelDeviceCount": 1024,
  "workFromAnywhereScore": "4.2",
  "windowsScore": "4.2",
  "cloudManagementScore": "4.2",
  "cloudIdentityScore": "4.2",
  "cloudProvisioningScore": "4.2",
  "healthStatus": "String"
}
```




