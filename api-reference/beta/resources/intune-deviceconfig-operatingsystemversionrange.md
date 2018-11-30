---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
ms.openlocfilehash: af140bf2a5d889b66d45460465e47c466bb2160b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043531"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

操作系统版本范围。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|字符串|此范围 （如有效 1702年生成） 的说明|
|lowestVersion|字符串|最低非独占此范围包含版本。|
|highestVersion|字符串|包含此范围的最高非独占版本。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





