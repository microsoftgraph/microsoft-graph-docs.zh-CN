---
title: skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 5377e8d8f2ec145f5aee590409206de75e915d9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048320"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="6da91-103">skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6da91-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6da91-104">属性</span><span class="sxs-lookup"><span data-stu-id="6da91-104">Properties</span></span>

| <span data-ttu-id="6da91-105">属性</span><span class="sxs-lookup"><span data-stu-id="6da91-105">Property</span></span>          | <span data-ttu-id="6da91-106">类型</span><span class="sxs-lookup"><span data-stu-id="6da91-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6da91-107">audio</span><span class="sxs-lookup"><span data-stu-id="6da91-107">audio</span></span>             | <span data-ttu-id="6da91-108">Int64</span><span class="sxs-lookup"><span data-stu-id="6da91-108">Int64</span></span>  |
| <span data-ttu-id="6da91-109">video</span><span class="sxs-lookup"><span data-stu-id="6da91-109">video</span></span>             | <span data-ttu-id="6da91-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6da91-110">Int64</span></span>  |
| <span data-ttu-id="6da91-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6da91-111">reportRefreshDate</span></span> | <span data-ttu-id="6da91-112">日期</span><span class="sxs-lookup"><span data-stu-id="6da91-112">Date</span></span>   |
| <span data-ttu-id="6da91-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="6da91-113">reportDate</span></span>        | <span data-ttu-id="6da91-114">日期</span><span class="sxs-lookup"><span data-stu-id="6da91-114">Date</span></span>   |
| <span data-ttu-id="6da91-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6da91-115">reportPeriod</span></span>      | <span data-ttu-id="6da91-116">String</span><span class="sxs-lookup"><span data-stu-id="6da91-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6da91-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6da91-117">JSON representation</span></span>

<span data-ttu-id="6da91-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6da91-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
