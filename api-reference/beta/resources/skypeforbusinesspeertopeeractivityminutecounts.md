---
title: skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2fcea49c157a04dd48eda0f1645eab08540a917e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008059"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="b8748-103">skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8748-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b8748-104">属性</span><span class="sxs-lookup"><span data-stu-id="b8748-104">Properties</span></span>

| <span data-ttu-id="b8748-105">属性</span><span class="sxs-lookup"><span data-stu-id="b8748-105">Property</span></span>          | <span data-ttu-id="b8748-106">类型</span><span class="sxs-lookup"><span data-stu-id="b8748-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b8748-107">audio</span><span class="sxs-lookup"><span data-stu-id="b8748-107">audio</span></span>             | <span data-ttu-id="b8748-108">Int64</span><span class="sxs-lookup"><span data-stu-id="b8748-108">Int64</span></span>  |
| <span data-ttu-id="b8748-109">video</span><span class="sxs-lookup"><span data-stu-id="b8748-109">video</span></span>             | <span data-ttu-id="b8748-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b8748-110">Int64</span></span>  |
| <span data-ttu-id="b8748-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b8748-111">reportRefreshDate</span></span> | <span data-ttu-id="b8748-112">日期</span><span class="sxs-lookup"><span data-stu-id="b8748-112">Date</span></span>   |
| <span data-ttu-id="b8748-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="b8748-113">reportDate</span></span>        | <span data-ttu-id="b8748-114">日期</span><span class="sxs-lookup"><span data-stu-id="b8748-114">Date</span></span>   |
| <span data-ttu-id="b8748-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b8748-115">reportPeriod</span></span>      | <span data-ttu-id="b8748-116">String</span><span class="sxs-lookup"><span data-stu-id="b8748-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8748-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8748-117">JSON representation</span></span>

<span data-ttu-id="b8748-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8748-118">The following is a JSON representation of the resource.</span></span>

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
