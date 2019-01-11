---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: cfe859bea40f15311a631e8b1d2b3c3a3c179d0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891530"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="17878-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="17878-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="17878-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="17878-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17878-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17878-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17878-106">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="17878-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17878-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17878-107">JSON representation</span></span>

<span data-ttu-id="17878-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17878-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="17878-109">属性</span><span class="sxs-lookup"><span data-stu-id="17878-109">Properties</span></span>
| <span data-ttu-id="17878-110">属性</span><span class="sxs-lookup"><span data-stu-id="17878-110">Property</span></span>     | <span data-ttu-id="17878-111">类型</span><span class="sxs-lookup"><span data-stu-id="17878-111">Type</span></span>   |<span data-ttu-id="17878-112">说明</span><span class="sxs-lookup"><span data-stu-id="17878-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17878-113">code</span><span class="sxs-lookup"><span data-stu-id="17878-113">code</span></span>|<span data-ttu-id="17878-114">string</span><span class="sxs-lookup"><span data-stu-id="17878-114">string</span></span>|<span data-ttu-id="17878-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="17878-115">The error code.</span></span>|
|<span data-ttu-id="17878-116">消息</span><span class="sxs-lookup"><span data-stu-id="17878-116">message</span></span>|<span data-ttu-id="17878-117">string</span><span class="sxs-lookup"><span data-stu-id="17878-117">string</span></span>|<span data-ttu-id="17878-118">错误消息。</span><span class="sxs-lookup"><span data-stu-id="17878-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
