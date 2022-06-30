---
title: writebackConfiguration 资源类型
description: 表示 Azure AD 云组 (Microsoft 365 和安全组) 的写回状态。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5b2dffd738684838ac0265f1f745f0071ec0aa60
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447565"
---
# <a name="writebackconfiguration-resource-type"></a>writebackConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 云组 (Microsoft 365 和安全组) 的写回状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否已启用将云组写回本地 Active Directory。 默认值 `true` 适用于 Microsoft 365 组和安全 `false` 组。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.writebackConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.writebackConfiguration",
  "isEnabled": "Boolean"
}
```

