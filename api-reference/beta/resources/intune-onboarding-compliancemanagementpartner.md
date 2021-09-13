---
title: complianceManagementPartner 资源类型
description: 所有平台的合规性管理合作伙伴
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc3e4ebd5009a410942cbfe6324bed259bf964a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017238"
---
# <a name="compliancemanagementpartner-resource-type"></a>complianceManagementPartner 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

所有平台的合规性管理合作伙伴

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 complianceManagementPartners](../api/intune-onboarding-compliancemanagementpartner-list.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 集合|列出 [complianceManagementPartner 对象的属性和](../resources/intune-onboarding-compliancemanagementpartner.md) 关系。|
|[获取 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|读取 [complianceManagementPartner 对象的属性和](../resources/intune-onboarding-compliancemanagementpartner.md) 关系。|
|[创建 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|创建新的 [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象。|
|[删除 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-delete.md)|None|删除 [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)。|
|[更新 complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|更新 [complianceManagementPartner 对象](../resources/intune-onboarding-compliancemanagementpartner.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的 ID|
|lastHeartbeatDateTime|DateTimeOffset|管理员载入合规性管理合作伙伴后最后检测信号的时间戳|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|此租户的合作伙伴状态。 可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。|
|displayName|String|合作伙伴显示名称|
|macOsOnboarded|布尔值|为 Mac 设备载入的合作伙伴。|
|windowsOnboarded|布尔值|合作伙伴已载入Windows设备。|
|androidOnboarded|布尔值|针对 Android 设备加入的合作伙伴。|
|iosOnboarded|布尔值|为 ios 设备载入的合作伙伴。|
|macOsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合|通过合作伙伴注册 Mac 设备的用户组。|
|windowsEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合|通过合作伙伴注册Windows的用户组。|
|androidEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合|通过合作伙伴注册 Android 设备的用户组。|
|iosEnrollmentAssignments|[complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md) 集合|通过合作伙伴注册 ios 设备的用户组。|

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ]
}
```



