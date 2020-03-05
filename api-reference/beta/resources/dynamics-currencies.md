---
title: 货币资源类型
description: Dynamics 365 Business Central 中的货币对象
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e986777d277e84246104561e5e275d7508b41b7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504732"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="3c8f4-103">货币资源类型</span><span class="sxs-lookup"><span data-stu-id="3c8f4-103">currencies resource type</span></span>

<span data-ttu-id="3c8f4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3c8f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c8f4-105">表示 Dynamics 365 Business Central 中使用的货币。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-105">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="3c8f4-106">方法</span><span class="sxs-lookup"><span data-stu-id="3c8f4-106">Methods</span></span>
| <span data-ttu-id="3c8f4-107">方法</span><span class="sxs-lookup"><span data-stu-id="3c8f4-107">Method</span></span>                                                  |<span data-ttu-id="3c8f4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c8f4-108">Return Type</span></span>|<span data-ttu-id="3c8f4-109">说明</span><span class="sxs-lookup"><span data-stu-id="3c8f4-109">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="3c8f4-110">获取货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-110">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="3c8f4-111">货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-111">currencies</span></span> |<span data-ttu-id="3c8f4-112">获取货币。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-112">Get a Currency.</span></span>   |
|[<span data-ttu-id="3c8f4-113">过帐货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-113">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="3c8f4-114">货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-114">currencies</span></span> |<span data-ttu-id="3c8f4-115">创建货币。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-115">Create a Currency.</span></span>|
|[<span data-ttu-id="3c8f4-116">修补程序货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-116">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="3c8f4-117">货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-117">currencies</span></span> |<span data-ttu-id="3c8f4-118">更新货币。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-118">Update a Currency.</span></span>|
|[<span data-ttu-id="3c8f4-119">删除货币</span><span class="sxs-lookup"><span data-stu-id="3c8f4-119">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="3c8f4-120">无</span><span class="sxs-lookup"><span data-stu-id="3c8f4-120">none</span></span>       |<span data-ttu-id="3c8f4-121">删除货币。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-121">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c8f4-122">属性</span><span class="sxs-lookup"><span data-stu-id="3c8f4-122">Properties</span></span>
| <span data-ttu-id="3c8f4-123">属性</span><span class="sxs-lookup"><span data-stu-id="3c8f4-123">Property</span></span>              | <span data-ttu-id="3c8f4-124">类型</span><span class="sxs-lookup"><span data-stu-id="3c8f4-124">Type</span></span>   |<span data-ttu-id="3c8f4-125">说明</span><span class="sxs-lookup"><span data-stu-id="3c8f4-125">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="3c8f4-126">id</span><span class="sxs-lookup"><span data-stu-id="3c8f4-126">id</span></span>                     |<span data-ttu-id="3c8f4-127">GUID</span><span class="sxs-lookup"><span data-stu-id="3c8f4-127">GUID</span></span>    |<span data-ttu-id="3c8f4-128">货币的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-128">The unique ID of the currency.</span></span> <span data-ttu-id="3c8f4-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-129">Non-editable.</span></span>                  |
|<span data-ttu-id="3c8f4-130">code</span><span class="sxs-lookup"><span data-stu-id="3c8f4-130">code</span></span>                   |<span data-ttu-id="3c8f4-131">string</span><span class="sxs-lookup"><span data-stu-id="3c8f4-131">string</span></span>  |<span data-ttu-id="3c8f4-132">指定货币代码。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-132">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="3c8f4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3c8f4-133">displayName</span></span>            |<span data-ttu-id="3c8f4-134">string</span><span class="sxs-lookup"><span data-stu-id="3c8f4-134">string</span></span>  |<span data-ttu-id="3c8f4-135">指定货币显示名称。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-135">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="3c8f4-136">符号</span><span class="sxs-lookup"><span data-stu-id="3c8f4-136">symbol</span></span>                 |<span data-ttu-id="3c8f4-137">string</span><span class="sxs-lookup"><span data-stu-id="3c8f4-137">string</span></span>  |<span data-ttu-id="3c8f4-138">指定在支票上显示的此货币符号。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-138">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="3c8f4-139">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="3c8f4-139">amountDecimalPlaces</span></span>    |<span data-ttu-id="3c8f4-140">string</span><span class="sxs-lookup"><span data-stu-id="3c8f4-140">string</span></span>  |<span data-ttu-id="3c8f4-141">指定系统将按此货币的金额显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-141">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="3c8f4-142">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="3c8f4-142">amountRoundingPrecision</span></span>|<span data-ttu-id="3c8f4-143">数位</span><span class="sxs-lookup"><span data-stu-id="3c8f4-143">decimal</span></span> |<span data-ttu-id="3c8f4-144">指定此货币的舍入金额时要使用的时间间隔的大小。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-144">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="3c8f4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c8f4-145">lastModifiedDateTime</span></span>   |<span data-ttu-id="3c8f4-146">datetime</span><span class="sxs-lookup"><span data-stu-id="3c8f4-146">datetime</span></span>|<span data-ttu-id="3c8f4-147">修改了货币的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-147">The last datetime the currency was modified.</span></span> <span data-ttu-id="3c8f4-148">只读。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-148">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="3c8f4-149">关系</span><span class="sxs-lookup"><span data-stu-id="3c8f4-149">Relationships</span></span>
<span data-ttu-id="3c8f4-150">无</span><span class="sxs-lookup"><span data-stu-id="3c8f4-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c8f4-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c8f4-151">JSON representation</span></span>

<span data-ttu-id="3c8f4-152">下面是货币的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c8f4-152">Here is a JSON representation of the currencies.</span></span>


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

