---
title: 货币资源类型
description: Dynamics 365 Business Central 中的货币对象
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543068"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="8d603-103">货币资源类型</span><span class="sxs-lookup"><span data-stu-id="8d603-103">currencies resource type</span></span>
<span data-ttu-id="8d603-104">表示 Dynamics 365 Business Central 中使用的货币。</span><span class="sxs-lookup"><span data-stu-id="8d603-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8d603-105">方法</span><span class="sxs-lookup"><span data-stu-id="8d603-105">Methods</span></span>
| <span data-ttu-id="8d603-106">方法</span><span class="sxs-lookup"><span data-stu-id="8d603-106">Method</span></span>                                                  |<span data-ttu-id="8d603-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d603-107">Return Type</span></span>|<span data-ttu-id="8d603-108">说明</span><span class="sxs-lookup"><span data-stu-id="8d603-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="8d603-109">获取货币</span><span class="sxs-lookup"><span data-stu-id="8d603-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="8d603-110">货币</span><span class="sxs-lookup"><span data-stu-id="8d603-110">currencies</span></span> |<span data-ttu-id="8d603-111">获取货币。</span><span class="sxs-lookup"><span data-stu-id="8d603-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="8d603-112">过帐货币</span><span class="sxs-lookup"><span data-stu-id="8d603-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="8d603-113">货币</span><span class="sxs-lookup"><span data-stu-id="8d603-113">currencies</span></span> |<span data-ttu-id="8d603-114">创建货币。</span><span class="sxs-lookup"><span data-stu-id="8d603-114">Create a Currency.</span></span>|
|[<span data-ttu-id="8d603-115">修补程序货币</span><span class="sxs-lookup"><span data-stu-id="8d603-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="8d603-116">货币</span><span class="sxs-lookup"><span data-stu-id="8d603-116">currencies</span></span> |<span data-ttu-id="8d603-117">更新货币。</span><span class="sxs-lookup"><span data-stu-id="8d603-117">Update a Currency.</span></span>|
|[<span data-ttu-id="8d603-118">删除货币</span><span class="sxs-lookup"><span data-stu-id="8d603-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="8d603-119">无</span><span class="sxs-lookup"><span data-stu-id="8d603-119">none</span></span>       |<span data-ttu-id="8d603-120">删除货币。</span><span class="sxs-lookup"><span data-stu-id="8d603-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d603-121">属性</span><span class="sxs-lookup"><span data-stu-id="8d603-121">Properties</span></span>
| <span data-ttu-id="8d603-122">属性</span><span class="sxs-lookup"><span data-stu-id="8d603-122">Property</span></span>              | <span data-ttu-id="8d603-123">类型</span><span class="sxs-lookup"><span data-stu-id="8d603-123">Type</span></span>   |<span data-ttu-id="8d603-124">说明</span><span class="sxs-lookup"><span data-stu-id="8d603-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="8d603-125">id</span><span class="sxs-lookup"><span data-stu-id="8d603-125">id</span></span>                     |<span data-ttu-id="8d603-126">GUID</span><span class="sxs-lookup"><span data-stu-id="8d603-126">GUID</span></span>    |<span data-ttu-id="8d603-127">货币的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8d603-127">The unique ID of the currency.</span></span> <span data-ttu-id="8d603-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="8d603-128">Non-editable.</span></span>                  |
|<span data-ttu-id="8d603-129">code</span><span class="sxs-lookup"><span data-stu-id="8d603-129">code</span></span>                   |<span data-ttu-id="8d603-130">string</span><span class="sxs-lookup"><span data-stu-id="8d603-130">string</span></span>  |<span data-ttu-id="8d603-131">指定货币代码。</span><span class="sxs-lookup"><span data-stu-id="8d603-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="8d603-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8d603-132">displayName</span></span>            |<span data-ttu-id="8d603-133">string</span><span class="sxs-lookup"><span data-stu-id="8d603-133">string</span></span>  |<span data-ttu-id="8d603-134">指定货币显示名称。</span><span class="sxs-lookup"><span data-stu-id="8d603-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="8d603-135">符号</span><span class="sxs-lookup"><span data-stu-id="8d603-135">symbol</span></span>                 |<span data-ttu-id="8d603-136">string</span><span class="sxs-lookup"><span data-stu-id="8d603-136">string</span></span>  |<span data-ttu-id="8d603-137">指定在支票上显示的此货币符号。</span><span class="sxs-lookup"><span data-stu-id="8d603-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="8d603-138">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="8d603-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="8d603-139">string</span><span class="sxs-lookup"><span data-stu-id="8d603-139">string</span></span>  |<span data-ttu-id="8d603-140">指定系统将按此货币的金额显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="8d603-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="8d603-141">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="8d603-141">amountRoundingPrecision</span></span>|<span data-ttu-id="8d603-142">数位</span><span class="sxs-lookup"><span data-stu-id="8d603-142">decimal</span></span> |<span data-ttu-id="8d603-143">指定此货币的舍入金额时要使用的时间间隔的大小。</span><span class="sxs-lookup"><span data-stu-id="8d603-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="8d603-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d603-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="8d603-145">datetime</span><span class="sxs-lookup"><span data-stu-id="8d603-145">datetime</span></span>|<span data-ttu-id="8d603-146">修改了货币的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8d603-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="8d603-147">只读。</span><span class="sxs-lookup"><span data-stu-id="8d603-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="8d603-148">关系</span><span class="sxs-lookup"><span data-stu-id="8d603-148">Relationships</span></span>
<span data-ttu-id="8d603-149">无</span><span class="sxs-lookup"><span data-stu-id="8d603-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d603-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d603-150">JSON representation</span></span>

<span data-ttu-id="8d603-151">下面是货币的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d603-151">Here is a JSON representation of the currencies.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

