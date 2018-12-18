---
title: iosBookmark 资源类型
description: iOS URL 书签
author: tfitzmac
ms.openlocfilehash: e1577537e57365b2452e956e010f6c3f918bd743
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308398"
---
# <a name="iosbookmark-resource-type"></a>iosBookmark 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

iOS URL 书签
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|url|String|允许访问的 URL|
|bookmarkFolder|字符串|向其中应在 Safari 中添加书签的文件夹|
|displayName|字符串|书签的显示名称|

## <a name="relationships"></a>Relationships
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





