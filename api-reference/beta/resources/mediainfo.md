---
title: mediaInfo 资源类型
description: 操作中使用的媒体信息提示。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 6fe2c49e86bac9d5961310694b21e9439a4896ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885601"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="53caf-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="53caf-103">mediaInfo resource type</span></span>

> <span data-ttu-id="53caf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="53caf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53caf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53caf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53caf-106">操作中使用的媒体信息提示。</span><span class="sxs-lookup"><span data-stu-id="53caf-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="53caf-107">属性</span><span class="sxs-lookup"><span data-stu-id="53caf-107">Properties</span></span>
| <span data-ttu-id="53caf-108">属性</span><span class="sxs-lookup"><span data-stu-id="53caf-108">Property</span></span>       | <span data-ttu-id="53caf-109">类型</span><span class="sxs-lookup"><span data-stu-id="53caf-109">Type</span></span>    | <span data-ttu-id="53caf-110">Description</span><span class="sxs-lookup"><span data-stu-id="53caf-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="53caf-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="53caf-111">resourceId</span></span>     | <span data-ttu-id="53caf-112">String</span><span class="sxs-lookup"><span data-stu-id="53caf-112">String</span></span>  | <span data-ttu-id="53caf-113">唯一标识的资源。</span><span class="sxs-lookup"><span data-stu-id="53caf-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="53caf-114">uri</span><span class="sxs-lookup"><span data-stu-id="53caf-114">uri</span></span>            | <span data-ttu-id="53caf-115">字符串</span><span class="sxs-lookup"><span data-stu-id="53caf-115">String</span></span>  | <span data-ttu-id="53caf-116">资源的路径。</span><span class="sxs-lookup"><span data-stu-id="53caf-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="53caf-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53caf-117">JSON representation</span></span>

<span data-ttu-id="53caf-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53caf-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
