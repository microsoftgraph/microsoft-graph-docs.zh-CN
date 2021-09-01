---
title: windowsUpdateState 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c0f4e986483f5c4dce849295406ebad3cec721c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803747"
---
# <a name="windowsupdatestate-resource-type"></a>windowsUpdateState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsUpdateStates](../api/intune-shared-windowsupdatestate-list.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 集合|列出 [windowsUpdateState 对象的属性和](../resources/intune-shared-windowsupdatestate.md) 关系。|
|[获取 windowsUpdateState](../api/intune-shared-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|读取 [windowsUpdateState 对象的属性和](../resources/intune-shared-windowsupdatestate.md) 关系。|
|[创建 windowsUpdateState](../api/intune-shared-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|创建新的 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象。|
|[删除 windowsUpdateState](../api/intune-shared-windowsupdatestate-delete.md)|无|删除 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)。|
|[更新 windowsUpdateState](../api/intune-shared-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)|更新 [windowsUpdateState 对象](../resources/intune-shared-windowsupdatestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|这是实体的 ID。|
|deviceId|String|设备的 ID。|
|userId|String|用户的 ID。|
|deviceDisplayName|String|设备显示名称。|
|userPrincipalName|String|用户主体名称。|
|状态|[windowsUpdateStatus](../resources/intune-shared-windowsupdatestatus.md)|Windows udpate 状态。 可能的值是：`upToDate`、`pendingInstallation`、`pendingReboot`、`failed`。|
|qualityUpdateVersion|String|质量更新设备的版本。|
|featureUpdateVersion|String|设备的当前功能更新版本。|
|lastScanDateTime|DateTimeOffset|更新代理执行Windows扫描的日期时间。|
|lastSyncDateTime|DateTimeOffset|设备上次与设备同步的日期Microsoft Intune。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```



