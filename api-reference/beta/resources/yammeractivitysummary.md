---
title: yammerActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 14cd88848e85d8260ccdadfbec8925faf4acba85
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006988"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="4e94e-103">yammerActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e94e-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4e94e-104">属性</span><span class="sxs-lookup"><span data-stu-id="4e94e-104">Properties</span></span>

| <span data-ttu-id="4e94e-105">属性</span><span class="sxs-lookup"><span data-stu-id="4e94e-105">Property</span></span>          | <span data-ttu-id="4e94e-106">类型</span><span class="sxs-lookup"><span data-stu-id="4e94e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4e94e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4e94e-107">reportRefreshDate</span></span> | <span data-ttu-id="4e94e-108">日期</span><span class="sxs-lookup"><span data-stu-id="4e94e-108">Date</span></span>   |
| <span data-ttu-id="4e94e-109">人</span><span class="sxs-lookup"><span data-stu-id="4e94e-109">liked</span></span>             | <span data-ttu-id="4e94e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4e94e-110">Int64</span></span>  |
| <span data-ttu-id="4e94e-111">发布</span><span class="sxs-lookup"><span data-stu-id="4e94e-111">posted</span></span>            | <span data-ttu-id="4e94e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4e94e-112">Int64</span></span>  |
| <span data-ttu-id="4e94e-113">自述</span><span class="sxs-lookup"><span data-stu-id="4e94e-113">read</span></span>              | <span data-ttu-id="4e94e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4e94e-114">Int64</span></span>  |
| <span data-ttu-id="4e94e-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="4e94e-115">reportDate</span></span>        | <span data-ttu-id="4e94e-116">日期</span><span class="sxs-lookup"><span data-stu-id="4e94e-116">Date</span></span>   |
| <span data-ttu-id="4e94e-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4e94e-117">reportPeriod</span></span>      | <span data-ttu-id="4e94e-118">String</span><span class="sxs-lookup"><span data-stu-id="4e94e-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e94e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e94e-119">JSON representation</span></span>

<span data-ttu-id="4e94e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e94e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
