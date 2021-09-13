---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示用于用户权限设置的本地用户或组的信息。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb8dd01d090c5d0aaef133b5e5b6367f5acdd278
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069227"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示用于用户权限设置的本地用户或组的信息。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|name|String|此本地用户或组的名称。|
|说明|String|此本地用户或组的管理员说明。|
|securityIdentifier|字符串|此本地用户或组的安全标识符 (例如 *S-1-5-32-544) 。|

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



