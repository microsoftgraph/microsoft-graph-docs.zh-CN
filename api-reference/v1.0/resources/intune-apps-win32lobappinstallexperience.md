---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用的安装体验属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d74492b8a9a053384fc15c01270f7d4c371af4917678e5a507890c03d4165762
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152612"
---
# <a name="win32lobappinstallexperience-resource-type"></a>win32LobAppInstallExperience 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用的安装体验属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|指示应用程序运行在的执行上下文的类型。 可取值为：`system`、`user`。|
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
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```




