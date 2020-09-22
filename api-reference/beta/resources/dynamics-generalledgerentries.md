---
title: generalLedgerEntries 资源类型
description: Dynamics 365 Business Central 中的总帐条目。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 354dac3ca4912231b7ced6449f61623c18dbd36d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071330"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="0ca50-103">generalLedgerEntries 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ca50-103">generalLedgerEntries resource type</span></span>

<span data-ttu-id="0ca50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ca50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca50-105">代表 Dynamics 365 Business Central 中的 generalLedgerEntry 对象。</span><span class="sxs-lookup"><span data-stu-id="0ca50-105">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0ca50-106">方法</span><span class="sxs-lookup"><span data-stu-id="0ca50-106">Methods</span></span>

| <span data-ttu-id="0ca50-107">方法</span><span class="sxs-lookup"><span data-stu-id="0ca50-107">Method</span></span>       | <span data-ttu-id="0ca50-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ca50-108">Return Type</span></span>  |<span data-ttu-id="0ca50-109">说明</span><span class="sxs-lookup"><span data-stu-id="0ca50-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="0ca50-110">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="0ca50-110">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="0ca50-111">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="0ca50-111">generalLedgerEntries</span></span>|<span data-ttu-id="0ca50-112">获取一个 G/L 入口对象。</span><span class="sxs-lookup"><span data-stu-id="0ca50-112">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ca50-113">属性</span><span class="sxs-lookup"><span data-stu-id="0ca50-113">Properties</span></span>
| <span data-ttu-id="0ca50-114">属性</span><span class="sxs-lookup"><span data-stu-id="0ca50-114">Property</span></span>           | <span data-ttu-id="0ca50-115">类型</span><span class="sxs-lookup"><span data-stu-id="0ca50-115">Type</span></span>                  |<span data-ttu-id="0ca50-116">说明</span><span class="sxs-lookup"><span data-stu-id="0ca50-116">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="0ca50-117">id</span><span class="sxs-lookup"><span data-stu-id="0ca50-117">id</span></span>                  |<span data-ttu-id="0ca50-118">位数</span><span class="sxs-lookup"><span data-stu-id="0ca50-118">numeric</span></span>                |<span data-ttu-id="0ca50-119">G/L 条目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="0ca50-119">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="0ca50-120">postingDate</span><span class="sxs-lookup"><span data-stu-id="0ca50-120">postingDate</span></span>         |<span data-ttu-id="0ca50-121">date</span><span class="sxs-lookup"><span data-stu-id="0ca50-121">date</span></span>                   |<span data-ttu-id="0ca50-122">指定 G/L 条目的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="0ca50-122">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="0ca50-123">documentNumber</span><span class="sxs-lookup"><span data-stu-id="0ca50-123">documentNumber</span></span>      |<span data-ttu-id="0ca50-124">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="0ca50-124">string, maximum size 20</span></span>|<span data-ttu-id="0ca50-125">指定 G/L 条目的文档编号。</span><span class="sxs-lookup"><span data-stu-id="0ca50-125">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="0ca50-126">documentType</span><span class="sxs-lookup"><span data-stu-id="0ca50-126">documentType</span></span>        |<span data-ttu-id="0ca50-127">string</span><span class="sxs-lookup"><span data-stu-id="0ca50-127">string</span></span>                 |<span data-ttu-id="0ca50-128">指定 G/L 项的文档类型。</span><span class="sxs-lookup"><span data-stu-id="0ca50-128">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="0ca50-129">accountId</span><span class="sxs-lookup"><span data-stu-id="0ca50-129">accountId</span></span>           |<span data-ttu-id="0ca50-130">GUID</span><span class="sxs-lookup"><span data-stu-id="0ca50-130">GUID</span></span>                   |<span data-ttu-id="0ca50-131">指定 G/L 条目的 accountId。</span><span class="sxs-lookup"><span data-stu-id="0ca50-131">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="0ca50-132">accountNumber</span><span class="sxs-lookup"><span data-stu-id="0ca50-132">accountNumber</span></span>       |<span data-ttu-id="0ca50-133">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="0ca50-133">string, maximum size 20</span></span>|<span data-ttu-id="0ca50-134">指定 G/L 条目的 accountNumber。</span><span class="sxs-lookup"><span data-stu-id="0ca50-134">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="0ca50-135">说明</span><span class="sxs-lookup"><span data-stu-id="0ca50-135">description</span></span>         |<span data-ttu-id="0ca50-136">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="0ca50-136">string, maximum size 50</span></span>|<span data-ttu-id="0ca50-137">指定 G/L 条目的说明。</span><span class="sxs-lookup"><span data-stu-id="0ca50-137">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="0ca50-138">debitAmount</span><span class="sxs-lookup"><span data-stu-id="0ca50-138">debitAmount</span></span>         |<span data-ttu-id="0ca50-139">位数</span><span class="sxs-lookup"><span data-stu-id="0ca50-139">numeric</span></span>                |<span data-ttu-id="0ca50-140">指定 G/L 条目的 debitAmount。</span><span class="sxs-lookup"><span data-stu-id="0ca50-140">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="0ca50-141">creditAmount</span><span class="sxs-lookup"><span data-stu-id="0ca50-141">creditAmount</span></span>        |<span data-ttu-id="0ca50-142">位数</span><span class="sxs-lookup"><span data-stu-id="0ca50-142">numeric</span></span>                |<span data-ttu-id="0ca50-143">指定 G/L 条目的 creditAmount。</span><span class="sxs-lookup"><span data-stu-id="0ca50-143">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="0ca50-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ca50-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0ca50-145">datetime</span><span class="sxs-lookup"><span data-stu-id="0ca50-145">datetime</span></span>               |<span data-ttu-id="0ca50-146">修改了 G/L 条目的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ca50-146">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="0ca50-147">关系</span><span class="sxs-lookup"><span data-stu-id="0ca50-147">Relationships</span></span>
<span data-ttu-id="0ca50-148">无</span><span class="sxs-lookup"><span data-stu-id="0ca50-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ca50-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ca50-149">JSON representation</span></span>

<span data-ttu-id="0ca50-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ca50-150">Here is a JSON representation of the resource.</span></span>


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



