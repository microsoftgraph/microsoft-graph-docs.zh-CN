---
title: trialBalance 资源类型
description: Dynamics 365 Business Central 中的试算平衡表对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 02e4f039411c992cd1d7335fc2463d660b8ff181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972871"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="599d5-103">trialBalance 资源类型</span><span class="sxs-lookup"><span data-stu-id="599d5-103">trialBalance resource type</span></span>
<span data-ttu-id="599d5-104">表示 Dynamics 365 Business Central 中的试算平衡表。</span><span class="sxs-lookup"><span data-stu-id="599d5-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="599d5-105">方法</span><span class="sxs-lookup"><span data-stu-id="599d5-105">Methods</span></span>

| <span data-ttu-id="599d5-106">方法</span><span class="sxs-lookup"><span data-stu-id="599d5-106">Method</span></span>       | <span data-ttu-id="599d5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="599d5-107">Return Type</span></span>  |<span data-ttu-id="599d5-108">说明</span><span class="sxs-lookup"><span data-stu-id="599d5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="599d5-109">获取 trialBalance</span><span class="sxs-lookup"><span data-stu-id="599d5-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="599d5-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="599d5-110">trialBalance</span></span>|<span data-ttu-id="599d5-111">获取试算平衡表对象。</span><span class="sxs-lookup"><span data-stu-id="599d5-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="599d5-112">属性</span><span class="sxs-lookup"><span data-stu-id="599d5-112">Properties</span></span>
| <span data-ttu-id="599d5-113">属性</span><span class="sxs-lookup"><span data-stu-id="599d5-113">Property</span></span>     | <span data-ttu-id="599d5-114">类型</span><span class="sxs-lookup"><span data-stu-id="599d5-114">Type</span></span>   |<span data-ttu-id="599d5-115">说明</span><span class="sxs-lookup"><span data-stu-id="599d5-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="599d5-116">number</span><span class="sxs-lookup"><span data-stu-id="599d5-116">number</span></span>|<span data-ttu-id="599d5-117">string</span><span class="sxs-lookup"><span data-stu-id="599d5-117">string</span></span>|<span data-ttu-id="599d5-118">TrialBalance 项目的 G/L 帐号</span><span class="sxs-lookup"><span data-stu-id="599d5-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="599d5-119">accountId</span><span class="sxs-lookup"><span data-stu-id="599d5-119">accountId</span></span>|<span data-ttu-id="599d5-120">GUID</span><span class="sxs-lookup"><span data-stu-id="599d5-120">GUID</span></span>|<span data-ttu-id="599d5-121">记录的 G/L 帐户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="599d5-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="599d5-122">accountType</span><span class="sxs-lookup"><span data-stu-id="599d5-122">accountType</span></span>|<span data-ttu-id="599d5-123">string</span><span class="sxs-lookup"><span data-stu-id="599d5-123">string</span></span>|<span data-ttu-id="599d5-124">记录的 G/L 帐户的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="599d5-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="599d5-125">显示屏</span><span class="sxs-lookup"><span data-stu-id="599d5-125">display</span></span>|<span data-ttu-id="599d5-126">string</span><span class="sxs-lookup"><span data-stu-id="599d5-126">string</span></span>|<span data-ttu-id="599d5-127">TrialBalance 项目的 G/L 帐户名称。</span><span class="sxs-lookup"><span data-stu-id="599d5-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="599d5-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="599d5-128">totalDebit</span></span>|<span data-ttu-id="599d5-129">string</span><span class="sxs-lookup"><span data-stu-id="599d5-129">string</span></span>|<span data-ttu-id="599d5-130">表示在 G/L 帐户中的借方总额。</span><span class="sxs-lookup"><span data-stu-id="599d5-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="599d5-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="599d5-131">totalCredit</span></span>|<span data-ttu-id="599d5-132">string</span><span class="sxs-lookup"><span data-stu-id="599d5-132">string</span></span>|<span data-ttu-id="599d5-133">表示 G/L 帐户中的总贷方金额。</span><span class="sxs-lookup"><span data-stu-id="599d5-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="599d5-134">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="599d5-134">balanceAtDateDebit</span></span>|<span data-ttu-id="599d5-135">string</span><span class="sxs-lookup"><span data-stu-id="599d5-135">string</span></span>|<span data-ttu-id="599d5-136">表示 G/L 帐户中的日期金额的正余额。</span><span class="sxs-lookup"><span data-stu-id="599d5-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="599d5-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="599d5-137">balanceAtDateCredit</span></span>|<span data-ttu-id="599d5-138">string</span><span class="sxs-lookup"><span data-stu-id="599d5-138">string</span></span>|<span data-ttu-id="599d5-139">表示在 G/L 帐户中的日期量为负余额。</span><span class="sxs-lookup"><span data-stu-id="599d5-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="599d5-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="599d5-140">dateFilter</span></span>|<span data-ttu-id="599d5-141">date</span><span class="sxs-lookup"><span data-stu-id="599d5-141">date</span></span>|<span data-ttu-id="599d5-142">用于计算 trialBalance 项目的日期筛选器。</span><span class="sxs-lookup"><span data-stu-id="599d5-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="599d5-143">关系</span><span class="sxs-lookup"><span data-stu-id="599d5-143">Relationships</span></span>
<span data-ttu-id="599d5-144">无</span><span class="sxs-lookup"><span data-stu-id="599d5-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="599d5-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="599d5-145">JSON representation</span></span>

<span data-ttu-id="599d5-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="599d5-146">Here is a JSON representation of the resource.</span></span>


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

