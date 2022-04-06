---
title: windowsDriverUpdateProfileInventorySyncStatus 资源类型
description: 用于存储驱动程序和固件配置文件清单同步状态的复杂类型。状态包括上次成功的同步日期时间和上次同步的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86bc48fd07619d7d5e99ef61239e6a92478cbd0f
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631033"
---
# <a name="windowsdriverupdateprofileinventorysyncstatus-resource-type"></a>windowsDriverUpdateProfileInventorySyncStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于存储驱动程序和固件配置文件清单同步状态的复杂类型。状态包括上次成功的同步日期时间和上次同步的状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastSuccessfulSyncDateTime|DateTimeOffset|上次成功同步的日期和时间（UTC 格式）。|
|driverInventorySyncState|[windowsDriverUpdateProfileInventorySyncState](../resources/intune-softwareupdate-windowsdriverupdateprofileinventorysyncstate.md)|最新同步的状态。可能的值是：、`pending`、`failure``success`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "driverInventorySyncState": "String"
}
```




