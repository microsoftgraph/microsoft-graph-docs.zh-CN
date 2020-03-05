---
title: mediaPrompt 资源类型
description: 此资源类型包含有关要播放的音频文件和其他其他设置的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4bc2f315a2f339d2ef6fe0f4b76b335970b5a642
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447442"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="b8306-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8306-103">mediaPrompt resource type</span></span>

<span data-ttu-id="b8306-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b8306-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8306-105">此资源类型包含有关要播放的音频文件和其他其他设置的信息。</span><span class="sxs-lookup"><span data-stu-id="b8306-105">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="b8306-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8306-106">Properties</span></span>

| <span data-ttu-id="b8306-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8306-107">Property</span></span>    | <span data-ttu-id="b8306-108">类型</span><span class="sxs-lookup"><span data-stu-id="b8306-108">Type</span></span>                      | <span data-ttu-id="b8306-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8306-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="b8306-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="b8306-110">mediaInfo</span></span>   | [<span data-ttu-id="b8306-111">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="b8306-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="b8306-112">媒体信息</span><span class="sxs-lookup"><span data-stu-id="b8306-112">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="b8306-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8306-113">JSON representation</span></span>

<span data-ttu-id="b8306-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8306-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
