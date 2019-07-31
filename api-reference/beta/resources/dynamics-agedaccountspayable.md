---
title: agedAccountsPayable 资源类型
description: Dynamics 365 Business Central 中的一个过期的应付帐款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a135627804e2d6c5be4203c0ee0c229642c70c65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973742"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="15bbc-103">agedAccountsPayable 资源类型</span><span class="sxs-lookup"><span data-stu-id="15bbc-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="15bbc-104">代表 Dynamics 365 Business Central 中的 agedAccountsPayable 对象, 它显示供应商帐户的帐龄。</span><span class="sxs-lookup"><span data-stu-id="15bbc-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="15bbc-105">方法</span><span class="sxs-lookup"><span data-stu-id="15bbc-105">Methods</span></span>

| <span data-ttu-id="15bbc-106">方法</span><span class="sxs-lookup"><span data-stu-id="15bbc-106">Method</span></span>         | <span data-ttu-id="15bbc-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="15bbc-107">Return Type</span></span>  |<span data-ttu-id="15bbc-108">说明</span><span class="sxs-lookup"><span data-stu-id="15bbc-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="15bbc-109">获取 agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="15bbc-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="15bbc-110">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="15bbc-110">agedAccountsPayable</span></span>|<span data-ttu-id="15bbc-111">获取 agedAccountsPayable 对象</span><span class="sxs-lookup"><span data-stu-id="15bbc-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="15bbc-112">属性</span><span class="sxs-lookup"><span data-stu-id="15bbc-112">Properties</span></span>
| <span data-ttu-id="15bbc-113">属性</span><span class="sxs-lookup"><span data-stu-id="15bbc-113">Property</span></span>      | <span data-ttu-id="15bbc-114">类型</span><span class="sxs-lookup"><span data-stu-id="15bbc-114">Type</span></span>     |<span data-ttu-id="15bbc-115">说明</span><span class="sxs-lookup"><span data-stu-id="15bbc-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="15bbc-116">vendorId</span><span class="sxs-lookup"><span data-stu-id="15bbc-116">vendorId</span></span>       |<span data-ttu-id="15bbc-117">GUID</span><span class="sxs-lookup"><span data-stu-id="15bbc-117">GUID</span></span>      |<span data-ttu-id="15bbc-118">供应商的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="15bbc-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="15bbc-119">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="15bbc-119">vendorNumber</span></span>   |<span data-ttu-id="15bbc-120">string</span><span class="sxs-lookup"><span data-stu-id="15bbc-120">string</span></span>    |<span data-ttu-id="15bbc-121">指定供应商的编号。</span><span class="sxs-lookup"><span data-stu-id="15bbc-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="15bbc-122">name</span><span class="sxs-lookup"><span data-stu-id="15bbc-122">name</span></span>           |<span data-ttu-id="15bbc-123">string</span><span class="sxs-lookup"><span data-stu-id="15bbc-123">string</span></span>    |<span data-ttu-id="15bbc-124">指定供应商的名称。</span><span class="sxs-lookup"><span data-stu-id="15bbc-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="15bbc-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="15bbc-125">currencyCode</span></span>   |<span data-ttu-id="15bbc-126">string</span><span class="sxs-lookup"><span data-stu-id="15bbc-126">string</span></span>    |<span data-ttu-id="15bbc-127">指定货币。</span><span class="sxs-lookup"><span data-stu-id="15bbc-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="15bbc-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="15bbc-128">balanceDue</span></span>     |<span data-ttu-id="15bbc-129">位数</span><span class="sxs-lookup"><span data-stu-id="15bbc-129">numeric</span></span>   |<span data-ttu-id="15bbc-130">指定供应商到期的总余额。</span><span class="sxs-lookup"><span data-stu-id="15bbc-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="15bbc-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="15bbc-131">currentAmount</span></span>  |<span data-ttu-id="15bbc-132">位数</span><span class="sxs-lookup"><span data-stu-id="15bbc-132">numeric</span></span>   |<span data-ttu-id="15bbc-133">指定在第一个帐龄期间之前的余额。</span><span class="sxs-lookup"><span data-stu-id="15bbc-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="15bbc-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="15bbc-134">period1Amount</span></span>  |<span data-ttu-id="15bbc-135">位数</span><span class="sxs-lookup"><span data-stu-id="15bbc-135">numeric</span></span>   |<span data-ttu-id="15bbc-136">指定第一个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="15bbc-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="15bbc-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="15bbc-137">period2Amount</span></span>  |<span data-ttu-id="15bbc-138">位数</span><span class="sxs-lookup"><span data-stu-id="15bbc-138">numeric</span></span>   |<span data-ttu-id="15bbc-139">指定第二个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="15bbc-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="15bbc-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="15bbc-140">period3Amount</span></span>  |<span data-ttu-id="15bbc-141">位数</span><span class="sxs-lookup"><span data-stu-id="15bbc-141">numeric</span></span>   |<span data-ttu-id="15bbc-142">指定第三个帐龄期间的余额。</span><span class="sxs-lookup"><span data-stu-id="15bbc-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="15bbc-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="15bbc-143">agedAsOfDate</span></span>   |<span data-ttu-id="15bbc-144">date</span><span class="sxs-lookup"><span data-stu-id="15bbc-144">date</span></span>|<span data-ttu-id="15bbc-145">指定用于计算帐龄期间的时间段起始日期。</span><span class="sxs-lookup"><span data-stu-id="15bbc-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="15bbc-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="15bbc-146">periodLengthFilter</span></span>|<span data-ttu-id="15bbc-147">string</span><span class="sxs-lookup"><span data-stu-id="15bbc-147">string</span></span> |<span data-ttu-id="15bbc-148">指定时间段的长度。</span><span class="sxs-lookup"><span data-stu-id="15bbc-148">Specifies the length of the periods.</span></span> <span data-ttu-id="15bbc-149">可接受的时间单位值为: D、WD、W、M、Q 或 Y (即基于日期的当前时间单位) 可以指定为时间单位的前缀。</span><span class="sxs-lookup"><span data-stu-id="15bbc-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="15bbc-150">关系</span><span class="sxs-lookup"><span data-stu-id="15bbc-150">Relationships</span></span>
<span data-ttu-id="15bbc-151">无</span><span class="sxs-lookup"><span data-stu-id="15bbc-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15bbc-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15bbc-152">JSON representation</span></span>

<span data-ttu-id="15bbc-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15bbc-153">Here is a JSON representation of the resource.</span></span>


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
