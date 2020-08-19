---
title: skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: fda548f97a2aa3a2236d920a0f3439fb20710dc7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810977"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="60ba3-103">skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="60ba3-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

<span data-ttu-id="60ba3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ba3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="60ba3-105">属性</span><span class="sxs-lookup"><span data-stu-id="60ba3-105">Properties</span></span>

| <span data-ttu-id="60ba3-106">属性</span><span class="sxs-lookup"><span data-stu-id="60ba3-106">Property</span></span>          | <span data-ttu-id="60ba3-107">类型</span><span class="sxs-lookup"><span data-stu-id="60ba3-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="60ba3-108">audio</span><span class="sxs-lookup"><span data-stu-id="60ba3-108">audio</span></span>             | <span data-ttu-id="60ba3-109">Int64</span><span class="sxs-lookup"><span data-stu-id="60ba3-109">Int64</span></span>  |
| <span data-ttu-id="60ba3-110">video</span><span class="sxs-lookup"><span data-stu-id="60ba3-110">video</span></span>             | <span data-ttu-id="60ba3-111">Int64</span><span class="sxs-lookup"><span data-stu-id="60ba3-111">Int64</span></span>  |
| <span data-ttu-id="60ba3-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="60ba3-112">reportRefreshDate</span></span> | <span data-ttu-id="60ba3-113">日期</span><span class="sxs-lookup"><span data-stu-id="60ba3-113">Date</span></span>   |
| <span data-ttu-id="60ba3-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="60ba3-114">reportDate</span></span>        | <span data-ttu-id="60ba3-115">日期</span><span class="sxs-lookup"><span data-stu-id="60ba3-115">Date</span></span>   |
| <span data-ttu-id="60ba3-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="60ba3-116">reportPeriod</span></span>      | <span data-ttu-id="60ba3-117">String</span><span class="sxs-lookup"><span data-stu-id="60ba3-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60ba3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60ba3-118">JSON representation</span></span>

<span data-ttu-id="60ba3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60ba3-119">The following is a JSON representation of the resource.</span></span>

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
