---
title: subjectRightsRequestEnumeratedMailboxLocation 资源类型
description: 表示主题权限请求的属性，该请求定义特定邮箱 (Exchange邮箱以及个人或组Microsoft Teams聊天) 作为搜索位置。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 1edae24833a7e003fa1a498ca3642508e38af6fa
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461668"
---
# <a name="subjectrightsrequestenumeratedmailboxlocation-resource-type"></a>subjectRightsRequestEnumeratedMailboxLocation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示主题权限请求的属性，该请求定义特定邮箱 (Exchange邮箱以及个人或组Microsoft Teams聊天) 作为搜索位置。

继承自 [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|upns|String collection|应包含在搜索中的邮箱集合。 包括每个邮箱的 UPN (用户主体名称) ，例如 `Monica.Thompson@contoso.com`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestEnumeratedMailboxLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestEnumeratedMailboxLocation",
  "upns": [
    "String"
  ]
}
```

