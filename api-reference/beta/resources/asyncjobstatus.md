---
author: JeremyKelley
description: 此资源提供异步作业进度状态的相关信息。
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7bbc0a9fe74217d2b510db1e4439962d099e3bef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027249"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="d6d61-103">AsyncJobStatus 资源</span><span class="sxs-lookup"><span data-stu-id="d6d61-103">AsyncJobStatus resource</span></span>

<span data-ttu-id="d6d61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6d61-105">此资源提供异步作业进度状态的相关信息。</span><span class="sxs-lookup"><span data-stu-id="d6d61-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="d6d61-106">以下 API 调用返回 **AsyncJobStatus** 资源：</span><span class="sxs-lookup"><span data-stu-id="d6d61-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="d6d61-107">复制项</span><span class="sxs-lookup"><span data-stu-id="d6d61-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="d6d61-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6d61-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="d6d61-109">属性</span><span class="sxs-lookup"><span data-stu-id="d6d61-109">Properties</span></span>

| <span data-ttu-id="d6d61-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="d6d61-110">Property name</span></span>          | <span data-ttu-id="d6d61-111">类型</span><span class="sxs-lookup"><span data-stu-id="d6d61-111">Type</span></span>   | <span data-ttu-id="d6d61-112">说明</span><span class="sxs-lookup"><span data-stu-id="d6d61-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="d6d61-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="d6d61-113">**percentageComplete**</span></span> | <span data-ttu-id="d6d61-114">Double</span><span class="sxs-lookup"><span data-stu-id="d6d61-114">Double</span></span> | <span data-ttu-id="d6d61-115">指明完成百分比的值，介于 0 到 100 之间。</span><span class="sxs-lookup"><span data-stu-id="d6d61-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="d6d61-116">**status**</span><span class="sxs-lookup"><span data-stu-id="d6d61-116">**status**</span></span>             | <span data-ttu-id="d6d61-117">String</span><span class="sxs-lookup"><span data-stu-id="d6d61-117">String</span></span> | <span data-ttu-id="d6d61-118">映射到作业状态可能值枚举的字符串值。</span><span class="sxs-lookup"><span data-stu-id="d6d61-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->


