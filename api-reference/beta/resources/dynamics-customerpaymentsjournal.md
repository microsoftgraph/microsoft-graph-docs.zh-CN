---
title: customerPaymentJournals 资源类型
description: Dynamics 365 Business Central 中的客户付款日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365736"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="800ff-103">customerPaymentsJournals 资源类型</span><span class="sxs-lookup"><span data-stu-id="800ff-103">customerPaymentsJournals resource type</span></span>
<span data-ttu-id="800ff-104">表示 Dynamics 365 Business Central 中的客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="800ff-104">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="800ff-105">方法</span><span class="sxs-lookup"><span data-stu-id="800ff-105">Methods</span></span>

| <span data-ttu-id="800ff-106">方法</span><span class="sxs-lookup"><span data-stu-id="800ff-106">Method</span></span>               | <span data-ttu-id="800ff-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="800ff-107">Return Type</span></span>             |<span data-ttu-id="800ff-108">说明</span><span class="sxs-lookup"><span data-stu-id="800ff-108">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="800ff-109">获取 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-109">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="800ff-110">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-110">customerPaymentJournals</span></span>|<span data-ttu-id="800ff-111">获取客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="800ff-111">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="800ff-112">Post customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-112">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="800ff-113">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-113">customerPaymentJournals</span></span>|<span data-ttu-id="800ff-114">创建客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="800ff-114">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="800ff-115">修补程序 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-115">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="800ff-116">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-116">customerPaymentJournals</span></span>|<span data-ttu-id="800ff-117">更新客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="800ff-117">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="800ff-118">删除 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="800ff-118">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="800ff-119">无</span><span class="sxs-lookup"><span data-stu-id="800ff-119">none</span></span>                     |<span data-ttu-id="800ff-120">删除客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="800ff-120">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="800ff-121">属性</span><span class="sxs-lookup"><span data-stu-id="800ff-121">Properties</span></span>
| <span data-ttu-id="800ff-122">属性</span><span class="sxs-lookup"><span data-stu-id="800ff-122">Property</span></span>           | <span data-ttu-id="800ff-123">类型</span><span class="sxs-lookup"><span data-stu-id="800ff-123">Type</span></span>                  |<span data-ttu-id="800ff-124">说明</span><span class="sxs-lookup"><span data-stu-id="800ff-124">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="800ff-125">id</span><span class="sxs-lookup"><span data-stu-id="800ff-125">id</span></span>                  |<span data-ttu-id="800ff-126">GUID</span><span class="sxs-lookup"><span data-stu-id="800ff-126">GUID</span></span>                   |<span data-ttu-id="800ff-127">客户付款日志的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="800ff-127">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="800ff-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="800ff-128">Non-editable.</span></span>           |
|<span data-ttu-id="800ff-129">code</span><span class="sxs-lookup"><span data-stu-id="800ff-129">code</span></span>                |<span data-ttu-id="800ff-130">字符串, 最大值为10</span><span class="sxs-lookup"><span data-stu-id="800ff-130">string, maximum size 10</span></span>| <span data-ttu-id="800ff-131">客户付款日志的代码。</span><span class="sxs-lookup"><span data-stu-id="800ff-131">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="800ff-132">displayName</span><span class="sxs-lookup"><span data-stu-id="800ff-132">displayName</span></span>         |<span data-ttu-id="800ff-133">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="800ff-133">string, maximum size 50</span></span>| <span data-ttu-id="800ff-134">客户付款日志的显示名称。</span><span class="sxs-lookup"><span data-stu-id="800ff-134">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="800ff-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="800ff-135">lastModifiedDateTime</span></span>|<span data-ttu-id="800ff-136">datetime</span><span class="sxs-lookup"><span data-stu-id="800ff-136">datetime</span></span>               |<span data-ttu-id="800ff-137">上次修改客户付款日志的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="800ff-137">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="800ff-138">只读。</span><span class="sxs-lookup"><span data-stu-id="800ff-138">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="800ff-139">关系</span><span class="sxs-lookup"><span data-stu-id="800ff-139">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="800ff-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="800ff-140">JSON representation</span></span>

<span data-ttu-id="800ff-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="800ff-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

