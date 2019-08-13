---
title: loggedOnUser 资源类型
description: 登录用户
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a32ee6182f8937123662e3a8c3e4d18145607151
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372326"
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



