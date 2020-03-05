---
title: paymentMethods 资源类型
description: Dynamics 365 Business Central 中的付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d72ac6ec655e15ad6f3c824dc2d5e9c3e09db0c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503647"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="d6fa9-103">paymentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6fa9-103">paymentMethods resource type</span></span>

<span data-ttu-id="d6fa9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d6fa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6fa9-105">代表 Dynamics 365 Business Central 中的付款方式，如 PayPal、信用卡和银行帐户。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-105">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="d6fa9-106">方法</span><span class="sxs-lookup"><span data-stu-id="d6fa9-106">Methods</span></span>

| <span data-ttu-id="d6fa9-107">方法</span><span class="sxs-lookup"><span data-stu-id="d6fa9-107">Method</span></span>                                                          | <span data-ttu-id="d6fa9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6fa9-108">Return Type</span></span>  |<span data-ttu-id="d6fa9-109">说明</span><span class="sxs-lookup"><span data-stu-id="d6fa9-109">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="d6fa9-110">获取 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-110">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="d6fa9-111">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-111">paymentMethods</span></span>|<span data-ttu-id="d6fa9-112">获取付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-112">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="d6fa9-113">Post paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-113">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="d6fa9-114">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-114">paymentMethods</span></span>|<span data-ttu-id="d6fa9-115">创建付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-115">Creates a payment method object.</span></span>|
|[<span data-ttu-id="d6fa9-116">修补程序 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-116">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="d6fa9-117">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-117">paymentMethods</span></span>|<span data-ttu-id="d6fa9-118">更新付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-118">Updates a payment method object.</span></span>|
|[<span data-ttu-id="d6fa9-119">删除 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d6fa9-119">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="d6fa9-120">无</span><span class="sxs-lookup"><span data-stu-id="d6fa9-120">none</span></span>          |<span data-ttu-id="d6fa9-121">删除付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-121">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6fa9-122">属性</span><span class="sxs-lookup"><span data-stu-id="d6fa9-122">Properties</span></span>
| <span data-ttu-id="d6fa9-123">属性</span><span class="sxs-lookup"><span data-stu-id="d6fa9-123">Property</span></span>           | <span data-ttu-id="d6fa9-124">类型</span><span class="sxs-lookup"><span data-stu-id="d6fa9-124">Type</span></span>   |<span data-ttu-id="d6fa9-125">说明</span><span class="sxs-lookup"><span data-stu-id="d6fa9-125">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="d6fa9-126">id</span><span class="sxs-lookup"><span data-stu-id="d6fa9-126">id</span></span>                  |<span data-ttu-id="d6fa9-127">GUID</span><span class="sxs-lookup"><span data-stu-id="d6fa9-127">GUID</span></span>    |<span data-ttu-id="d6fa9-128">PaymentMethods 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-128">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="d6fa9-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-129">Non-editable.</span></span>           |
|<span data-ttu-id="d6fa9-130">code</span><span class="sxs-lookup"><span data-stu-id="d6fa9-130">code</span></span>                |<span data-ttu-id="d6fa9-131">string</span><span class="sxs-lookup"><span data-stu-id="d6fa9-131">string</span></span>  |<span data-ttu-id="d6fa9-132">指定付款方法代码。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-132">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="d6fa9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d6fa9-133">displayName</span></span>         |<span data-ttu-id="d6fa9-134">string</span><span class="sxs-lookup"><span data-stu-id="d6fa9-134">string</span></span>  |<span data-ttu-id="d6fa9-135">指定付款方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-135">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="d6fa9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6fa9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d6fa9-137">datetime</span><span class="sxs-lookup"><span data-stu-id="d6fa9-137">datetime</span></span>|<span data-ttu-id="d6fa9-138">上次修改付款方法的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-138">The last datetime the payment method was modified.</span></span> <span data-ttu-id="d6fa9-139">只读。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="d6fa9-140">关系</span><span class="sxs-lookup"><span data-stu-id="d6fa9-140">Relationships</span></span>
<span data-ttu-id="d6fa9-141">无</span><span class="sxs-lookup"><span data-stu-id="d6fa9-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6fa9-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6fa9-142">JSON representation</span></span>

<span data-ttu-id="d6fa9-143">下面是 paymentMethods 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6fa9-143">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
