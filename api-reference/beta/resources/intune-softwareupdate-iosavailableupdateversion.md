---
title: iosAvailableUpdateVersion 资源类型
description: iOS 可用更新版本详细信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3174d0405785d31547f5b85bbd21d48598b9837783b97d0dd782b639ff43e7c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193508"
---
# <a name="iosavailableupdateversion-resource-type"></a>iosAvailableUpdateVersion 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS 可用更新版本详细信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|productVersion|String|更新的版本。|
|postingDateTime|DateTimeOffset|更新的发布日期。|
|expirationDateTime|DateTimeOffset|更新的到期日期。|
|supportedDevices|String collection|更新支持的设备列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```




