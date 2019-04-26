---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 74ead4ca8e45c5baebe3ea74377ce102d9e2ee88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328645"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="f0250-102">AsyncJobStatus 资源</span><span class="sxs-lookup"><span data-stu-id="f0250-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0250-103">此资源提供异步作业进度状态的相关信息。</span><span class="sxs-lookup"><span data-stu-id="f0250-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="f0250-104">以下 API 调用返回 **AsyncJobStatus** 资源：</span><span class="sxs-lookup"><span data-stu-id="f0250-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="f0250-105">复制项</span><span class="sxs-lookup"><span data-stu-id="f0250-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="f0250-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0250-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="f0250-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0250-107">Properties</span></span>

| <span data-ttu-id="f0250-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="f0250-108">Property name</span></span>          | <span data-ttu-id="f0250-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0250-109">Type</span></span>   | <span data-ttu-id="f0250-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0250-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="f0250-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="f0250-111">**percentageComplete**</span></span> | <span data-ttu-id="f0250-112">Double</span><span class="sxs-lookup"><span data-stu-id="f0250-112">Double</span></span> | <span data-ttu-id="f0250-113">指明完成百分比的值，介于 0 到 100 之间。</span><span class="sxs-lookup"><span data-stu-id="f0250-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="f0250-114">**status**</span><span class="sxs-lookup"><span data-stu-id="f0250-114">**status**</span></span>             | <span data-ttu-id="f0250-115">String</span><span class="sxs-lookup"><span data-stu-id="f0250-115">String</span></span> | <span data-ttu-id="f0250-116">映射到作业状态可能值枚举的字符串值。</span><span class="sxs-lookup"><span data-stu-id="f0250-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
