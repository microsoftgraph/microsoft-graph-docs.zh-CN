---
title: sharePointActivityPages 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 9111457d5cb9e710f0b07a43ea06c137af0db0f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041510"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="fbf2a-103">sharePointActivityPages 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbf2a-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fbf2a-104">属性</span><span class="sxs-lookup"><span data-stu-id="fbf2a-104">Properties</span></span>

| <span data-ttu-id="fbf2a-105">属性</span><span class="sxs-lookup"><span data-stu-id="fbf2a-105">Property</span></span>          | <span data-ttu-id="fbf2a-106">类型</span><span class="sxs-lookup"><span data-stu-id="fbf2a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fbf2a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fbf2a-107">reportRefreshDate</span></span> | <span data-ttu-id="fbf2a-108">日期</span><span class="sxs-lookup"><span data-stu-id="fbf2a-108">Date</span></span>   |
| <span data-ttu-id="fbf2a-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="fbf2a-109">visitedPageCount</span></span>  | <span data-ttu-id="fbf2a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="fbf2a-110">Int64</span></span>  |
| <span data-ttu-id="fbf2a-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="fbf2a-111">reportDate</span></span>        | <span data-ttu-id="fbf2a-112">日期</span><span class="sxs-lookup"><span data-stu-id="fbf2a-112">Date</span></span>   |
| <span data-ttu-id="fbf2a-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fbf2a-113">reportPeriod</span></span>      | <span data-ttu-id="fbf2a-114">String</span><span class="sxs-lookup"><span data-stu-id="fbf2a-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fbf2a-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbf2a-115">JSON representation</span></span>

<span data-ttu-id="fbf2a-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbf2a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
