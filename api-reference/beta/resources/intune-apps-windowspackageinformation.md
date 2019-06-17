---
title: 了 windowspackageinformation 资源类型
description: 包含 Windows 业务线应用程序的包信息的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63b335aec3a4eeebb5d7cf031a05eaa7547bfd25
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975656"
---
# <a name="windowspackageinformation-resource-type"></a>了 windowspackageinformation 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Windows 业务线应用程序的包信息的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|将 applicablearchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|可在其上运行此应用程序的 Windows 体系结构。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。|
|displayName|String|显示名称。|
|identityName|String|标识名称。|
|identityPublisher|String|标识发布者。|
|identityResourceIdentifier|String|标识资源标识符。|
|identityVersion|String|标识版本。|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|最低适用操作系统的值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  }
}
```





