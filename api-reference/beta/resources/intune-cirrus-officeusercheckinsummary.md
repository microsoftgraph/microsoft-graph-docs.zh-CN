---
title: officeUserCheckinSummary 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8564f7d0d2fb06218b141b7e9369f2096bdec982
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462517"
---
# <a name="officeusercheckinsummary-resource-type"></a>officeUserCheckinSummary 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述租户签入统计信息的实体。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|succeededUserCount|Int32|最近3个月内成功的用户签入次数总计。|
|failedUserCount|Int32|最近3个月的用户签入失败总计。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



