---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb768938ffa2e167f13a267451041b65f39011c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755117"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>mobileAppInstallTimeSettings 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|useLocalTime|Boolean|确定可用和截止时间时，应该使用本地设备时间还是 UTC 时间。|
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




