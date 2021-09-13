---
title: windowsKioskAzureADUser 资源类型
description: 用于标识展台配置的 AzureAD 用户帐户的类
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b0a0528c119c9f75306cb8f132ff2d35aee5a29
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086531"
---
# <a name="windowskioskazureaduser-resource-type"></a>windowsKioskAzureADUser 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于标识展台配置的 AzureAD 用户帐户的类


继承自 [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|userId|String|将锁定到此展台配置的 AzureAD 用户的 ID|
|userPrincipalName|String|将锁定到此展台配置的用户帐户|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```



