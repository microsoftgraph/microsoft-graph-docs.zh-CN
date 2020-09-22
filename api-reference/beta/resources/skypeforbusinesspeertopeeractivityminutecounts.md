---
title: skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 3ca572cb5ab5199ff42b895f72ca23fcdfc6d118
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087521"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="53a62-103">skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="53a62-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

<span data-ttu-id="53a62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53a62-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="53a62-105">属性</span><span class="sxs-lookup"><span data-stu-id="53a62-105">Properties</span></span>

| <span data-ttu-id="53a62-106">属性</span><span class="sxs-lookup"><span data-stu-id="53a62-106">Property</span></span>          | <span data-ttu-id="53a62-107">类型</span><span class="sxs-lookup"><span data-stu-id="53a62-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="53a62-108">audio</span><span class="sxs-lookup"><span data-stu-id="53a62-108">audio</span></span>             | <span data-ttu-id="53a62-109">Int64</span><span class="sxs-lookup"><span data-stu-id="53a62-109">Int64</span></span>  |
| <span data-ttu-id="53a62-110">video</span><span class="sxs-lookup"><span data-stu-id="53a62-110">video</span></span>             | <span data-ttu-id="53a62-111">Int64</span><span class="sxs-lookup"><span data-stu-id="53a62-111">Int64</span></span>  |
| <span data-ttu-id="53a62-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="53a62-112">reportRefreshDate</span></span> | <span data-ttu-id="53a62-113">日期</span><span class="sxs-lookup"><span data-stu-id="53a62-113">Date</span></span>   |
| <span data-ttu-id="53a62-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="53a62-114">reportDate</span></span>        | <span data-ttu-id="53a62-115">日期</span><span class="sxs-lookup"><span data-stu-id="53a62-115">Date</span></span>   |
| <span data-ttu-id="53a62-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="53a62-116">reportPeriod</span></span>      | <span data-ttu-id="53a62-117">字符串</span><span class="sxs-lookup"><span data-stu-id="53a62-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53a62-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53a62-118">JSON representation</span></span>

<span data-ttu-id="53a62-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53a62-119">The following is a JSON representation of the resource.</span></span>

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


