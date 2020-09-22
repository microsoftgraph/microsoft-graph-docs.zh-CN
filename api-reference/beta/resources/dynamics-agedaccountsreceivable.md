---
title: agedAccountsReceivable 资源类型
description: Dynamics 365 Business Central 中的已过期的应收帐款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 4d56e954e39bae22db07e025f9570f1fe7a92280
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040054"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="6135e-103">agedAccountsReceivable 资源类型</span><span class="sxs-lookup"><span data-stu-id="6135e-103">agedAccountsReceivable resource type</span></span>

<span data-ttu-id="6135e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6135e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6135e-105">代表 Dynamics 365 Business Central 中的 agedAccountsReceivable 对象，它显示客户帐户的帐龄。</span><span class="sxs-lookup"><span data-stu-id="6135e-105">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="6135e-106">方法</span><span class="sxs-lookup"><span data-stu-id="6135e-106">Methods</span></span>

| <span data-ttu-id="6135e-107">方法</span><span class="sxs-lookup"><span data-stu-id="6135e-107">Method</span></span>         | <span data-ttu-id="6135e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6135e-108">Return Type</span></span>  |<span data-ttu-id="6135e-109">说明</span><span class="sxs-lookup"><span data-stu-id="6135e-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="6135e-110">获取 agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="6135e-110">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="6135e-111">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="6135e-111">agedAccountsReceivable</span></span>|<span data-ttu-id="6135e-112">获取 agedAccountsReceivable 对象</span><span class="sxs-lookup"><span data-stu-id="6135e-112">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="6135e-113">属性</span><span class="sxs-lookup"><span data-stu-id="6135e-113">Properties</span></span>
| <span data-ttu-id="6135e-114">属性</span><span class="sxs-lookup"><span data-stu-id="6135e-114">Property</span></span>       | <span data-ttu-id="6135e-115">类型</span><span class="sxs-lookup"><span data-stu-id="6135e-115">Type</span></span>    |<span data-ttu-id="6135e-116">说明</span><span class="sxs-lookup"><span data-stu-id="6135e-116">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="6135e-117">customerId</span><span class="sxs-lookup"><span data-stu-id="6135e-117">customerId</span></span>      |<span data-ttu-id="6135e-118">GUID</span><span class="sxs-lookup"><span data-stu-id="6135e-118">GUID</span></span>     |<span data-ttu-id="6135e-119">客户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6135e-119">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="6135e-120">customerNumber</span><span class="sxs-lookup"><span data-stu-id="6135e-120">customerNumber</span></span>  |<span data-ttu-id="6135e-121">string</span><span class="sxs-lookup"><span data-stu-id="6135e-121">string</span></span>   |<span data-ttu-id="6135e-122">指定 customer 的号码。</span><span class="sxs-lookup"><span data-stu-id="6135e-122">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="6135e-123">name</span><span class="sxs-lookup"><span data-stu-id="6135e-123">name</span></span>            |<span data-ttu-id="6135e-124">string</span><span class="sxs-lookup"><span data-stu-id="6135e-124">string</span></span>   |<span data-ttu-id="6135e-125">指定客户的名称。</span><span class="sxs-lookup"><span data-stu-id="6135e-125">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="6135e-126">currencyCode</span><span class="sxs-lookup"><span data-stu-id="6135e-126">currencyCode</span></span>    |<span data-ttu-id="6135e-127">string</span><span class="sxs-lookup"><span data-stu-id="6135e-127">string</span></span>   |<span data-ttu-id="6135e-128">指定货币。</span><span class="sxs-lookup"><span data-stu-id="6135e-128">Specifies the currency.</span></span>                      |
|<span data-ttu-id="6135e-129">balanceDue</span><span class="sxs-lookup"><span data-stu-id="6135e-129">balanceDue</span></span>      |<span data-ttu-id="6135e-130">位数</span><span class="sxs-lookup"><span data-stu-id="6135e-130">numeric</span></span>  |<span data-ttu-id="6135e-131">指定客户的总余额。</span><span class="sxs-lookup"><span data-stu-id="6135e-131">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="6135e-132">currentAmount</span><span class="sxs-lookup"><span data-stu-id="6135e-132">currentAmount</span></span>   |<span data-ttu-id="6135e-133">位数</span><span class="sxs-lookup"><span data-stu-id="6135e-133">numeric</span></span>  |<span data-ttu-id="6135e-134">指定当前帐龄时段的余额。</span><span class="sxs-lookup"><span data-stu-id="6135e-134">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="6135e-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="6135e-135">period1Amount</span></span>   |<span data-ttu-id="6135e-136">位数</span><span class="sxs-lookup"><span data-stu-id="6135e-136">numeric</span></span>  |<span data-ttu-id="6135e-137">指定第一个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="6135e-137">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="6135e-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="6135e-138">period2Amount</span></span>   |<span data-ttu-id="6135e-139">位数</span><span class="sxs-lookup"><span data-stu-id="6135e-139">numeric</span></span>  |<span data-ttu-id="6135e-140">指定第二个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="6135e-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="6135e-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="6135e-141">period3Amount</span></span>   |<span data-ttu-id="6135e-142">位数</span><span class="sxs-lookup"><span data-stu-id="6135e-142">numeric</span></span>  |<span data-ttu-id="6135e-143">指定第三个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="6135e-143">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="6135e-144">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="6135e-144">agedAsOfDate</span></span>    |<span data-ttu-id="6135e-145">date</span><span class="sxs-lookup"><span data-stu-id="6135e-145">date</span></span>     |<span data-ttu-id="6135e-146">指定用于计算帐龄期间的时间段起始日期。</span><span class="sxs-lookup"><span data-stu-id="6135e-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="6135e-147">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="6135e-147">periodLengthFilter</span></span>|<span data-ttu-id="6135e-148">string</span><span class="sxs-lookup"><span data-stu-id="6135e-148">string</span></span> |<span data-ttu-id="6135e-149">指定时间段的长度。</span><span class="sxs-lookup"><span data-stu-id="6135e-149">Specifies the length of the periods.</span></span> <span data-ttu-id="6135e-150">可接受的时间单位包括： D、WD、W、M、Q 和 Y （意味着当前时间单位基于日期）可以指定为时间单位的前缀。</span><span class="sxs-lookup"><span data-stu-id="6135e-150">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="6135e-151">关系</span><span class="sxs-lookup"><span data-stu-id="6135e-151">Relationships</span></span>
<span data-ttu-id="6135e-152">无</span><span class="sxs-lookup"><span data-stu-id="6135e-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6135e-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6135e-153">JSON representation</span></span>

<span data-ttu-id="6135e-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6135e-154">Here is a JSON representation of the resource.</span></span>


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```




