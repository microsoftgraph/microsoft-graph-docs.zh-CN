---
title: generalLedgerEntries 资源类型
description: Dynamics 365 Business Central 中的总帐条目。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365757"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="170d1-103">generalLedgerEntries 资源类型</span><span class="sxs-lookup"><span data-stu-id="170d1-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="170d1-104">代表 Dynamics 365 Business Central 中的 generalLedgerEntry 对象。</span><span class="sxs-lookup"><span data-stu-id="170d1-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="170d1-105">方法</span><span class="sxs-lookup"><span data-stu-id="170d1-105">Methods</span></span>

| <span data-ttu-id="170d1-106">方法</span><span class="sxs-lookup"><span data-stu-id="170d1-106">Method</span></span>       | <span data-ttu-id="170d1-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="170d1-107">Return Type</span></span>  |<span data-ttu-id="170d1-108">说明</span><span class="sxs-lookup"><span data-stu-id="170d1-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="170d1-109">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="170d1-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="170d1-110">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="170d1-110">generalLedgerEntries</span></span>|<span data-ttu-id="170d1-111">获取一个 G/L 入口对象。</span><span class="sxs-lookup"><span data-stu-id="170d1-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="170d1-112">属性</span><span class="sxs-lookup"><span data-stu-id="170d1-112">Properties</span></span>
| <span data-ttu-id="170d1-113">属性</span><span class="sxs-lookup"><span data-stu-id="170d1-113">Property</span></span>           | <span data-ttu-id="170d1-114">类型</span><span class="sxs-lookup"><span data-stu-id="170d1-114">Type</span></span>                  |<span data-ttu-id="170d1-115">说明</span><span class="sxs-lookup"><span data-stu-id="170d1-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="170d1-116">id</span><span class="sxs-lookup"><span data-stu-id="170d1-116">id</span></span>                  |<span data-ttu-id="170d1-117">位数</span><span class="sxs-lookup"><span data-stu-id="170d1-117">numeric</span></span>                |<span data-ttu-id="170d1-118">G/L 条目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="170d1-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="170d1-119">postingDate</span><span class="sxs-lookup"><span data-stu-id="170d1-119">postingDate</span></span>         |<span data-ttu-id="170d1-120">date</span><span class="sxs-lookup"><span data-stu-id="170d1-120">date</span></span>                   |<span data-ttu-id="170d1-121">指定 G/L 条目的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="170d1-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="170d1-122">documentNumber</span><span class="sxs-lookup"><span data-stu-id="170d1-122">documentNumber</span></span>      |<span data-ttu-id="170d1-123">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="170d1-123">string, maximum size 20</span></span>|<span data-ttu-id="170d1-124">指定 G/L 条目的文档编号。</span><span class="sxs-lookup"><span data-stu-id="170d1-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="170d1-125">documentType</span><span class="sxs-lookup"><span data-stu-id="170d1-125">documentType</span></span>        |<span data-ttu-id="170d1-126">string</span><span class="sxs-lookup"><span data-stu-id="170d1-126">string</span></span>                 |<span data-ttu-id="170d1-127">指定 G/L 项的文档类型。</span><span class="sxs-lookup"><span data-stu-id="170d1-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="170d1-128">accountId</span><span class="sxs-lookup"><span data-stu-id="170d1-128">accountId</span></span>           |<span data-ttu-id="170d1-129">GUID</span><span class="sxs-lookup"><span data-stu-id="170d1-129">GUID</span></span>                   |<span data-ttu-id="170d1-130">指定 G/L 条目的 accountId。</span><span class="sxs-lookup"><span data-stu-id="170d1-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="170d1-131">accountNumber</span><span class="sxs-lookup"><span data-stu-id="170d1-131">accountNumber</span></span>       |<span data-ttu-id="170d1-132">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="170d1-132">string, maximum size 20</span></span>|<span data-ttu-id="170d1-133">指定 G/L 条目的 accountNumber。</span><span class="sxs-lookup"><span data-stu-id="170d1-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="170d1-134">说明</span><span class="sxs-lookup"><span data-stu-id="170d1-134">description</span></span>         |<span data-ttu-id="170d1-135">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="170d1-135">string, maximum size 50</span></span>|<span data-ttu-id="170d1-136">指定 G/L 条目的说明。</span><span class="sxs-lookup"><span data-stu-id="170d1-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="170d1-137">debitAmount</span><span class="sxs-lookup"><span data-stu-id="170d1-137">debitAmount</span></span>         |<span data-ttu-id="170d1-138">位数</span><span class="sxs-lookup"><span data-stu-id="170d1-138">numeric</span></span>                |<span data-ttu-id="170d1-139">指定 G/L 条目的 debitAmount。</span><span class="sxs-lookup"><span data-stu-id="170d1-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="170d1-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="170d1-140">creditAmount</span></span>        |<span data-ttu-id="170d1-141">位数</span><span class="sxs-lookup"><span data-stu-id="170d1-141">numeric</span></span>                |<span data-ttu-id="170d1-142">指定 G/L 条目的 creditAmount。</span><span class="sxs-lookup"><span data-stu-id="170d1-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="170d1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="170d1-143">lastModifiedDateTime</span></span>|<span data-ttu-id="170d1-144">datetime</span><span class="sxs-lookup"><span data-stu-id="170d1-144">datetime</span></span>               |<span data-ttu-id="170d1-145">修改了 G/L 条目的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="170d1-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="170d1-146">关系</span><span class="sxs-lookup"><span data-stu-id="170d1-146">Relationships</span></span>
<span data-ttu-id="170d1-147">无</span><span class="sxs-lookup"><span data-stu-id="170d1-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="170d1-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="170d1-148">JSON representation</span></span>

<span data-ttu-id="170d1-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="170d1-149">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

