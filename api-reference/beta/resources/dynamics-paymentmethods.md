---
title: paymentMethods 资源类型
description: Dynamics 365 Business Central 中的付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 08cfc864ee670a799a5f1672fa96cf8167ef1423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006582"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="d538a-103">paymentMethods 资源类型</span><span class="sxs-lookup"><span data-stu-id="d538a-103">paymentMethods resource type</span></span>
<span data-ttu-id="d538a-104">代表 Dynamics 365 Business Central 中的付款方式, 如 PayPal、信用卡和银行帐户。</span><span class="sxs-lookup"><span data-stu-id="d538a-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="d538a-105">方法</span><span class="sxs-lookup"><span data-stu-id="d538a-105">Methods</span></span>

| <span data-ttu-id="d538a-106">方法</span><span class="sxs-lookup"><span data-stu-id="d538a-106">Method</span></span>                                                          | <span data-ttu-id="d538a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d538a-107">Return Type</span></span>  |<span data-ttu-id="d538a-108">说明</span><span class="sxs-lookup"><span data-stu-id="d538a-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="d538a-109">获取 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="d538a-110">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-110">paymentMethods</span></span>|<span data-ttu-id="d538a-111">获取付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d538a-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="d538a-112">Post paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="d538a-113">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-113">paymentMethods</span></span>|<span data-ttu-id="d538a-114">创建付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d538a-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="d538a-115">修补程序 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="d538a-116">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-116">paymentMethods</span></span>|<span data-ttu-id="d538a-117">更新付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d538a-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="d538a-118">删除 paymentMethods</span><span class="sxs-lookup"><span data-stu-id="d538a-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="d538a-119">无</span><span class="sxs-lookup"><span data-stu-id="d538a-119">none</span></span>          |<span data-ttu-id="d538a-120">删除付款方法对象。</span><span class="sxs-lookup"><span data-stu-id="d538a-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d538a-121">属性</span><span class="sxs-lookup"><span data-stu-id="d538a-121">Properties</span></span>
| <span data-ttu-id="d538a-122">属性</span><span class="sxs-lookup"><span data-stu-id="d538a-122">Property</span></span>           | <span data-ttu-id="d538a-123">类型</span><span class="sxs-lookup"><span data-stu-id="d538a-123">Type</span></span>   |<span data-ttu-id="d538a-124">说明</span><span class="sxs-lookup"><span data-stu-id="d538a-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="d538a-125">id</span><span class="sxs-lookup"><span data-stu-id="d538a-125">id</span></span>                  |<span data-ttu-id="d538a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="d538a-126">GUID</span></span>    |<span data-ttu-id="d538a-127">PaymentMethods 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d538a-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="d538a-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="d538a-128">Non-editable.</span></span>           |
|<span data-ttu-id="d538a-129">code</span><span class="sxs-lookup"><span data-stu-id="d538a-129">code</span></span>                |<span data-ttu-id="d538a-130">string</span><span class="sxs-lookup"><span data-stu-id="d538a-130">string</span></span>  |<span data-ttu-id="d538a-131">指定付款方法代码。</span><span class="sxs-lookup"><span data-stu-id="d538a-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="d538a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d538a-132">displayName</span></span>         |<span data-ttu-id="d538a-133">string</span><span class="sxs-lookup"><span data-stu-id="d538a-133">string</span></span>  |<span data-ttu-id="d538a-134">指定付款方法的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d538a-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="d538a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d538a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d538a-136">datetime</span><span class="sxs-lookup"><span data-stu-id="d538a-136">datetime</span></span>|<span data-ttu-id="d538a-137">上次修改付款方法的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d538a-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="d538a-138">只读。</span><span class="sxs-lookup"><span data-stu-id="d538a-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="d538a-139">关系</span><span class="sxs-lookup"><span data-stu-id="d538a-139">Relationships</span></span>
<span data-ttu-id="d538a-140">无</span><span class="sxs-lookup"><span data-stu-id="d538a-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d538a-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d538a-141">JSON representation</span></span>

<span data-ttu-id="d538a-142">下面是 paymentMethods 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d538a-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
