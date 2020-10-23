---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a2965a2ba1f30d19e4f755caa0d10676d110f41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730344"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>mobileAppInstallTimeSettings 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|useLocalTime|布尔|确定可用时间和截止时间时，是否应使用本地设备时间或 UTC 时间。|
|startDateTime|DateTimeOffset|应用程序可供安装的时间。|
|deadlineDateTime|DateTimeOffset|应安装应用程序的时间。|

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





