---
title: win32LobAppRule 资源类型
description: 用于存储 Win32 LOB 应用的检测或要求规则数据的基复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d1db8b27033022b37ef8f79f0d251408ed42b13c4b69038715350eb98f15974f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54170451"
---
# <a name="win32lobapprule-resource-type"></a>win32LobAppRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于存储 Win32 LOB 应用的检测或要求规则数据的基复杂类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|指示规则用途的规则类型。 可取值为：`detection`、`requirement`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRule",
  "ruleType": "String"
}
```




