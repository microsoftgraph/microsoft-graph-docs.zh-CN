---
author: JeremyKelley
description: 此资源提供异步作业进度状态的相关信息。
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 81348ce59e060dadf4201222fca43bf96241dbc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508169"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="3ba5f-103">AsyncJobStatus 资源</span><span class="sxs-lookup"><span data-stu-id="3ba5f-103">AsyncJobStatus resource</span></span>

<span data-ttu-id="3ba5f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3ba5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ba5f-105">此资源提供异步作业进度状态的相关信息。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="3ba5f-106">以下 API 调用返回 **AsyncJobStatus** 资源：</span><span class="sxs-lookup"><span data-stu-id="3ba5f-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="3ba5f-107">复制项</span><span class="sxs-lookup"><span data-stu-id="3ba5f-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="3ba5f-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ba5f-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="3ba5f-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ba5f-109">Properties</span></span>

| <span data-ttu-id="3ba5f-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="3ba5f-110">Property name</span></span>          | <span data-ttu-id="3ba5f-111">类型</span><span class="sxs-lookup"><span data-stu-id="3ba5f-111">Type</span></span>   | <span data-ttu-id="3ba5f-112">说明</span><span class="sxs-lookup"><span data-stu-id="3ba5f-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="3ba5f-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="3ba5f-113">**percentageComplete**</span></span> | <span data-ttu-id="3ba5f-114">Double</span><span class="sxs-lookup"><span data-stu-id="3ba5f-114">Double</span></span> | <span data-ttu-id="3ba5f-115">指明完成百分比的值，介于 0 到 100 之间。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="3ba5f-116">**status**</span><span class="sxs-lookup"><span data-stu-id="3ba5f-116">**status**</span></span>             | <span data-ttu-id="3ba5f-117">String</span><span class="sxs-lookup"><span data-stu-id="3ba5f-117">String</span></span> | <span data-ttu-id="3ba5f-118">映射到作业状态可能值枚举的字符串值。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
