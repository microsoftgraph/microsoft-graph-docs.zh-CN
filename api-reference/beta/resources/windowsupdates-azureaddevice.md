---
title: azureADDevice 资源类型
description: 表示 Azure AD Azure Active Directory (注册) Azure AD 服务中的设备。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a9d7b68257895674530acfbafcd0fb6b6c9c7b02
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067871"
---
# <a name="azureaddevice-resource-type"></a>azureADDevice 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD Azure Active Directory (注册) Azure AD 服务中的设备。

Azure AD 设备通过以下方法之一自动创建：
* [updatableAsset： enrollAssets](../api/windowsupdates-updatableasset-enrollassets.md)
* [updatableAsset： enrollAssetsById](../api/windowsupdates-updatableasset-enrollassetsbyid.md)
* [deploymentAudience：updateAudience](../api/windowsupdates-deploymentaudience-updateaudience.md)
* [deploymentAudience：updateAudienceById](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)
* [updatableAssetGroup：addMembers](../api/windowsupdates-updatableassetgroup-addmembers.md)
* [updatableAssetGroup：addMembersById](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)

继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 azureADDevice 资源](../api/windowsupdates-updates-list-updatableassets-azureaddevice.md)|[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md) 集合|获取 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象及其属性的列表。|
|[获取 azureADDevice](../api/windowsupdates-azureaddevice-get.md)|[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)|读取 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象的属性和关系。|
|[删除 azureADDevice](../api/windowsupdates-azureaddevice-delete.md)|无|删除 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。|
|[在管理中注册 azureADDevice 资源](../api/windowsupdates-updatableasset-enrollassets.md)|无|在 [部署服务更新管理中注册 azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|
|[按 ID 管理中心注册 azureADDevice (azureADDevice) ](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|无|在 [部署服务更新管理中注册 azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|
|[从管理中注销 azureADDevice 资源](../api/windowsupdates-updatableasset-unenrollassets.md)|无|从部署服务的更新管理中注销 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|
|[取消注册按 ID 管理 (azureADDevice) ](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|无|从部署服务的更新管理中注销 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enrollments|[microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md) 集合|指定设备注册的服务区域。 只读。 默认情况下返回。|
|错误|[microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md) 集合|指定阻止设备注册更新管理或重新记录已部署内容的任何错误。 只读。 默认情况下返回。|
|id|String|设备的标识符。 键。 不可为 null。 只读。 默认情况下返回。 继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
  "id": "String (identifier)",
  "errors": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
    }
  ],
  "enrollments": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
    }
  ]
}
```

