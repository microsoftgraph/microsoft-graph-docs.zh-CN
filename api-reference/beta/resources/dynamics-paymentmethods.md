---
title: paymentMethods 资源类型
description: Dynamics 365 Business Central 中的付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366646"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="b017b-103">paymentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="b017b-103">paymentMethods resource type</span></span>
<span data-ttu-id="b017b-104">代表 Dynamics 365 Business Central 中的付款方式, 如 PayPal、信用卡和银行帐户。</span><span class="sxs-lookup"><span data-stu-id="b017b-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="b017b-105">方法</span><span class="sxs-lookup"><span data-stu-id="b017b-105">Methods</span></span>

| <span data-ttu-id="b017b-106">方法</span><span class="sxs-lookup"><span data-stu-id="b017b-106">Method</span></span>                                                          | <span data-ttu-id="b017b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b017b-107">Return Type</span></span>  |<span data-ttu-id="b017b-108">说明</span><span class="sxs-lookup"><span data-stu-id="b017b-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="b017b-109">获取 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="b017b-110">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-110">paymentMethods</span></span>|<span data-ttu-id="b017b-111">获取付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="b017b-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="b017b-112">Post paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="b017b-113">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-113">paymentMethods</span></span>|<span data-ttu-id="b017b-114">创建付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="b017b-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="b017b-115">修补程序 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="b017b-116">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-116">paymentMethods</span></span>|<span data-ttu-id="b017b-117">更新付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="b017b-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="b017b-118">删除 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="b017b-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="b017b-119">无</span><span class="sxs-lookup"><span data-stu-id="b017b-119">none</span></span>          |<span data-ttu-id="b017b-120">删除付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="b017b-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b017b-121">属性</span><span class="sxs-lookup"><span data-stu-id="b017b-121">Properties</span></span>
| <span data-ttu-id="b017b-122">属性</span><span class="sxs-lookup"><span data-stu-id="b017b-122">Property</span></span>           | <span data-ttu-id="b017b-123">类型</span><span class="sxs-lookup"><span data-stu-id="b017b-123">Type</span></span>   |<span data-ttu-id="b017b-124">说明</span><span class="sxs-lookup"><span data-stu-id="b017b-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="b017b-125">id</span><span class="sxs-lookup"><span data-stu-id="b017b-125">id</span></span>                  |<span data-ttu-id="b017b-126">GUID</span><span class="sxs-lookup"><span data-stu-id="b017b-126">GUID</span></span>    |<span data-ttu-id="b017b-127">paymentMethods 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b017b-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="b017b-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="b017b-128">Non-editable.</span></span>           |
|<span data-ttu-id="b017b-129">code</span><span class="sxs-lookup"><span data-stu-id="b017b-129">code</span></span>                |<span data-ttu-id="b017b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="b017b-130">string</span></span>  |<span data-ttu-id="b017b-131">指定付款方法代码。</span><span class="sxs-lookup"><span data-stu-id="b017b-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="b017b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b017b-132">displayName</span></span>         |<span data-ttu-id="b017b-133">string</span><span class="sxs-lookup"><span data-stu-id="b017b-133">string</span></span>  |<span data-ttu-id="b017b-134">指定付款方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b017b-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="b017b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b017b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b017b-136">datetime</span><span class="sxs-lookup"><span data-stu-id="b017b-136">datetime</span></span>|<span data-ttu-id="b017b-137">上次修改付款方法的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b017b-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="b017b-138">只读。</span><span class="sxs-lookup"><span data-stu-id="b017b-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="b017b-139">关系</span><span class="sxs-lookup"><span data-stu-id="b017b-139">Relationships</span></span>
<span data-ttu-id="b017b-140">无</span><span class="sxs-lookup"><span data-stu-id="b017b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b017b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b017b-141">JSON representation</span></span>

<span data-ttu-id="b017b-142">下面是 paymentMethods 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b017b-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
