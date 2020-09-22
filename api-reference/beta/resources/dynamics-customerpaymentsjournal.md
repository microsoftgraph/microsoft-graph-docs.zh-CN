---
title: customerPaymentJournals 资源类型
description: Dynamics 365 Business Central 中的客户付款日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a6fc1cf1541ebfbcf514de3005c7a89961531568
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071352"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="1827d-103">customerPaymentsJournals 资源类型</span><span class="sxs-lookup"><span data-stu-id="1827d-103">customerPaymentsJournals resource type</span></span>

<span data-ttu-id="1827d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1827d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1827d-105">表示 Dynamics 365 Business Central 中的客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="1827d-105">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1827d-106">方法</span><span class="sxs-lookup"><span data-stu-id="1827d-106">Methods</span></span>

| <span data-ttu-id="1827d-107">方法</span><span class="sxs-lookup"><span data-stu-id="1827d-107">Method</span></span>               | <span data-ttu-id="1827d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1827d-108">Return Type</span></span>             |<span data-ttu-id="1827d-109">说明</span><span class="sxs-lookup"><span data-stu-id="1827d-109">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="1827d-110">获取 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-110">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="1827d-111">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-111">customerPaymentJournals</span></span>|<span data-ttu-id="1827d-112">获取客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="1827d-112">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="1827d-113">Post customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-113">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="1827d-114">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-114">customerPaymentJournals</span></span>|<span data-ttu-id="1827d-115">创建客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="1827d-115">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="1827d-116">修补程序 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-116">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="1827d-117">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-117">customerPaymentJournals</span></span>|<span data-ttu-id="1827d-118">更新客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="1827d-118">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="1827d-119">删除 customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="1827d-119">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="1827d-120">无</span><span class="sxs-lookup"><span data-stu-id="1827d-120">none</span></span>                     |<span data-ttu-id="1827d-121">删除客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="1827d-121">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="1827d-122">属性</span><span class="sxs-lookup"><span data-stu-id="1827d-122">Properties</span></span>
| <span data-ttu-id="1827d-123">属性</span><span class="sxs-lookup"><span data-stu-id="1827d-123">Property</span></span>           | <span data-ttu-id="1827d-124">类型</span><span class="sxs-lookup"><span data-stu-id="1827d-124">Type</span></span>                  |<span data-ttu-id="1827d-125">说明</span><span class="sxs-lookup"><span data-stu-id="1827d-125">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="1827d-126">id</span><span class="sxs-lookup"><span data-stu-id="1827d-126">id</span></span>                  |<span data-ttu-id="1827d-127">GUID</span><span class="sxs-lookup"><span data-stu-id="1827d-127">GUID</span></span>                   |<span data-ttu-id="1827d-128">客户付款日志的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1827d-128">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="1827d-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="1827d-129">Non-editable.</span></span>           |
|<span data-ttu-id="1827d-130">code</span><span class="sxs-lookup"><span data-stu-id="1827d-130">code</span></span>                |<span data-ttu-id="1827d-131">字符串，最大值为10</span><span class="sxs-lookup"><span data-stu-id="1827d-131">string, maximum size 10</span></span>| <span data-ttu-id="1827d-132">客户付款日志的代码。</span><span class="sxs-lookup"><span data-stu-id="1827d-132">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="1827d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1827d-133">displayName</span></span>         |<span data-ttu-id="1827d-134">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="1827d-134">string, maximum size 50</span></span>| <span data-ttu-id="1827d-135">客户付款日志的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1827d-135">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="1827d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1827d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1827d-137">datetime</span><span class="sxs-lookup"><span data-stu-id="1827d-137">datetime</span></span>               |<span data-ttu-id="1827d-138">上次修改客户付款日志的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1827d-138">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="1827d-139">只读。</span><span class="sxs-lookup"><span data-stu-id="1827d-139">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1827d-140">关系</span><span class="sxs-lookup"><span data-stu-id="1827d-140">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="1827d-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1827d-141">JSON representation</span></span>

<span data-ttu-id="1827d-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1827d-142">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```



