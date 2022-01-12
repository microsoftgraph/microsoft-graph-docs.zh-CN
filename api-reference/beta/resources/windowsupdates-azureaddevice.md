---
title: azureADDevice 资源类型
description: 表示在部署Azure Active Directory (Azure AD) 注册的设备。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a055c944c1b7a5f2bd4bbd23a9edc8d9c3b3ff88
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792188"
---
# <a name="azureaddevice-resource-type"></a>azureADDevice 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在部署Azure Active Directory (Azure AD) 注册的设备。

系统Azure AD以下方法之一自动创建设备：
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
|[删除 azureADDevice](../api/windowsupdates-azureaddevice-delete.md)|None|删除 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。|
|[在管理中注册 azureADDevice 资源](../api/windowsupdates-updatableasset-enrollassets.md)|None|在 [部署服务更新管理中注册 azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|
|[按 ID 管理策略注册 azureADDevice (管理) ](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|None|在 [部署服务更新管理中注册 azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|
|[从管理中注销 azureADDevice 资源](../api/windowsupdates-updatableasset-unenrollassets.md)|None|从部署服务的更新管理中注销 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|
|[取消注册按 ID 管理 (azureADDevice) ](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|None|从部署服务的更新管理中注销 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。|

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

