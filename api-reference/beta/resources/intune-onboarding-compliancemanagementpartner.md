---
title: complianceManagementPartner 资源类型
description: 适用于所有平台的合规性管理合作伙伴
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 50dd8cabc61cba2207b661ce9398b022838ed8ea
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088047"
---
# <a name="compliancemanagementpartner-resource-type"></a>complianceManagementPartner 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于所有平台的合规性管理合作伙伴

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 complianceManagementPartners](../api/intune-onboarding-compliancemanagementpartner-list.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)集合|列出[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性和关系。|
|[获取 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|读取[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性和关系。|
|[创建 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|创建新的[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。|
|[删除 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-delete.md)|无|删除[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)。|
|[更新 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|更新[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的 Id|
|lastHeartbeatDateTime|DateTimeOffset|Admin 载入到合规性管理合作伙伴之后的最后一次检测信号的时间戳|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|此租户的合作伙伴状态。 可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。|
|displayName|String|合作伙伴显示名称|
|macOsOnboarded|Boolean|适用于 Mac 设备的合作伙伴载入。|
|windowsOnboarded|Boolean|适用于 Windows 设备的合作伙伴载入。|
|androidOnboarded|Boolean|适用于 Android 设备的合作伙伴载入。|
|iosOnboarded|Boolean|适用于 ios 设备的合作伙伴载入。|
|macOsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合|通过合作伙伴注册 Mac 设备的用户组。|
|windowsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合|通过合作伙伴注册 Windows 设备的用户组。|
|androidEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合|通过合作伙伴注册 Android 设备的用户组。|
|iosEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)集合|通过合作伙伴注册 ios 设备的用户组。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.complianceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "displayName": "String",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```



