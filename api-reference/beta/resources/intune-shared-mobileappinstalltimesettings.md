---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b22ae3e5e9b94527417f671d0c6ca3a3545fee6e6819ef31743d0be410129e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251125"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>mobileAppInstallTimeSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|useLocalTime|布尔值|确定可用和截止时间时，应该使用本地设备时间还是 UTC 时间。|
|startDateTime|DateTimeOffset|应用应可供安装的时间。|
|deadlineDateTime|DateTimeOffset|应安装应用的时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```




