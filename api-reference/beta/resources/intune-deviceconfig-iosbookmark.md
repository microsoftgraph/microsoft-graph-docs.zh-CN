---
title: iosBookmark 资源类型
description: iOS URL 书签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9de5d95cd14931da850ab9bdaf5c581fd17f09dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174994"
---
# <a name="iosbookmark-resource-type"></a>iosBookmark 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS URL 书签

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|url|String|允许访问的 URL|
|bookmarkFolder|字符串|应在 Safari 中添加书签的文件夹|
|displayName|字符串|书签的显示名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




