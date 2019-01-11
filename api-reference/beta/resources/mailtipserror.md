---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: 7df13bb45471d89fdf25b4a251e441bbf2dfad9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865622"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="8a8c0-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a8c0-103">mailTipsError resource type</span></span>

> <span data-ttu-id="8a8c0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8a8c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a8c0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8a8c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a8c0-106">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="8a8c0-106">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="8a8c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="8a8c0-107">Properties</span></span>
| <span data-ttu-id="8a8c0-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a8c0-108">Property</span></span>     | <span data-ttu-id="8a8c0-109">类型</span><span class="sxs-lookup"><span data-stu-id="8a8c0-109">Type</span></span>   |<span data-ttu-id="8a8c0-110">Description</span><span class="sxs-lookup"><span data-stu-id="8a8c0-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="8a8c0-111">message</span><span class="sxs-lookup"><span data-stu-id="8a8c0-111">message</span></span> | <span data-ttu-id="8a8c0-112">字符串</span><span class="sxs-lookup"><span data-stu-id="8a8c0-112">String</span></span> | <span data-ttu-id="8a8c0-113">错误消息。</span><span class="sxs-lookup"><span data-stu-id="8a8c0-113">The error message.</span></span> |
| <span data-ttu-id="8a8c0-114">code</span><span class="sxs-lookup"><span data-stu-id="8a8c0-114">code</span></span> | <span data-ttu-id="8a8c0-115">字符串</span><span class="sxs-lookup"><span data-stu-id="8a8c0-115">String</span></span> | <span data-ttu-id="8a8c0-116">错误代码。</span><span class="sxs-lookup"><span data-stu-id="8a8c0-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a8c0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a8c0-117">JSON representation</span></span>

<span data-ttu-id="8a8c0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a8c0-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
