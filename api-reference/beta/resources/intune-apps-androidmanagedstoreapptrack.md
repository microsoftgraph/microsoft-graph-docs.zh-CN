---
title: androidManagedStoreAppTrack 资源类型
description: 包含 Android 托管应用商店应用的跟踪信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bd0b73caa37ef5a1a56b7a80addc941c567f9fb347fdd4dafcb285836b12d65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54233012"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a>androidManagedStoreAppTrack 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Android 托管应用商店应用的跟踪信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|trackId|字符串|唯一轨标识符。|
|trackAlias|String|跟踪的友好名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```




