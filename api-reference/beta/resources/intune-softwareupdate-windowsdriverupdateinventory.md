---
title: windowsDriverUpdateInventory 资源类型
description: 表示驱动程序清单的新实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d61d8d0dbefabb0bbb2cfc2be823ff66a2ba2ae3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792124"
---
# <a name="windowsdriverupdateinventory-resource-type"></a>windowsDriverUpdateInventory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示驱动程序清单的新实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsDriverUpdateInventories](../api/intune-softwareupdate-windowsdriverupdateinventory-list.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 集合|列出 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 对象的属性和关系。|
|[获取 windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-get.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|读取 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 对象的属性和关系。|
|[创建 windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-create.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|创建新的 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 对象。|
|[删除 windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-delete.md)|无|删除 [windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)。|
|[更新 windowsDriverUpdateInventory](../api/intune-softwareupdate-windowsdriverupdateinventory-update.md)|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)|更新 [windowsDriverUpdateInventory 对象](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|驱动程序的 ID。|
|name|String|驱动程序的名称。|
|version|String|驱动程序的版本。|
|manufacturer|String|驱动程序的制造商。|
|releaseDateTime|DateTimeOffset|驱动程序的发布日期时间。|
|driverClass|String|驱动程序的类。|
|applicableDeviceCount|Int32|此驱动程序适用的设备数量。|
|approvalStatus|[driverApprovalStatus](../resources/intune-softwareupdate-driverapprovalstatus.md)|此驱动程序的审批状态。 可能的值是：`needsReview`、`declined`、`approved`、`suspended`。|
|“类别”|[driverCategory](../resources/intune-softwareupdate-drivercategory.md)|此驱动程序的类别。 可取值为：`recommended`、`previouslyApproved`、`other`。|
|deployDateTime|DateTimeOffset|如果 approvalStatus 获得批准，应部署驱动程序的日期时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateInventory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
  "id": "String (identifier)",
  "name": "String",
  "version": "String",
  "manufacturer": "String",
  "releaseDateTime": "String (timestamp)",
  "driverClass": "String",
  "applicableDeviceCount": 1024,
  "approvalStatus": "String",
  "category": "String",
  "deployDateTime": "String (timestamp)"
}
```



