---
title: generalLedgerEntries 资源类型
description: Dynamics 365 Business Central 中的总帐条目。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 500c78d0e29d83c68c2b7247a9787b977cc8a7b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973602"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="3c121-103">generalLedgerEntries 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c121-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="3c121-104">代表 Dynamics 365 Business Central 中的 generalLedgerEntry 对象。</span><span class="sxs-lookup"><span data-stu-id="3c121-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="3c121-105">方法</span><span class="sxs-lookup"><span data-stu-id="3c121-105">Methods</span></span>

| <span data-ttu-id="3c121-106">方法</span><span class="sxs-lookup"><span data-stu-id="3c121-106">Method</span></span>       | <span data-ttu-id="3c121-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c121-107">Return Type</span></span>  |<span data-ttu-id="3c121-108">说明</span><span class="sxs-lookup"><span data-stu-id="3c121-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="3c121-109">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="3c121-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="3c121-110">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="3c121-110">generalLedgerEntries</span></span>|<span data-ttu-id="3c121-111">获取一个 G/L 入口对象。</span><span class="sxs-lookup"><span data-stu-id="3c121-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c121-112">属性</span><span class="sxs-lookup"><span data-stu-id="3c121-112">Properties</span></span>
| <span data-ttu-id="3c121-113">属性</span><span class="sxs-lookup"><span data-stu-id="3c121-113">Property</span></span>           | <span data-ttu-id="3c121-114">类型</span><span class="sxs-lookup"><span data-stu-id="3c121-114">Type</span></span>                  |<span data-ttu-id="3c121-115">说明</span><span class="sxs-lookup"><span data-stu-id="3c121-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="3c121-116">id</span><span class="sxs-lookup"><span data-stu-id="3c121-116">id</span></span>                  |<span data-ttu-id="3c121-117">位数</span><span class="sxs-lookup"><span data-stu-id="3c121-117">numeric</span></span>                |<span data-ttu-id="3c121-118">G/L 条目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3c121-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="3c121-119">postingDate</span><span class="sxs-lookup"><span data-stu-id="3c121-119">postingDate</span></span>         |<span data-ttu-id="3c121-120">date</span><span class="sxs-lookup"><span data-stu-id="3c121-120">date</span></span>                   |<span data-ttu-id="3c121-121">指定 G/L 条目的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="3c121-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="3c121-122">documentNumber</span><span class="sxs-lookup"><span data-stu-id="3c121-122">documentNumber</span></span>      |<span data-ttu-id="3c121-123">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="3c121-123">string, maximum size 20</span></span>|<span data-ttu-id="3c121-124">指定 G/L 条目的文档编号。</span><span class="sxs-lookup"><span data-stu-id="3c121-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="3c121-125">documentType</span><span class="sxs-lookup"><span data-stu-id="3c121-125">documentType</span></span>        |<span data-ttu-id="3c121-126">string</span><span class="sxs-lookup"><span data-stu-id="3c121-126">string</span></span>                 |<span data-ttu-id="3c121-127">指定 G/L 项的文档类型。</span><span class="sxs-lookup"><span data-stu-id="3c121-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="3c121-128">accountId</span><span class="sxs-lookup"><span data-stu-id="3c121-128">accountId</span></span>           |<span data-ttu-id="3c121-129">GUID</span><span class="sxs-lookup"><span data-stu-id="3c121-129">GUID</span></span>                   |<span data-ttu-id="3c121-130">指定 G/L 条目的 accountId。</span><span class="sxs-lookup"><span data-stu-id="3c121-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="3c121-131">accountNumber</span><span class="sxs-lookup"><span data-stu-id="3c121-131">accountNumber</span></span>       |<span data-ttu-id="3c121-132">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="3c121-132">string, maximum size 20</span></span>|<span data-ttu-id="3c121-133">指定 G/L 条目的 accountNumber。</span><span class="sxs-lookup"><span data-stu-id="3c121-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="3c121-134">说明</span><span class="sxs-lookup"><span data-stu-id="3c121-134">description</span></span>         |<span data-ttu-id="3c121-135">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="3c121-135">string, maximum size 50</span></span>|<span data-ttu-id="3c121-136">指定 G/L 条目的说明。</span><span class="sxs-lookup"><span data-stu-id="3c121-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="3c121-137">debitAmount</span><span class="sxs-lookup"><span data-stu-id="3c121-137">debitAmount</span></span>         |<span data-ttu-id="3c121-138">位数</span><span class="sxs-lookup"><span data-stu-id="3c121-138">numeric</span></span>                |<span data-ttu-id="3c121-139">指定 G/L 条目的 debitAmount。</span><span class="sxs-lookup"><span data-stu-id="3c121-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="3c121-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="3c121-140">creditAmount</span></span>        |<span data-ttu-id="3c121-141">位数</span><span class="sxs-lookup"><span data-stu-id="3c121-141">numeric</span></span>                |<span data-ttu-id="3c121-142">指定 G/L 条目的 creditAmount。</span><span class="sxs-lookup"><span data-stu-id="3c121-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="3c121-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c121-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3c121-144">datetime</span><span class="sxs-lookup"><span data-stu-id="3c121-144">datetime</span></span>               |<span data-ttu-id="3c121-145">修改了 G/L 条目的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c121-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3c121-146">关系</span><span class="sxs-lookup"><span data-stu-id="3c121-146">Relationships</span></span>
<span data-ttu-id="3c121-147">无</span><span class="sxs-lookup"><span data-stu-id="3c121-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c121-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c121-148">JSON representation</span></span>

<span data-ttu-id="3c121-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c121-149">Here is a JSON representation of the resource.</span></span>


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

