---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f974ae033389deba42a838f122e2b2bb200db84
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454775"
---
# <a name="organization-resource-type"></a>组织资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组织资源表示在租户级别操作和配置的全局设置和资源的实例。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 organizations](../api/intune-onboarding-organization-list.md)|[organization](../resources/intune-onboarding-organization.md) 集合|列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。|
|[获取组织](../api/intune-onboarding-organization-get.md)|[组织](../resources/intune-onboarding-organization.md)|读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。|
|[更新 organization](../api/intune-onboarding-organization-update.md)|[organization](../resources/intune-onboarding-organization.md)|更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。|
|[setMobileDeviceManagementAuthority 操作](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|Int32|设置移动设备管理机构|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID。|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune-onboarding-mdmauthority.md)|移动设备管理机构。 可取值为：`unknown`、`intune`、`sccm`、`office365`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```



