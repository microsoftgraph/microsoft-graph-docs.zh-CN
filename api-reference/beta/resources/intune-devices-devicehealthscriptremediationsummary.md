---
title: deviceHealthScriptRemediationSummary 资源类型
description: 部署的设备运行状况脚本数和已修复脚本的设备数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac9e06cdbc8aa5ba754528459e52142b7e4f3679
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820686"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a>deviceHealthScriptRemediationSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

部署的设备运行状况脚本数和已修复脚本的设备数。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|scriptCount|Int32|部署的设备运行状况脚本的数量。|
|remediatedDeviceCount|Int32|由设备运行状况脚本修正的设备数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```



