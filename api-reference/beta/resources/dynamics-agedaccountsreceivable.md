---
title: agedAccountsReceivable 资源类型
description: Dynamics 365 Business Central 中的已过期的应收帐款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365575"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="f47dd-103">agedAccountsReceivable 资源类型</span><span class="sxs-lookup"><span data-stu-id="f47dd-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="f47dd-104">代表 Dynamics 365 Business Central 中的 agedAccountsReceivable 对象, 它显示客户帐户的帐龄。</span><span class="sxs-lookup"><span data-stu-id="f47dd-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="f47dd-105">方法</span><span class="sxs-lookup"><span data-stu-id="f47dd-105">Methods</span></span>

| <span data-ttu-id="f47dd-106">方法</span><span class="sxs-lookup"><span data-stu-id="f47dd-106">Method</span></span>         | <span data-ttu-id="f47dd-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f47dd-107">Return Type</span></span>  |<span data-ttu-id="f47dd-108">说明</span><span class="sxs-lookup"><span data-stu-id="f47dd-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="f47dd-109">获取 agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="f47dd-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="f47dd-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="f47dd-110">agedAccountsReceivable</span></span>|<span data-ttu-id="f47dd-111">获取 agedAccountsReceivable 对象</span><span class="sxs-lookup"><span data-stu-id="f47dd-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="f47dd-112">属性</span><span class="sxs-lookup"><span data-stu-id="f47dd-112">Properties</span></span>
| <span data-ttu-id="f47dd-113">属性</span><span class="sxs-lookup"><span data-stu-id="f47dd-113">Property</span></span>       | <span data-ttu-id="f47dd-114">类型</span><span class="sxs-lookup"><span data-stu-id="f47dd-114">Type</span></span>    |<span data-ttu-id="f47dd-115">说明</span><span class="sxs-lookup"><span data-stu-id="f47dd-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="f47dd-116">customerId</span><span class="sxs-lookup"><span data-stu-id="f47dd-116">customerId</span></span>      |<span data-ttu-id="f47dd-117">GUID</span><span class="sxs-lookup"><span data-stu-id="f47dd-117">GUID</span></span>     |<span data-ttu-id="f47dd-118">客户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="f47dd-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="f47dd-119">customerNumber</span><span class="sxs-lookup"><span data-stu-id="f47dd-119">customerNumber</span></span>  |<span data-ttu-id="f47dd-120">string</span><span class="sxs-lookup"><span data-stu-id="f47dd-120">string</span></span>   |<span data-ttu-id="f47dd-121">指定 customer 的号码。</span><span class="sxs-lookup"><span data-stu-id="f47dd-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="f47dd-122">name</span><span class="sxs-lookup"><span data-stu-id="f47dd-122">name</span></span>            |<span data-ttu-id="f47dd-123">string</span><span class="sxs-lookup"><span data-stu-id="f47dd-123">string</span></span>   |<span data-ttu-id="f47dd-124">指定客户的名称。</span><span class="sxs-lookup"><span data-stu-id="f47dd-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="f47dd-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="f47dd-125">currencyCode</span></span>    |<span data-ttu-id="f47dd-126">string</span><span class="sxs-lookup"><span data-stu-id="f47dd-126">string</span></span>   |<span data-ttu-id="f47dd-127">指定货币。</span><span class="sxs-lookup"><span data-stu-id="f47dd-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="f47dd-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="f47dd-128">balanceDue</span></span>      |<span data-ttu-id="f47dd-129">位数</span><span class="sxs-lookup"><span data-stu-id="f47dd-129">numeric</span></span>  |<span data-ttu-id="f47dd-130">指定客户的总余额。</span><span class="sxs-lookup"><span data-stu-id="f47dd-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="f47dd-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="f47dd-131">currentAmount</span></span>   |<span data-ttu-id="f47dd-132">位数</span><span class="sxs-lookup"><span data-stu-id="f47dd-132">numeric</span></span>  |<span data-ttu-id="f47dd-133">指定当前帐龄时段的余额。</span><span class="sxs-lookup"><span data-stu-id="f47dd-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="f47dd-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="f47dd-134">period1Amount</span></span>   |<span data-ttu-id="f47dd-135">位数</span><span class="sxs-lookup"><span data-stu-id="f47dd-135">numeric</span></span>  |<span data-ttu-id="f47dd-136">指定第一个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="f47dd-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="f47dd-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="f47dd-137">period2Amount</span></span>   |<span data-ttu-id="f47dd-138">位数</span><span class="sxs-lookup"><span data-stu-id="f47dd-138">numeric</span></span>  |<span data-ttu-id="f47dd-139">指定第二个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="f47dd-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="f47dd-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="f47dd-140">period3Amount</span></span>   |<span data-ttu-id="f47dd-141">位数</span><span class="sxs-lookup"><span data-stu-id="f47dd-141">numeric</span></span>  |<span data-ttu-id="f47dd-142">指定第三个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="f47dd-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="f47dd-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="f47dd-143">agedAsOfDate</span></span>    |<span data-ttu-id="f47dd-144">date</span><span class="sxs-lookup"><span data-stu-id="f47dd-144">date</span></span>     |<span data-ttu-id="f47dd-145">指定用于计算帐龄期间的时间段起始日期。</span><span class="sxs-lookup"><span data-stu-id="f47dd-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="f47dd-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="f47dd-146">periodLengthFilter</span></span>|<span data-ttu-id="f47dd-147">string</span><span class="sxs-lookup"><span data-stu-id="f47dd-147">string</span></span> |<span data-ttu-id="f47dd-148">指定时间段的长度。</span><span class="sxs-lookup"><span data-stu-id="f47dd-148">Specifies the length of the periods.</span></span> <span data-ttu-id="f47dd-149">可接受的时间单位包括: D、WD、W、M、Q 和 Y (意味着当前时间单位基于日期) 可以指定为时间单位的前缀。</span><span class="sxs-lookup"><span data-stu-id="f47dd-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f47dd-150">关系</span><span class="sxs-lookup"><span data-stu-id="f47dd-150">Relationships</span></span>
<span data-ttu-id="f47dd-151">无</span><span class="sxs-lookup"><span data-stu-id="f47dd-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f47dd-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f47dd-152">JSON representation</span></span>

<span data-ttu-id="f47dd-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f47dd-153">Here is a JSON representation of the resource.</span></span>


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


