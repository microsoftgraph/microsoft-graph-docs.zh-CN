---
title: win32LobAppInstallExperience 资源类型
description: 包含 Win32 应用程序的安装体验属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c981c2ae9842e928d35ec05f146955dd766d6c35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012294"
---
# <a name="win32lobappinstallexperience-resource-type"></a>win32LobAppInstallExperience 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用程序的安装体验属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示应用程序在其中运行的执行上下文的类型。 可取值为：`system`、`user`。|

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
  "runAsAccount": "String"
}
```





