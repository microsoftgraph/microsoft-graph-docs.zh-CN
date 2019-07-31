---
author: JeremyKelley
description: 此资源提供异步作业进度状态的相关信息。
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e8a745a6ab03728eb879767c6af45a423f151d63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974300"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="b0761-103">AsyncJobStatus 资源</span><span class="sxs-lookup"><span data-stu-id="b0761-103">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0761-104">此资源提供异步作业进度状态的相关信息。</span><span class="sxs-lookup"><span data-stu-id="b0761-104">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="b0761-105">以下 API 调用返回 **AsyncJobStatus** 资源：</span><span class="sxs-lookup"><span data-stu-id="b0761-105">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="b0761-106">复制项</span><span class="sxs-lookup"><span data-stu-id="b0761-106">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="b0761-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0761-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="b0761-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0761-108">Properties</span></span>

| <span data-ttu-id="b0761-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="b0761-109">Property name</span></span>          | <span data-ttu-id="b0761-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0761-110">Type</span></span>   | <span data-ttu-id="b0761-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0761-111">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="b0761-112">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="b0761-112">**percentageComplete**</span></span> | <span data-ttu-id="b0761-113">Double</span><span class="sxs-lookup"><span data-stu-id="b0761-113">Double</span></span> | <span data-ttu-id="b0761-114">指明完成百分比的值，介于 0 到 100 之间。</span><span class="sxs-lookup"><span data-stu-id="b0761-114">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="b0761-115">**status**</span><span class="sxs-lookup"><span data-stu-id="b0761-115">**status**</span></span>             | <span data-ttu-id="b0761-116">String</span><span class="sxs-lookup"><span data-stu-id="b0761-116">String</span></span> | <span data-ttu-id="b0761-117">映射到作业状态可能值枚举的字符串值。</span><span class="sxs-lookup"><span data-stu-id="b0761-117">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
