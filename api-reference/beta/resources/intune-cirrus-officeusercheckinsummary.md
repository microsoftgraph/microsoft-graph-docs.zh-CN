---
title: officeUserCheckinSummary 资源类型
description: 描述租户签入统计数据的实体。
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38428d8f7e4f8808b8275f45c94757368b50e3f4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069367"
---
# <a name="officeusercheckinsummary-resource-type"></a>officeUserCheckinSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述租户签入统计数据的实体。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|succeededUserCount|Int32|最近 3 个月内用户签入成功总数。|
|failedUserCount|Int32|最近 3 个月内用户签入失败总数。|

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



