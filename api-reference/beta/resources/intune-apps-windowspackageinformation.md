---
title: windowsPackageInformation 资源类型
description: 包含为业务应用程序的 Windows 行的程序包信息的属性。
author: tfitzmac
ms.openlocfilehash: dcc277c610e6ceb27a94ab41993e599a258dd55e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342824"
---
# <a name="windowspackageinformation-resource-type"></a>windowsPackageInformation 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含为业务应用程序的 Windows 行的程序包信息的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|运行此应用程序可以为其 Windows 体系结构。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。|
|displayName|字符串|显示名称。|
|identityName|String|标识名称。|
|identityPublisher|字符串|标识发布者。|
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
    "v10_1803": true
  }
}
```





