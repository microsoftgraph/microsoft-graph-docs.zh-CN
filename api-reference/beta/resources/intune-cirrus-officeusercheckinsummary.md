---
title: officeUserCheckinSummary 资源类型
description: 介绍租户中签入 stats 的实体。
author: tfitzmac
ms.openlocfilehash: 5064882f74a13feca726a6ebb91c34cf9a85af86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306326"
---
# <a name="officeusercheckinsummary-resource-type"></a>officeUserCheckinSummary 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

介绍租户中签入 stats 的实体。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|succeededUserCount|Int32|总用户成功检查的最近 3 个月的项。|
|failedUserCount|Int32|失败的总用户检查的最近 3 个月的项。|

## <a name="relationships"></a>Relationships
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



