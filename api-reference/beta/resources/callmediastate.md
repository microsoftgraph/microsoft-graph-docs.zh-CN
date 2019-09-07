---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: VinodRavichandran
ms.prod: microsoft-teams
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 6b092598c50663ec9e7803a13332798d05fe095b
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793019"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="fcf63-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcf63-103">audioConferencing resource type</span></span>

> <span data-ttu-id="fcf63-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fcf63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcf63-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fcf63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fcf63-106">表示呼叫[呼叫](call.md)的媒体状态。</span><span class="sxs-lookup"><span data-stu-id="fcf63-106">Represents the media state for a call [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fcf63-107">属性</span><span class="sxs-lookup"><span data-stu-id="fcf63-107">Properties</span></span>

| <span data-ttu-id="fcf63-108">属性</span><span class="sxs-lookup"><span data-stu-id="fcf63-108">Property</span></span>            | <span data-ttu-id="fcf63-109">类型</span><span class="sxs-lookup"><span data-stu-id="fcf63-109">Type</span></span>    | <span data-ttu-id="fcf63-110">说明</span><span class="sxs-lookup"><span data-stu-id="fcf63-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="fcf63-111">audio</span><span class="sxs-lookup"><span data-stu-id="fcf63-111">audio</span></span>           | <span data-ttu-id="fcf63-112">String</span><span class="sxs-lookup"><span data-stu-id="fcf63-112">String</span></span>  | <span data-ttu-id="fcf63-113">音频媒体状态。</span><span class="sxs-lookup"><span data-stu-id="fcf63-113">The audio media state.</span></span> <span data-ttu-id="fcf63-114">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="fcf63-114">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fcf63-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcf63-115">JSON representation</span></span>

<span data-ttu-id="fcf63-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcf63-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
