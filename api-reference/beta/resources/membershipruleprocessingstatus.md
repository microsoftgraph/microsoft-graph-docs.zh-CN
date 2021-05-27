---
title: membershipRuleProcessingStatus 资源类型
description: 表示动态组处理的当前状态。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c86f044517ad7b808db69364413727c8d76f076
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680995"
---
# <a name="membershipruleprocessingstatus-resource-type"></a><span data-ttu-id="2f495-103">membershipRuleProcessingStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f495-103">membershipRuleProcessingStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f495-104">表示动态组处理的当前状态。</span><span class="sxs-lookup"><span data-stu-id="2f495-104">Represents the current status of dynamic group processing.</span></span>

## <a name="properties"></a><span data-ttu-id="2f495-105">属性</span><span class="sxs-lookup"><span data-stu-id="2f495-105">Properties</span></span>

| <span data-ttu-id="2f495-106">属性</span><span class="sxs-lookup"><span data-stu-id="2f495-106">Property</span></span> | <span data-ttu-id="2f495-107">类型</span><span class="sxs-lookup"><span data-stu-id="2f495-107">Type</span></span> | <span data-ttu-id="2f495-108">说明</span><span class="sxs-lookup"><span data-stu-id="2f495-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="2f495-109">状态</span><span class="sxs-lookup"><span data-stu-id="2f495-109">status</span></span> | [<span data-ttu-id="2f495-110">membershipRuleProcessingStatusDetails</span><span class="sxs-lookup"><span data-stu-id="2f495-110">membershipRuleProcessingStatusDetails</span></span>](#membershipruleprocessingstatusdetails-values) | <span data-ttu-id="2f495-111">动态组处理的当前状态。</span><span class="sxs-lookup"><span data-stu-id="2f495-111">Current status of a dynamic group processing.</span></span> <span data-ttu-id="2f495-112">可能的值是 `NotStarted` `Running` `Succeeded` ：、、、 `Failed` 和 `UnknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="2f495-112">Possible values are: `NotStarted`, `Running`, `Succeeded`, `Failed`, and `UnknownFutureValue`.</span></span>  <br><br> <span data-ttu-id="2f495-113">必需。</span><span class="sxs-lookup"><span data-stu-id="2f495-113">Required.</span></span> <span data-ttu-id="2f495-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2f495-114">Read-only.</span></span>|
| <span data-ttu-id="2f495-115">lastMembershipUpdated</span><span class="sxs-lookup"><span data-stu-id="2f495-115">lastMembershipUpdated</span></span> | <span data-ttu-id="2f495-116">edm。DateTime</span><span class="sxs-lookup"><span data-stu-id="2f495-116">edm.DateTime</span></span> | <span data-ttu-id="2f495-117">更新动态组的成员身份的最近日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f495-117">Most recent date and time when membership of a dynamic group was updated.</span></span> <br><br> <span data-ttu-id="2f495-118">可选。</span><span class="sxs-lookup"><span data-stu-id="2f495-118">Optional.</span></span> <span data-ttu-id="2f495-119">只读。</span><span class="sxs-lookup"><span data-stu-id="2f495-119">Read-only.</span></span>|
| <span data-ttu-id="2f495-120">errorMessage</span><span class="sxs-lookup"><span data-stu-id="2f495-120">errorMessage</span></span> | <span data-ttu-id="2f495-121">String</span><span class="sxs-lookup"><span data-stu-id="2f495-121">String</span></span> | <span data-ttu-id="2f495-122">动态组处理出现错误时的详细错误消息。</span><span class="sxs-lookup"><span data-stu-id="2f495-122">Detailed error message if dynamic group processing ran into an error.</span></span> <br><br> <span data-ttu-id="2f495-123">可选。</span><span class="sxs-lookup"><span data-stu-id="2f495-123">Optional.</span></span> <span data-ttu-id="2f495-124">只读。</span><span class="sxs-lookup"><span data-stu-id="2f495-124">Read-only.</span></span>|

### <a name="membershipruleprocessingstatusdetails-values"></a><span data-ttu-id="2f495-125">membershipRuleProcessingStatusDetails 值</span><span class="sxs-lookup"><span data-stu-id="2f495-125">membershipRuleProcessingStatusDetails values</span></span>

| <span data-ttu-id="2f495-126">成员</span><span class="sxs-lookup"><span data-stu-id="2f495-126">Member</span></span> | <span data-ttu-id="2f495-127">说明</span><span class="sxs-lookup"><span data-stu-id="2f495-127">Description</span></span> |
|:-------- |:----------- |
| <span data-ttu-id="2f495-128">NotStarted</span><span class="sxs-lookup"><span data-stu-id="2f495-128">NotStarted</span></span> | <span data-ttu-id="2f495-129">已创建或更新组，并等待处理。</span><span class="sxs-lookup"><span data-stu-id="2f495-129">Group has been created or updated, and awaiting processing.</span></span>|
| <span data-ttu-id="2f495-130">正在运行</span><span class="sxs-lookup"><span data-stu-id="2f495-130">Running</span></span> | <span data-ttu-id="2f495-131">处理已开始。</span><span class="sxs-lookup"><span data-stu-id="2f495-131">Processing has started.</span></span>|
| <span data-ttu-id="2f495-132">Succeeded</span><span class="sxs-lookup"><span data-stu-id="2f495-132">Succeeded</span></span> | <span data-ttu-id="2f495-133">处理已完成。</span><span class="sxs-lookup"><span data-stu-id="2f495-133">Processing has completed.</span></span> <span data-ttu-id="2f495-134">增量对象更改将永久处理。</span><span class="sxs-lookup"><span data-stu-id="2f495-134">Incremental object changes are processed perpetually.</span></span> |
| <span data-ttu-id="2f495-135">已失败</span><span class="sxs-lookup"><span data-stu-id="2f495-135">Failed</span></span> | <span data-ttu-id="2f495-136">处理出现错误。</span><span class="sxs-lookup"><span data-stu-id="2f495-136">Processing ran into an error.</span></span> <span data-ttu-id="2f495-137">有关详细信息 **，请参阅 errorMessage。**</span><span class="sxs-lookup"><span data-stu-id="2f495-137">See **errorMessage** for details.</span></span> |
| <span data-ttu-id="2f495-138">UnknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="2f495-138">UnknownFutureValue</span></span> | <span data-ttu-id="2f495-139">支持未来值。</span><span class="sxs-lookup"><span data-stu-id="2f495-139">Supports future values.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f495-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f495-140">JSON representation</span></span>

<span data-ttu-id="2f495-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f495-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.membershipRuleProcessingStatus",
  "baseType": null
}-->

```json
{
  "status": "string",
  "lastMembershipUpdated": "DateTime",
  "errorMessage": "string"
}
```
