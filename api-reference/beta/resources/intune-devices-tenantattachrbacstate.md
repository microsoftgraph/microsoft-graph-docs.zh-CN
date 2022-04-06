---
title: tenantAttachRBACState 资源类型
description: 表示 GetState API 的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 534570f827eb96658f49f115e6a5d3ba5bdc7d26
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631059"
---
# <a name="tenantattachrbacstate-resource-type"></a>tenantAttachRBACState 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 GetState API 的结果。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|已启用|Boolean|指示是否使用角色管理为租户附加启用租户附加。  如果启用，则其为 TRUE;如果禁用了具有 rolemanagement 的租户附加，则其为 FALSE。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tenantAttachRBACState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantAttachRBACState",
  "enabled": true
}
```




