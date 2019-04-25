---
title: domainState 资源类型
description: 表示在域上计划的异步操作的状态。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6a7741448b9c91be32f67f89cbafa5a579320083
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562775"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="96731-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="96731-103">domainState resource type</span></span>

<span data-ttu-id="96731-104">表示在域上计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="96731-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="96731-105">属性</span><span class="sxs-lookup"><span data-stu-id="96731-105">Properties</span></span>

| <span data-ttu-id="96731-106">属性</span><span class="sxs-lookup"><span data-stu-id="96731-106">Property</span></span>   | <span data-ttu-id="96731-107">类型</span><span class="sxs-lookup"><span data-stu-id="96731-107">Type</span></span> | <span data-ttu-id="96731-108">说明</span><span class="sxs-lookup"><span data-stu-id="96731-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="96731-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="96731-109">lastActionDateTime</span></span> | <span data-ttu-id="96731-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96731-110">DateTimeOffset</span></span> | <span data-ttu-id="96731-111">上一次活动发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="96731-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="96731-112">在计划工序、异步任务启动和操作完成时, 会更新该值。</span><span class="sxs-lookup"><span data-stu-id="96731-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="96731-113">操作</span><span class="sxs-lookup"><span data-stu-id="96731-113">operation</span></span> | <span data-ttu-id="96731-114">String</span><span class="sxs-lookup"><span data-stu-id="96731-114">String</span></span> | <span data-ttu-id="96731-115">异步操作的类型。</span><span class="sxs-lookup"><span data-stu-id="96731-115">Type of asynchronous operation.</span></span> <span data-ttu-id="96731-116">这些值可以是*ForceDelete*或*验证*</span><span class="sxs-lookup"><span data-stu-id="96731-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="96731-117">状态</span><span class="sxs-lookup"><span data-stu-id="96731-117">status</span></span> | <span data-ttu-id="96731-118">字符串</span><span class="sxs-lookup"><span data-stu-id="96731-118">String</span></span> | <span data-ttu-id="96731-119">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="96731-119">Current status of the operation.</span></span> <br> <span data-ttu-id="96731-120">*计划*-操作已计划, 但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="96731-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="96731-121">*InProgress* -任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="96731-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="96731-122">*failed* -操作失败。</span><span class="sxs-lookup"><span data-stu-id="96731-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96731-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96731-123">JSON representation</span></span>
<span data-ttu-id="96731-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96731-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
