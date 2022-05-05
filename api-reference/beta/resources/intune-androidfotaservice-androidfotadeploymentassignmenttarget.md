---
title: androidFotaDeploymentAssignmentTarget 资源类型
description: 要将固件更新部署到的AAD组
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bc95f25abe2f1971573a4b4904b2535420fe9ff
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213115"
---
# <a name="androidfotadeploymentassignmenttarget-resource-type"></a>androidFotaDeploymentAssignmentTarget 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要将固件更新部署到的AAD组

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|groupId|String|AAD组 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidFotaDeploymentAssignmentTarget",
  "groupId": "String"
}
```




