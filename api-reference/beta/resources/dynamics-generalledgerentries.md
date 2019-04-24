---
title: generalLedgerEntries 资源类型
description: Dynamics 365 Business Central 中的总帐条目。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507237"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="e5877-103">generalLedgerEntries 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5877-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="e5877-104">代表 Dynamics 365 Business Central 中的 generalLedgerEntry 对象。</span><span class="sxs-lookup"><span data-stu-id="e5877-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e5877-105">方法</span><span class="sxs-lookup"><span data-stu-id="e5877-105">Methods</span></span>

| <span data-ttu-id="e5877-106">方法</span><span class="sxs-lookup"><span data-stu-id="e5877-106">Method</span></span>       | <span data-ttu-id="e5877-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5877-107">Return Type</span></span>  |<span data-ttu-id="e5877-108">说明</span><span class="sxs-lookup"><span data-stu-id="e5877-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="e5877-109">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="e5877-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="e5877-110">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="e5877-110">generalLedgerEntries</span></span>|<span data-ttu-id="e5877-111">获取一个 G/L 入口对象。</span><span class="sxs-lookup"><span data-stu-id="e5877-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5877-112">属性</span><span class="sxs-lookup"><span data-stu-id="e5877-112">Properties</span></span>
| <span data-ttu-id="e5877-113">属性</span><span class="sxs-lookup"><span data-stu-id="e5877-113">Property</span></span>           | <span data-ttu-id="e5877-114">类型</span><span class="sxs-lookup"><span data-stu-id="e5877-114">Type</span></span>                  |<span data-ttu-id="e5877-115">说明</span><span class="sxs-lookup"><span data-stu-id="e5877-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="e5877-116">id</span><span class="sxs-lookup"><span data-stu-id="e5877-116">id</span></span>                  |<span data-ttu-id="e5877-117">位数</span><span class="sxs-lookup"><span data-stu-id="e5877-117">numeric</span></span>                |<span data-ttu-id="e5877-118">G/L 条目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e5877-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="e5877-119">postingDate</span><span class="sxs-lookup"><span data-stu-id="e5877-119">postingDate</span></span>         |<span data-ttu-id="e5877-120">date</span><span class="sxs-lookup"><span data-stu-id="e5877-120">date</span></span>                   |<span data-ttu-id="e5877-121">指定 G/L 条目的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="e5877-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="e5877-122">documentNumber</span><span class="sxs-lookup"><span data-stu-id="e5877-122">documentNumber</span></span>      |<span data-ttu-id="e5877-123">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="e5877-123">string, maximum size 20</span></span>|<span data-ttu-id="e5877-124">指定 G/L 条目的文档编号。</span><span class="sxs-lookup"><span data-stu-id="e5877-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="e5877-125">documentType</span><span class="sxs-lookup"><span data-stu-id="e5877-125">documentType</span></span>        |<span data-ttu-id="e5877-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e5877-126">string</span></span>                 |<span data-ttu-id="e5877-127">指定 G/L 项的文档类型。</span><span class="sxs-lookup"><span data-stu-id="e5877-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="e5877-128">accountId</span><span class="sxs-lookup"><span data-stu-id="e5877-128">accountId</span></span>           |<span data-ttu-id="e5877-129">GUID</span><span class="sxs-lookup"><span data-stu-id="e5877-129">GUID</span></span>                   |<span data-ttu-id="e5877-130">指定 G/L 条目的 accountId。</span><span class="sxs-lookup"><span data-stu-id="e5877-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="e5877-131">accountNumber</span><span class="sxs-lookup"><span data-stu-id="e5877-131">accountNumber</span></span>       |<span data-ttu-id="e5877-132">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="e5877-132">string, maximum size 20</span></span>|<span data-ttu-id="e5877-133">指定 G/L 条目的 accountNumber。</span><span class="sxs-lookup"><span data-stu-id="e5877-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="e5877-134">description</span><span class="sxs-lookup"><span data-stu-id="e5877-134">description</span></span>         |<span data-ttu-id="e5877-135">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="e5877-135">string, maximum size 50</span></span>|<span data-ttu-id="e5877-136">指定 G/L 条目的说明。</span><span class="sxs-lookup"><span data-stu-id="e5877-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="e5877-137">debitAmount</span><span class="sxs-lookup"><span data-stu-id="e5877-137">debitAmount</span></span>         |<span data-ttu-id="e5877-138">位数</span><span class="sxs-lookup"><span data-stu-id="e5877-138">numeric</span></span>                |<span data-ttu-id="e5877-139">指定 G/L 条目的 debitAmount。</span><span class="sxs-lookup"><span data-stu-id="e5877-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="e5877-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="e5877-140">creditAmount</span></span>        |<span data-ttu-id="e5877-141">位数</span><span class="sxs-lookup"><span data-stu-id="e5877-141">numeric</span></span>                |<span data-ttu-id="e5877-142">指定 G/L 条目的 creditAmount。</span><span class="sxs-lookup"><span data-stu-id="e5877-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="e5877-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5877-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e5877-144">datetime</span><span class="sxs-lookup"><span data-stu-id="e5877-144">datetime</span></span>               |<span data-ttu-id="e5877-145">修改了 G/L 条目的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e5877-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e5877-146">关系</span><span class="sxs-lookup"><span data-stu-id="e5877-146">Relationships</span></span>
<span data-ttu-id="e5877-147">无</span><span class="sxs-lookup"><span data-stu-id="e5877-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5877-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5877-148">JSON representation</span></span>

<span data-ttu-id="e5877-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5877-149">Here is a JSON representation of the resource.</span></span>


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

