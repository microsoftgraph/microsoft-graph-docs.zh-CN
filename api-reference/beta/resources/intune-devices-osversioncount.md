---
title: osVersionCount 资源类型
description: 每个操作系统版本包含恶意软件的设备计数
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a0d71b2b0a82d921613823713765e72f633e9d5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091333"
---
# <a name="osversioncount-resource-type"></a>osVersionCount 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每个操作系统版本包含恶意软件的设备计数

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|osVersion|String|操作系统版本|
|deviceCount|Int32|操作系统版本包含恶意软件的设备计数|
|lastUpdateDateTime|DateTimeOffset|设备计数的上次更新时间戳（UTC 格式）|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```



