---
title: audioSourceLevel 资源类型
description: 对于其他源的级别配置。
author: VinodRavichandran
ms.openlocfilehash: 5d5abe7eba03891427b30ba1c8f63b15b3707e46
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380238"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="8dd3c-103">audioSourceLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="8dd3c-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="8dd3c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dd3c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8dd3c-106">对于其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="8dd3c-107">属性</span><span class="sxs-lookup"><span data-stu-id="8dd3c-107">Properties</span></span>

| <span data-ttu-id="8dd3c-108">属性</span><span class="sxs-lookup"><span data-stu-id="8dd3c-108">Property</span></span>               | <span data-ttu-id="8dd3c-109">类型</span><span class="sxs-lookup"><span data-stu-id="8dd3c-109">Type</span></span>    | <span data-ttu-id="8dd3c-110">说明</span><span class="sxs-lookup"><span data-stu-id="8dd3c-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8dd3c-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="8dd3c-111">duckOthers</span></span>             | <span data-ttu-id="8dd3c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dd3c-112">Boolean</span></span> | <span data-ttu-id="8dd3c-113">允许此源回避活动时的其他源。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="8dd3c-114">如果设置为 true，放掉级别设置。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="8dd3c-115">level</span><span class="sxs-lookup"><span data-stu-id="8dd3c-115">level</span></span>                  | <span data-ttu-id="8dd3c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8dd3c-116">Int64</span></span>   | <span data-ttu-id="8dd3c-117">如果放掉源的级别`duckOthers`设置为`true`。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="8dd3c-118">参与者</span><span class="sxs-lookup"><span data-stu-id="8dd3c-118">participant</span></span>            | <span data-ttu-id="8dd3c-119">字符串</span><span class="sxs-lookup"><span data-stu-id="8dd3c-119">String</span></span>  | <span data-ttu-id="8dd3c-120">源参与者音频流。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="8dd3c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8dd3c-121">JSON representation</span></span>

<span data-ttu-id="8dd3c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dd3c-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
