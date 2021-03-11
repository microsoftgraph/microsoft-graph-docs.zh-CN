---
title: teamworkHostedContent 资源类型
description: 表示 Microsoft Teams 托管的丰富内容。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a4a4d0a553f77766dd4ddb1f68e27b440fdbf2f
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634294"
---
# <a name="teamworkhostedcontent-resource-type"></a>teamworkHostedContent 资源类型

命名空间：microsoft.graph

表示 Microsoft Teams 中的丰富内容，如图像和代码段。 有关频道和聊天消息[中的丰富内容](chatMessage.md)，请参阅[chatMessageHostedContent。](chatMessageHostedContent.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentBytes|Binary|仅写入。 托管内容存储的字节 (例如图像) 。|
|contentType|String|仅写入。 内容类型。 sicj as image/png， image/jpg.|
|id|String|托管内容的 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```
