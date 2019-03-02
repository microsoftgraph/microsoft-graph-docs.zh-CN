---
title: trialBalance 资源类型
description: Dynamics 365 Business Central 中的试算平衡表对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365323"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="e185e-103">trialBalance 资源类型</span><span class="sxs-lookup"><span data-stu-id="e185e-103">trialBalance resource type</span></span>
<span data-ttu-id="e185e-104">表示 Dynamics 365 Business Central 中的试算平衡表。</span><span class="sxs-lookup"><span data-stu-id="e185e-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e185e-105">方法</span><span class="sxs-lookup"><span data-stu-id="e185e-105">Methods</span></span>

| <span data-ttu-id="e185e-106">方法</span><span class="sxs-lookup"><span data-stu-id="e185e-106">Method</span></span>       | <span data-ttu-id="e185e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e185e-107">Return Type</span></span>  |<span data-ttu-id="e185e-108">说明</span><span class="sxs-lookup"><span data-stu-id="e185e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e185e-109">获取 trialBalance</span><span class="sxs-lookup"><span data-stu-id="e185e-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="e185e-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="e185e-110">trialBalance</span></span>|<span data-ttu-id="e185e-111">获取试算平衡表对象。</span><span class="sxs-lookup"><span data-stu-id="e185e-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e185e-112">属性</span><span class="sxs-lookup"><span data-stu-id="e185e-112">Properties</span></span>
| <span data-ttu-id="e185e-113">属性</span><span class="sxs-lookup"><span data-stu-id="e185e-113">Property</span></span>     | <span data-ttu-id="e185e-114">类型</span><span class="sxs-lookup"><span data-stu-id="e185e-114">Type</span></span>   |<span data-ttu-id="e185e-115">说明</span><span class="sxs-lookup"><span data-stu-id="e185e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e185e-116">number</span><span class="sxs-lookup"><span data-stu-id="e185e-116">number</span></span>|<span data-ttu-id="e185e-117">string</span><span class="sxs-lookup"><span data-stu-id="e185e-117">string</span></span>|<span data-ttu-id="e185e-118">trialBalance 项目的 G/L 帐号</span><span class="sxs-lookup"><span data-stu-id="e185e-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="e185e-119">accountId</span><span class="sxs-lookup"><span data-stu-id="e185e-119">accountId</span></span>|<span data-ttu-id="e185e-120">GUID</span><span class="sxs-lookup"><span data-stu-id="e185e-120">GUID</span></span>|<span data-ttu-id="e185e-121">记录的 G/L 帐户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e185e-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="e185e-122">accountType</span><span class="sxs-lookup"><span data-stu-id="e185e-122">accountType</span></span>|<span data-ttu-id="e185e-123">string</span><span class="sxs-lookup"><span data-stu-id="e185e-123">string</span></span>|<span data-ttu-id="e185e-124">记录的 G/L 帐户的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="e185e-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="e185e-125">显示屏</span><span class="sxs-lookup"><span data-stu-id="e185e-125">display</span></span>|<span data-ttu-id="e185e-126">string</span><span class="sxs-lookup"><span data-stu-id="e185e-126">string</span></span>|<span data-ttu-id="e185e-127">trialBalance 项目的 G/L 帐户名称。</span><span class="sxs-lookup"><span data-stu-id="e185e-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="e185e-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="e185e-128">totalDebit</span></span>|<span data-ttu-id="e185e-129">string</span><span class="sxs-lookup"><span data-stu-id="e185e-129">string</span></span>|<span data-ttu-id="e185e-130">表示在 G/L 帐户中的借方总额。</span><span class="sxs-lookup"><span data-stu-id="e185e-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="e185e-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="e185e-131">totalCredit</span></span>|<span data-ttu-id="e185e-132">string</span><span class="sxs-lookup"><span data-stu-id="e185e-132">string</span></span>|<span data-ttu-id="e185e-133">表示 G/L 帐户中的总贷方金额。</span><span class="sxs-lookup"><span data-stu-id="e185e-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="e185e-134">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="e185e-134">balanceAtDateDebit</span></span>|<span data-ttu-id="e185e-135">string</span><span class="sxs-lookup"><span data-stu-id="e185e-135">string</span></span>|<span data-ttu-id="e185e-136">表示 G/L 帐户中的日期金额的正余额。</span><span class="sxs-lookup"><span data-stu-id="e185e-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="e185e-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="e185e-137">balanceAtDateCredit</span></span>|<span data-ttu-id="e185e-138">string</span><span class="sxs-lookup"><span data-stu-id="e185e-138">string</span></span>|<span data-ttu-id="e185e-139">表示在 G/L 帐户中的日期量为负余额。</span><span class="sxs-lookup"><span data-stu-id="e185e-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="e185e-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="e185e-140">dateFilter</span></span>|<span data-ttu-id="e185e-141">date</span><span class="sxs-lookup"><span data-stu-id="e185e-141">date</span></span>|<span data-ttu-id="e185e-142">用于计算 trialBalance 项目的日期筛选器。</span><span class="sxs-lookup"><span data-stu-id="e185e-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e185e-143">关系</span><span class="sxs-lookup"><span data-stu-id="e185e-143">Relationships</span></span>
<span data-ttu-id="e185e-144">无</span><span class="sxs-lookup"><span data-stu-id="e185e-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e185e-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e185e-145">JSON representation</span></span>

<span data-ttu-id="e185e-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e185e-146">Here is a JSON representation of the resource.</span></span>


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

