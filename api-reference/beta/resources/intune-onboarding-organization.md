---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bc7a0fba8c5ecdc2b2a88062855e8b279721c45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990766"
---
# <a name="organization-resource-type"></a>组织资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

组织资源表示在租户级别操作和配置的全局设置和资源的实例。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 organizations](../api/intune-onboarding-organization-list.md)|[organization](../resources/intune-onboarding-organization.md) 集合|列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。|
|[获取 organization](../api/intune-onboarding-organization-get.md)|[organization](../resources/intune-onboarding-organization.md)|读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。|
|[更新 organization](../api/intune-onboarding-organization-update.md)|[organization](../resources/intune-onboarding-organization.md)|更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。|
|[setMobileDeviceManagementAuthority 操作](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|Int32|设置移动设备管理机构|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID。|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune-onboarding-mdmauthority.md)|移动设备管理机构。 可取值为：`unknown`、`intune`、`sccm`、`office365`。|
|certificateConnectorSetting|[certificateConnectorSetting](../resources/intune-onboarding-certificateconnectorsetting.md)|证书连接器设置。|

## <a name="relationships"></a>Relationships
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
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```





