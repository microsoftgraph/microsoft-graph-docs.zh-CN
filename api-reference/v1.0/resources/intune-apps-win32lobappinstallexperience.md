---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 468afea165645c2fc6a728e5a171b1ef37e9e338
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080079"
---
# <a name="win32lobappinstallexperience-resource-type"></a>win32LobAppInstallExperience 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用程序的安装体验属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceRestartBehavior|[win32LobAppRestartBehavior](../resources/intune-apps-win32lobapprestartbehavior.md)|设备重启行为。 可取值为：`basedOnReturnCode`、`allow`、`suppress`、`force`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "deviceRestartBehavior": "String"
}
```





