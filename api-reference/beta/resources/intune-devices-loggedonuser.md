---
title: loggedOnUser 资源类型
description: 登录用户
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeacee7d4d3a22e0d069851c1f9271ceb0e32c0d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941966"
---
# <a name="loggedonuser-resource-type"></a>loggedOnUser 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

登录用户

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userId|String|用户 ID|
|lastLogOnDateTime|DateTimeOffset|用户登录的日期时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




