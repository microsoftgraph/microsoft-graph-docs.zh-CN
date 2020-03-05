---
title: agedAccountsPayable 资源类型
description: Dynamics 365 Business Central 中的一个过期的应付帐款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9a8dc7eed4bdbcc39a04f55996e11b6d9dc6da1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505166"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="82333-103">agedAccountsPayable 资源类型</span><span class="sxs-lookup"><span data-stu-id="82333-103">agedAccountsPayable resource type</span></span>

<span data-ttu-id="82333-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82333-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82333-105">代表 Dynamics 365 Business Central 中的 agedAccountsPayable 对象，它显示供应商帐户的帐龄。</span><span class="sxs-lookup"><span data-stu-id="82333-105">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="82333-106">方法</span><span class="sxs-lookup"><span data-stu-id="82333-106">Methods</span></span>

| <span data-ttu-id="82333-107">方法</span><span class="sxs-lookup"><span data-stu-id="82333-107">Method</span></span>         | <span data-ttu-id="82333-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="82333-108">Return Type</span></span>  |<span data-ttu-id="82333-109">说明</span><span class="sxs-lookup"><span data-stu-id="82333-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="82333-110">获取 agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="82333-110">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="82333-111">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="82333-111">agedAccountsPayable</span></span>|<span data-ttu-id="82333-112">获取 agedAccountsPayable 对象</span><span class="sxs-lookup"><span data-stu-id="82333-112">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="82333-113">属性</span><span class="sxs-lookup"><span data-stu-id="82333-113">Properties</span></span>
| <span data-ttu-id="82333-114">属性</span><span class="sxs-lookup"><span data-stu-id="82333-114">Property</span></span>      | <span data-ttu-id="82333-115">类型</span><span class="sxs-lookup"><span data-stu-id="82333-115">Type</span></span>     |<span data-ttu-id="82333-116">说明</span><span class="sxs-lookup"><span data-stu-id="82333-116">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="82333-117">vendorId</span><span class="sxs-lookup"><span data-stu-id="82333-117">vendorId</span></span>       |<span data-ttu-id="82333-118">GUID</span><span class="sxs-lookup"><span data-stu-id="82333-118">GUID</span></span>      |<span data-ttu-id="82333-119">供应商的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="82333-119">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="82333-120">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="82333-120">vendorNumber</span></span>   |<span data-ttu-id="82333-121">string</span><span class="sxs-lookup"><span data-stu-id="82333-121">string</span></span>    |<span data-ttu-id="82333-122">指定供应商的编号。</span><span class="sxs-lookup"><span data-stu-id="82333-122">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="82333-123">name</span><span class="sxs-lookup"><span data-stu-id="82333-123">name</span></span>           |<span data-ttu-id="82333-124">string</span><span class="sxs-lookup"><span data-stu-id="82333-124">string</span></span>    |<span data-ttu-id="82333-125">指定供应商的名称。</span><span class="sxs-lookup"><span data-stu-id="82333-125">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="82333-126">currencyCode</span><span class="sxs-lookup"><span data-stu-id="82333-126">currencyCode</span></span>   |<span data-ttu-id="82333-127">string</span><span class="sxs-lookup"><span data-stu-id="82333-127">string</span></span>    |<span data-ttu-id="82333-128">指定货币。</span><span class="sxs-lookup"><span data-stu-id="82333-128">Specifies the currency.</span></span>                     |
|<span data-ttu-id="82333-129">balanceDue</span><span class="sxs-lookup"><span data-stu-id="82333-129">balanceDue</span></span>     |<span data-ttu-id="82333-130">位数</span><span class="sxs-lookup"><span data-stu-id="82333-130">numeric</span></span>   |<span data-ttu-id="82333-131">指定供应商到期的总余额。</span><span class="sxs-lookup"><span data-stu-id="82333-131">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="82333-132">currentAmount</span><span class="sxs-lookup"><span data-stu-id="82333-132">currentAmount</span></span>  |<span data-ttu-id="82333-133">位数</span><span class="sxs-lookup"><span data-stu-id="82333-133">numeric</span></span>   |<span data-ttu-id="82333-134">指定在第一个帐龄期间之前的余额。</span><span class="sxs-lookup"><span data-stu-id="82333-134">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="82333-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="82333-135">period1Amount</span></span>  |<span data-ttu-id="82333-136">位数</span><span class="sxs-lookup"><span data-stu-id="82333-136">numeric</span></span>   |<span data-ttu-id="82333-137">指定第一个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="82333-137">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="82333-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="82333-138">period2Amount</span></span>  |<span data-ttu-id="82333-139">位数</span><span class="sxs-lookup"><span data-stu-id="82333-139">numeric</span></span>   |<span data-ttu-id="82333-140">指定第二个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="82333-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="82333-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="82333-141">period3Amount</span></span>  |<span data-ttu-id="82333-142">位数</span><span class="sxs-lookup"><span data-stu-id="82333-142">numeric</span></span>   |<span data-ttu-id="82333-143">指定第三个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="82333-143">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="82333-144">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="82333-144">agedAsOfDate</span></span>   |<span data-ttu-id="82333-145">date</span><span class="sxs-lookup"><span data-stu-id="82333-145">date</span></span>|<span data-ttu-id="82333-146">指定用于计算帐龄期间的时间段起始日期。</span><span class="sxs-lookup"><span data-stu-id="82333-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="82333-147">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="82333-147">periodLengthFilter</span></span>|<span data-ttu-id="82333-148">string</span><span class="sxs-lookup"><span data-stu-id="82333-148">string</span></span> |<span data-ttu-id="82333-149">指定时间段的长度。</span><span class="sxs-lookup"><span data-stu-id="82333-149">Specifies the length of the periods.</span></span> <span data-ttu-id="82333-150">可接受的时间单位值为： D、WD、W、M、Q 或 Y （即基于日期的当前时间单位）可以指定为时间单位的前缀。</span><span class="sxs-lookup"><span data-stu-id="82333-150">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="82333-151">关系</span><span class="sxs-lookup"><span data-stu-id="82333-151">Relationships</span></span>
<span data-ttu-id="82333-152">无</span><span class="sxs-lookup"><span data-stu-id="82333-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82333-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82333-153">JSON representation</span></span>

<span data-ttu-id="82333-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82333-154">Here is a JSON representation of the resource.</span></span>


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
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
