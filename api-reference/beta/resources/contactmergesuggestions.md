---
title: contactMergeSuggestions 资源类型
description: 表示建议在用户联系人列表中检测到Outlook项时合并联系人项目的功能
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 56237901cca14d075dfa7f03729a9261d8d281a0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338313"
---
# <a name="contactmergesuggestions-resource-type"></a>contactMergeSuggestions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在用户联系人列表中检测到重复项Outlook建议合并联系人项目的功能。

此资源提供了一种在用户级别启用或禁用功能的方式。 默认情况下，建议已启用。 重复的联系人项目在联系人文件夹中保留为重复项，除非用户选择合并它们。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/contactmergesuggestions-get.md)|[contactMergeSuggestions](contactmergesuggestions.md)|读取 **contactMergeSuggestions 对象** 的属性。|
|[更新](../api/contactmergesuggestions-update.md)|无 |更新 **contactMergeSuggestions 对象** 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|`true` 如果为用户启用了重复的联系人合并建议功能; `false` 如果禁用此功能。 默认值为 `true`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactMergeSuggestions",
  "openType": false
}
-->
``` json
{
  "isEnabled": "Boolean"
}
```

