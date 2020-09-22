---
title: trialBalance 资源类型
description: Dynamics 365 Business Central 中的试算平衡表对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 43368ace9a47064833aa388dda0a7da31d9e5f0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040033"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="18ca1-103">trialBalance 资源类型</span><span class="sxs-lookup"><span data-stu-id="18ca1-103">trialBalance resource type</span></span>

<span data-ttu-id="18ca1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18ca1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18ca1-105">表示 Dynamics 365 Business Central 中的试算平衡表。</span><span class="sxs-lookup"><span data-stu-id="18ca1-105">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="18ca1-106">方法</span><span class="sxs-lookup"><span data-stu-id="18ca1-106">Methods</span></span>

| <span data-ttu-id="18ca1-107">方法</span><span class="sxs-lookup"><span data-stu-id="18ca1-107">Method</span></span>       | <span data-ttu-id="18ca1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="18ca1-108">Return Type</span></span>  |<span data-ttu-id="18ca1-109">说明</span><span class="sxs-lookup"><span data-stu-id="18ca1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18ca1-110">获取 trialBalance</span><span class="sxs-lookup"><span data-stu-id="18ca1-110">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="18ca1-111">trialBalance</span><span class="sxs-lookup"><span data-stu-id="18ca1-111">trialBalance</span></span>|<span data-ttu-id="18ca1-112">获取试算平衡表对象。</span><span class="sxs-lookup"><span data-stu-id="18ca1-112">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18ca1-113">属性</span><span class="sxs-lookup"><span data-stu-id="18ca1-113">Properties</span></span>
| <span data-ttu-id="18ca1-114">属性</span><span class="sxs-lookup"><span data-stu-id="18ca1-114">Property</span></span>     | <span data-ttu-id="18ca1-115">类型</span><span class="sxs-lookup"><span data-stu-id="18ca1-115">Type</span></span>   |<span data-ttu-id="18ca1-116">说明</span><span class="sxs-lookup"><span data-stu-id="18ca1-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18ca1-117">数字</span><span class="sxs-lookup"><span data-stu-id="18ca1-117">number</span></span>|<span data-ttu-id="18ca1-118">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-118">string</span></span>|<span data-ttu-id="18ca1-119">TrialBalance 项目的 G/L 帐号</span><span class="sxs-lookup"><span data-stu-id="18ca1-119">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="18ca1-120">accountId</span><span class="sxs-lookup"><span data-stu-id="18ca1-120">accountId</span></span>|<span data-ttu-id="18ca1-121">GUID</span><span class="sxs-lookup"><span data-stu-id="18ca1-121">GUID</span></span>|<span data-ttu-id="18ca1-122">记录的 G/L 帐户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="18ca1-122">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="18ca1-123">accountType</span><span class="sxs-lookup"><span data-stu-id="18ca1-123">accountType</span></span>|<span data-ttu-id="18ca1-124">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-124">string</span></span>|<span data-ttu-id="18ca1-125">记录的 G/L 帐户的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="18ca1-125">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="18ca1-126">显示屏</span><span class="sxs-lookup"><span data-stu-id="18ca1-126">display</span></span>|<span data-ttu-id="18ca1-127">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-127">string</span></span>|<span data-ttu-id="18ca1-128">TrialBalance 项目的 G/L 帐户名称。</span><span class="sxs-lookup"><span data-stu-id="18ca1-128">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="18ca1-129">totalDebit</span><span class="sxs-lookup"><span data-stu-id="18ca1-129">totalDebit</span></span>|<span data-ttu-id="18ca1-130">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-130">string</span></span>|<span data-ttu-id="18ca1-131">表示在 G/L 帐户中的借方总额。</span><span class="sxs-lookup"><span data-stu-id="18ca1-131">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="18ca1-132">totalCredit</span><span class="sxs-lookup"><span data-stu-id="18ca1-132">totalCredit</span></span>|<span data-ttu-id="18ca1-133">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-133">string</span></span>|<span data-ttu-id="18ca1-134">表示 G/L 帐户中的总贷方金额。</span><span class="sxs-lookup"><span data-stu-id="18ca1-134">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="18ca1-135">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="18ca1-135">balanceAtDateDebit</span></span>|<span data-ttu-id="18ca1-136">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-136">string</span></span>|<span data-ttu-id="18ca1-137">表示 G/L 帐户中的日期金额的正余额。</span><span class="sxs-lookup"><span data-stu-id="18ca1-137">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="18ca1-138">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="18ca1-138">balanceAtDateCredit</span></span>|<span data-ttu-id="18ca1-139">string</span><span class="sxs-lookup"><span data-stu-id="18ca1-139">string</span></span>|<span data-ttu-id="18ca1-140">表示在 G/L 帐户中的日期量为负余额。</span><span class="sxs-lookup"><span data-stu-id="18ca1-140">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="18ca1-141">dateFilter</span><span class="sxs-lookup"><span data-stu-id="18ca1-141">dateFilter</span></span>|<span data-ttu-id="18ca1-142">date</span><span class="sxs-lookup"><span data-stu-id="18ca1-142">date</span></span>|<span data-ttu-id="18ca1-143">用于计算 trialBalance 项目的日期筛选器。</span><span class="sxs-lookup"><span data-stu-id="18ca1-143">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="18ca1-144">关系</span><span class="sxs-lookup"><span data-stu-id="18ca1-144">Relationships</span></span>
<span data-ttu-id="18ca1-145">无</span><span class="sxs-lookup"><span data-stu-id="18ca1-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18ca1-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18ca1-146">JSON representation</span></span>

<span data-ttu-id="18ca1-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18ca1-147">Here is a JSON representation of the resource.</span></span>


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



