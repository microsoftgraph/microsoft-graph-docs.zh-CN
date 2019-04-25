---
title: trialBalance 资源类型
description: Dynamics 365 Business Central 中的试算平衡表对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534848"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="d4284-103">trialBalance 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4284-103">trialBalance resource type</span></span>
<span data-ttu-id="d4284-104">表示 Dynamics 365 Business Central 中的试算平衡表。</span><span class="sxs-lookup"><span data-stu-id="d4284-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="d4284-105">方法</span><span class="sxs-lookup"><span data-stu-id="d4284-105">Methods</span></span>

| <span data-ttu-id="d4284-106">方法</span><span class="sxs-lookup"><span data-stu-id="d4284-106">Method</span></span>       | <span data-ttu-id="d4284-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4284-107">Return Type</span></span>  |<span data-ttu-id="d4284-108">说明</span><span class="sxs-lookup"><span data-stu-id="d4284-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4284-109">获取 trialBalance</span><span class="sxs-lookup"><span data-stu-id="d4284-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="d4284-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="d4284-110">trialBalance</span></span>|<span data-ttu-id="d4284-111">获取试算平衡表对象。</span><span class="sxs-lookup"><span data-stu-id="d4284-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4284-112">属性</span><span class="sxs-lookup"><span data-stu-id="d4284-112">Properties</span></span>
| <span data-ttu-id="d4284-113">属性</span><span class="sxs-lookup"><span data-stu-id="d4284-113">Property</span></span>     | <span data-ttu-id="d4284-114">类型</span><span class="sxs-lookup"><span data-stu-id="d4284-114">Type</span></span>   |<span data-ttu-id="d4284-115">说明</span><span class="sxs-lookup"><span data-stu-id="d4284-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4284-116">数字</span><span class="sxs-lookup"><span data-stu-id="d4284-116">number</span></span>|<span data-ttu-id="d4284-117">string</span><span class="sxs-lookup"><span data-stu-id="d4284-117">string</span></span>|<span data-ttu-id="d4284-118">trialBalance 项目的 G/L 帐号</span><span class="sxs-lookup"><span data-stu-id="d4284-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="d4284-119">accountId</span><span class="sxs-lookup"><span data-stu-id="d4284-119">accountId</span></span>|<span data-ttu-id="d4284-120">GUID</span><span class="sxs-lookup"><span data-stu-id="d4284-120">GUID</span></span>|<span data-ttu-id="d4284-121">记录的 G/L 帐户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d4284-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="d4284-122">accountType</span><span class="sxs-lookup"><span data-stu-id="d4284-122">accountType</span></span>|<span data-ttu-id="d4284-123">string</span><span class="sxs-lookup"><span data-stu-id="d4284-123">string</span></span>|<span data-ttu-id="d4284-124">记录的 G/L 帐户的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="d4284-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="d4284-125">显示屏</span><span class="sxs-lookup"><span data-stu-id="d4284-125">display</span></span>|<span data-ttu-id="d4284-126">string</span><span class="sxs-lookup"><span data-stu-id="d4284-126">string</span></span>|<span data-ttu-id="d4284-127">trialBalance 项目的 G/L 帐户名称。</span><span class="sxs-lookup"><span data-stu-id="d4284-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="d4284-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="d4284-128">totalDebit</span></span>|<span data-ttu-id="d4284-129">string</span><span class="sxs-lookup"><span data-stu-id="d4284-129">string</span></span>|<span data-ttu-id="d4284-130">表示在 G/L 帐户中的借方总额。</span><span class="sxs-lookup"><span data-stu-id="d4284-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="d4284-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="d4284-131">totalCredit</span></span>|<span data-ttu-id="d4284-132">string</span><span class="sxs-lookup"><span data-stu-id="d4284-132">string</span></span>|<span data-ttu-id="d4284-133">表示 G/L 帐户中的总贷方金额。</span><span class="sxs-lookup"><span data-stu-id="d4284-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="d4284-134">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="d4284-134">balanceAtDateDebit</span></span>|<span data-ttu-id="d4284-135">string</span><span class="sxs-lookup"><span data-stu-id="d4284-135">string</span></span>|<span data-ttu-id="d4284-136">表示 G/L 帐户中的日期金额的正余额。</span><span class="sxs-lookup"><span data-stu-id="d4284-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="d4284-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="d4284-137">balanceAtDateCredit</span></span>|<span data-ttu-id="d4284-138">string</span><span class="sxs-lookup"><span data-stu-id="d4284-138">string</span></span>|<span data-ttu-id="d4284-139">表示在 G/L 帐户中的日期量为负余额。</span><span class="sxs-lookup"><span data-stu-id="d4284-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="d4284-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="d4284-140">dateFilter</span></span>|<span data-ttu-id="d4284-141">date</span><span class="sxs-lookup"><span data-stu-id="d4284-141">date</span></span>|<span data-ttu-id="d4284-142">用于计算 trialBalance 项目的日期筛选器。</span><span class="sxs-lookup"><span data-stu-id="d4284-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d4284-143">关系</span><span class="sxs-lookup"><span data-stu-id="d4284-143">Relationships</span></span>
<span data-ttu-id="d4284-144">无</span><span class="sxs-lookup"><span data-stu-id="d4284-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4284-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4284-145">JSON representation</span></span>

<span data-ttu-id="d4284-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4284-146">Here is a JSON representation of the resource.</span></span>


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

