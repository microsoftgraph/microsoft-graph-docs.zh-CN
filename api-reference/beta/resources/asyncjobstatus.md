---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 8c442ad8ff3b23d20e8377a224a3f67b00163f5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820963"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="12ae7-102">AsyncJobStatus 资源</span><span class="sxs-lookup"><span data-stu-id="12ae7-102">AsyncJobStatus resource</span></span>

> <span data-ttu-id="12ae7-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12ae7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12ae7-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12ae7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12ae7-105">此资源提供异步作业进度状态的相关信息。</span><span class="sxs-lookup"><span data-stu-id="12ae7-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="12ae7-106">以下 API 调用返回 **AsyncJobStatus** 资源：</span><span class="sxs-lookup"><span data-stu-id="12ae7-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="12ae7-107">复制项</span><span class="sxs-lookup"><span data-stu-id="12ae7-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="12ae7-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12ae7-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="12ae7-109">属性</span><span class="sxs-lookup"><span data-stu-id="12ae7-109">Properties</span></span>

| <span data-ttu-id="12ae7-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="12ae7-110">Property name</span></span>          | <span data-ttu-id="12ae7-111">类型</span><span class="sxs-lookup"><span data-stu-id="12ae7-111">Type</span></span>   | <span data-ttu-id="12ae7-112">说明</span><span class="sxs-lookup"><span data-stu-id="12ae7-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="12ae7-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="12ae7-113">**percentageComplete**</span></span> | <span data-ttu-id="12ae7-114">Double</span><span class="sxs-lookup"><span data-stu-id="12ae7-114">Double</span></span> | <span data-ttu-id="12ae7-115">指明完成百分比的值，介于 0 到 100 之间。</span><span class="sxs-lookup"><span data-stu-id="12ae7-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="12ae7-116">**status**</span><span class="sxs-lookup"><span data-stu-id="12ae7-116">**status**</span></span>             | <span data-ttu-id="12ae7-117">String</span><span class="sxs-lookup"><span data-stu-id="12ae7-117">String</span></span> | <span data-ttu-id="12ae7-118">映射到作业状态可能值枚举的字符串值。</span><span class="sxs-lookup"><span data-stu-id="12ae7-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
