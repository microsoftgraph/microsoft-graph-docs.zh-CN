---
title: groupWritebackConfiguration 资源类型
description: 指示是否已启用云组到本地 Active Directory 的写回以及本地组的目标组类型。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1b546da83c3f53ad1b8126e2967e224e9569cbf5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439684"
---
# <a name="groupwritebackconfiguration-resource-type"></a>groupWritebackConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示是否已启用云组到本地 Active Directory 的写回以及本地组的目标组类型。

 默认情况下，所有 Azure AD 安全组均未启用写回。 对于 Microsoft 365 组，可由此资源的属性定义的默认设置由`NewUnifiedgroupWritebackDefault`[目录设置对象](directorysetting.md)覆盖。

继承自 [writebackConfiguration](../resources/writebackconfiguration.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否已启用将云组写回本地 Active Directory。 可为 NULL。 默认值 `true` 适用于 Microsoft 365 组和安全 `false` 组。 继承自 [writebackConfiguration](../resources/writebackconfiguration.md)。|
|onPremisesGroupType|String|指示将写回云对象的目标本地组类型。 可为 NULL。 可能的值包括 `universalDistributionGroup`、`universalSecurityGroup`、`universalMailEnabledSecurityGroup`。 <br>+ 如果云组是统一 (Microsoft 365) 组，则此属性可以是下列属性之一： `universalDistributionGroup`， `universalSecurityGroup`。 `universalMailEnabledSecurityGroup` <br> + Azure AD 安全组可以写回为 `universalSecurityGroup`。 <br> + 如果 **isEnabled** 或`NewUnifiedGroupWritebackDefault`[组设置](directorysetting.md)为`true`，但未显式配置此属性： <br> &nbsp;&nbsp; + Microsoft 365 组将默认写回`universalDistributionGroup` <br> &nbsp;&nbsp; + 默认情况下将写回`universalSecurityGroup`安全组|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupWritebackConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupWritebackConfiguration",
  "isEnabled": "Boolean",
  "onPremisesGroupType": "String"
}
```

