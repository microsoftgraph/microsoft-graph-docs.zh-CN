---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1c2a324c30e1372cc6ba79c3330249121fe0d367
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023253"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>mobileAppInstallTimeSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。

## <a name="properties"></a>属性
|属性|类型|描述|
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



