---
title: 货币资源类型
description: Dynamics 365 Business Central 中的货币对象
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ba8ad750831394e2a84fab7ca87d76754838db60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012616"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="712e8-103">货币资源类型</span><span class="sxs-lookup"><span data-stu-id="712e8-103">currencies resource type</span></span>
<span data-ttu-id="712e8-104">表示 Dynamics 365 Business Central 中使用的货币。</span><span class="sxs-lookup"><span data-stu-id="712e8-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="712e8-105">方法</span><span class="sxs-lookup"><span data-stu-id="712e8-105">Methods</span></span>
| <span data-ttu-id="712e8-106">方法</span><span class="sxs-lookup"><span data-stu-id="712e8-106">Method</span></span>                                                  |<span data-ttu-id="712e8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="712e8-107">Return Type</span></span>|<span data-ttu-id="712e8-108">说明</span><span class="sxs-lookup"><span data-stu-id="712e8-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="712e8-109">获取货币</span><span class="sxs-lookup"><span data-stu-id="712e8-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="712e8-110">货币</span><span class="sxs-lookup"><span data-stu-id="712e8-110">currencies</span></span> |<span data-ttu-id="712e8-111">获取货币。</span><span class="sxs-lookup"><span data-stu-id="712e8-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="712e8-112">过帐货币</span><span class="sxs-lookup"><span data-stu-id="712e8-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="712e8-113">货币</span><span class="sxs-lookup"><span data-stu-id="712e8-113">currencies</span></span> |<span data-ttu-id="712e8-114">创建货币。</span><span class="sxs-lookup"><span data-stu-id="712e8-114">Create a Currency.</span></span>|
|[<span data-ttu-id="712e8-115">修补程序货币</span><span class="sxs-lookup"><span data-stu-id="712e8-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="712e8-116">货币</span><span class="sxs-lookup"><span data-stu-id="712e8-116">currencies</span></span> |<span data-ttu-id="712e8-117">更新货币。</span><span class="sxs-lookup"><span data-stu-id="712e8-117">Update a Currency.</span></span>|
|[<span data-ttu-id="712e8-118">删除货币</span><span class="sxs-lookup"><span data-stu-id="712e8-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="712e8-119">无</span><span class="sxs-lookup"><span data-stu-id="712e8-119">none</span></span>       |<span data-ttu-id="712e8-120">删除货币。</span><span class="sxs-lookup"><span data-stu-id="712e8-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="712e8-121">属性</span><span class="sxs-lookup"><span data-stu-id="712e8-121">Properties</span></span>
| <span data-ttu-id="712e8-122">属性</span><span class="sxs-lookup"><span data-stu-id="712e8-122">Property</span></span>              | <span data-ttu-id="712e8-123">类型</span><span class="sxs-lookup"><span data-stu-id="712e8-123">Type</span></span>   |<span data-ttu-id="712e8-124">说明</span><span class="sxs-lookup"><span data-stu-id="712e8-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="712e8-125">id</span><span class="sxs-lookup"><span data-stu-id="712e8-125">id</span></span>                     |<span data-ttu-id="712e8-126">GUID</span><span class="sxs-lookup"><span data-stu-id="712e8-126">GUID</span></span>    |<span data-ttu-id="712e8-127">货币的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="712e8-127">The unique ID of the currency.</span></span> <span data-ttu-id="712e8-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="712e8-128">Non-editable.</span></span>                  |
|<span data-ttu-id="712e8-129">code</span><span class="sxs-lookup"><span data-stu-id="712e8-129">code</span></span>                   |<span data-ttu-id="712e8-130">string</span><span class="sxs-lookup"><span data-stu-id="712e8-130">string</span></span>  |<span data-ttu-id="712e8-131">指定货币代码。</span><span class="sxs-lookup"><span data-stu-id="712e8-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="712e8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="712e8-132">displayName</span></span>            |<span data-ttu-id="712e8-133">string</span><span class="sxs-lookup"><span data-stu-id="712e8-133">string</span></span>  |<span data-ttu-id="712e8-134">指定货币显示名称。</span><span class="sxs-lookup"><span data-stu-id="712e8-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="712e8-135">符号</span><span class="sxs-lookup"><span data-stu-id="712e8-135">symbol</span></span>                 |<span data-ttu-id="712e8-136">string</span><span class="sxs-lookup"><span data-stu-id="712e8-136">string</span></span>  |<span data-ttu-id="712e8-137">指定在支票上显示的此货币符号。</span><span class="sxs-lookup"><span data-stu-id="712e8-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="712e8-138">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="712e8-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="712e8-139">string</span><span class="sxs-lookup"><span data-stu-id="712e8-139">string</span></span>  |<span data-ttu-id="712e8-140">指定系统将按此货币的金额显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="712e8-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="712e8-141">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="712e8-141">amountRoundingPrecision</span></span>|<span data-ttu-id="712e8-142">数位</span><span class="sxs-lookup"><span data-stu-id="712e8-142">decimal</span></span> |<span data-ttu-id="712e8-143">指定此货币的舍入金额时要使用的时间间隔的大小。</span><span class="sxs-lookup"><span data-stu-id="712e8-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="712e8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="712e8-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="712e8-145">datetime</span><span class="sxs-lookup"><span data-stu-id="712e8-145">datetime</span></span>|<span data-ttu-id="712e8-146">修改了货币的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="712e8-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="712e8-147">只读。</span><span class="sxs-lookup"><span data-stu-id="712e8-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="712e8-148">关系</span><span class="sxs-lookup"><span data-stu-id="712e8-148">Relationships</span></span>
<span data-ttu-id="712e8-149">无</span><span class="sxs-lookup"><span data-stu-id="712e8-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="712e8-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="712e8-150">JSON representation</span></span>

<span data-ttu-id="712e8-151">下面是货币的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="712e8-151">Here is a JSON representation of the currencies.</span></span>


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

