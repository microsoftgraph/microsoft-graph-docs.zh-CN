---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482229"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="4a583-102">AsyncJobStatus 资源</span><span class="sxs-lookup"><span data-stu-id="4a583-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a583-103">此资源提供异步作业进度状态的相关信息。</span><span class="sxs-lookup"><span data-stu-id="4a583-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="4a583-104">以下 API 调用返回 **AsyncJobStatus** 资源：</span><span class="sxs-lookup"><span data-stu-id="4a583-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="4a583-105">复制项</span><span class="sxs-lookup"><span data-stu-id="4a583-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="4a583-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a583-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="4a583-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a583-107">Properties</span></span>

| <span data-ttu-id="4a583-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="4a583-108">Property name</span></span>          | <span data-ttu-id="4a583-109">类型</span><span class="sxs-lookup"><span data-stu-id="4a583-109">Type</span></span>   | <span data-ttu-id="4a583-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a583-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="4a583-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="4a583-111">**percentageComplete**</span></span> | <span data-ttu-id="4a583-112">Double</span><span class="sxs-lookup"><span data-stu-id="4a583-112">Double</span></span> | <span data-ttu-id="4a583-113">指明完成百分比的值，介于 0 到 100 之间。</span><span class="sxs-lookup"><span data-stu-id="4a583-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="4a583-114">**status**</span><span class="sxs-lookup"><span data-stu-id="4a583-114">**status**</span></span>             | <span data-ttu-id="4a583-115">String</span><span class="sxs-lookup"><span data-stu-id="4a583-115">String</span></span> | <span data-ttu-id="4a583-116">映射到作业状态可能值枚举的字符串值。</span><span class="sxs-lookup"><span data-stu-id="4a583-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
