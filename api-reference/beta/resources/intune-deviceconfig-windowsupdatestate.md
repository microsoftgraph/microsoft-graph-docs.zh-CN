---
title: windowsUpdateState 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20387d9e1fd9b84853a7bc097dfa08d128809358
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429486"
---
# <a name="windowsupdatestate-resource-type"></a>windowsUpdateState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|这是实体的 Id。|
|deviceId|String|设备的 id。|
|userId|String|用户的 id。|
|deviceDisplayName|String|设备的显示名称。|
|userPrincipalName|String|用户主体名称。|
|status|[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)|Windows udpate 状态。|
|qualityUpdateVersion|String|设备质量更新版本。|
|featureUpdateVersion|String|设备的当前功能更新版本。|
|lastScanDateTime|DateTimeOffset|显示日期时间的 Windows Update 代理未成功的扫描。|
|lastSyncDateTime|DateTimeOffset|与 Microsoft Intune 与设备同步的最后一个日期时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.WindowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WindowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String (identifier)",
  "userId": "String (identifier)",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```


