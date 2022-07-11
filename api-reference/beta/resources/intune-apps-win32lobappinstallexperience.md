---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用的安装体验属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ca646e00800e62005c7aad89bd44439bfb85748
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666835"
---
# <a name="win32lobappinstallexperience-resource-type"></a>win32LobAppInstallExperience 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用的安装体验属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|指示应用在其中运行的执行上下文的类型。 可取值为：`system`、`user`。|
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




