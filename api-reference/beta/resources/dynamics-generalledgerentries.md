---
title: generalLedgerEntries 资源类型
description: Dynamics 365 Business Central 中的总帐条目。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f1dc4ec7bb3fa30f7dc6362c850893953c4aa6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503976"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="8d826-103">generalLedgerEntries 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d826-103">generalLedgerEntries resource type</span></span>

<span data-ttu-id="8d826-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8d826-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d826-105">代表 Dynamics 365 Business Central 中的 generalLedgerEntry 对象。</span><span class="sxs-lookup"><span data-stu-id="8d826-105">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8d826-106">方法</span><span class="sxs-lookup"><span data-stu-id="8d826-106">Methods</span></span>

| <span data-ttu-id="8d826-107">方法</span><span class="sxs-lookup"><span data-stu-id="8d826-107">Method</span></span>       | <span data-ttu-id="8d826-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d826-108">Return Type</span></span>  |<span data-ttu-id="8d826-109">说明</span><span class="sxs-lookup"><span data-stu-id="8d826-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="8d826-110">获取 generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="8d826-110">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="8d826-111">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="8d826-111">generalLedgerEntries</span></span>|<span data-ttu-id="8d826-112">获取一个 G/L 入口对象。</span><span class="sxs-lookup"><span data-stu-id="8d826-112">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d826-113">属性</span><span class="sxs-lookup"><span data-stu-id="8d826-113">Properties</span></span>
| <span data-ttu-id="8d826-114">属性</span><span class="sxs-lookup"><span data-stu-id="8d826-114">Property</span></span>           | <span data-ttu-id="8d826-115">类型</span><span class="sxs-lookup"><span data-stu-id="8d826-115">Type</span></span>                  |<span data-ttu-id="8d826-116">说明</span><span class="sxs-lookup"><span data-stu-id="8d826-116">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="8d826-117">id</span><span class="sxs-lookup"><span data-stu-id="8d826-117">id</span></span>                  |<span data-ttu-id="8d826-118">位数</span><span class="sxs-lookup"><span data-stu-id="8d826-118">numeric</span></span>                |<span data-ttu-id="8d826-119">G/L 条目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8d826-119">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="8d826-120">postingDate</span><span class="sxs-lookup"><span data-stu-id="8d826-120">postingDate</span></span>         |<span data-ttu-id="8d826-121">date</span><span class="sxs-lookup"><span data-stu-id="8d826-121">date</span></span>                   |<span data-ttu-id="8d826-122">指定 G/L 条目的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="8d826-122">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="8d826-123">documentNumber</span><span class="sxs-lookup"><span data-stu-id="8d826-123">documentNumber</span></span>      |<span data-ttu-id="8d826-124">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="8d826-124">string, maximum size 20</span></span>|<span data-ttu-id="8d826-125">指定 G/L 条目的文档编号。</span><span class="sxs-lookup"><span data-stu-id="8d826-125">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="8d826-126">documentType</span><span class="sxs-lookup"><span data-stu-id="8d826-126">documentType</span></span>        |<span data-ttu-id="8d826-127">string</span><span class="sxs-lookup"><span data-stu-id="8d826-127">string</span></span>                 |<span data-ttu-id="8d826-128">指定 G/L 项的文档类型。</span><span class="sxs-lookup"><span data-stu-id="8d826-128">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="8d826-129">accountId</span><span class="sxs-lookup"><span data-stu-id="8d826-129">accountId</span></span>           |<span data-ttu-id="8d826-130">GUID</span><span class="sxs-lookup"><span data-stu-id="8d826-130">GUID</span></span>                   |<span data-ttu-id="8d826-131">指定 G/L 条目的 accountId。</span><span class="sxs-lookup"><span data-stu-id="8d826-131">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="8d826-132">accountNumber</span><span class="sxs-lookup"><span data-stu-id="8d826-132">accountNumber</span></span>       |<span data-ttu-id="8d826-133">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="8d826-133">string, maximum size 20</span></span>|<span data-ttu-id="8d826-134">指定 G/L 条目的 accountNumber。</span><span class="sxs-lookup"><span data-stu-id="8d826-134">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="8d826-135">说明</span><span class="sxs-lookup"><span data-stu-id="8d826-135">description</span></span>         |<span data-ttu-id="8d826-136">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="8d826-136">string, maximum size 50</span></span>|<span data-ttu-id="8d826-137">指定 G/L 条目的说明。</span><span class="sxs-lookup"><span data-stu-id="8d826-137">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="8d826-138">debitAmount</span><span class="sxs-lookup"><span data-stu-id="8d826-138">debitAmount</span></span>         |<span data-ttu-id="8d826-139">位数</span><span class="sxs-lookup"><span data-stu-id="8d826-139">numeric</span></span>                |<span data-ttu-id="8d826-140">指定 G/L 条目的 debitAmount。</span><span class="sxs-lookup"><span data-stu-id="8d826-140">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="8d826-141">creditAmount</span><span class="sxs-lookup"><span data-stu-id="8d826-141">creditAmount</span></span>        |<span data-ttu-id="8d826-142">位数</span><span class="sxs-lookup"><span data-stu-id="8d826-142">numeric</span></span>                |<span data-ttu-id="8d826-143">指定 G/L 条目的 creditAmount。</span><span class="sxs-lookup"><span data-stu-id="8d826-143">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="8d826-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d826-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8d826-145">datetime</span><span class="sxs-lookup"><span data-stu-id="8d826-145">datetime</span></span>               |<span data-ttu-id="8d826-146">修改了 G/L 条目的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8d826-146">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8d826-147">关系</span><span class="sxs-lookup"><span data-stu-id="8d826-147">Relationships</span></span>
<span data-ttu-id="8d826-148">无</span><span class="sxs-lookup"><span data-stu-id="8d826-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d826-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d826-149">JSON representation</span></span>

<span data-ttu-id="8d826-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d826-150">Here is a JSON representation of the resource.</span></span>


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

