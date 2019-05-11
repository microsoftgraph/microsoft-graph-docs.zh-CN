---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示用于用户权限设置的本地用户或组的信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acccbb68ecc0b62d27ac20e3eba9e637aac3e11c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946936"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示用于用户权限设置的本地用户或组的信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|此本地用户或组的名称。|
|说明|String|管理员对此本地用户或组的说明。|
|securityIdentifier|String|此本地用户或组的安全标识符 (例如 * S-1-5-32-544)。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```




