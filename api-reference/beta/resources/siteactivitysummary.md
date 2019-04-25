---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583597"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="5e2c9-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e2c9-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5e2c9-104">属性</span><span class="sxs-lookup"><span data-stu-id="5e2c9-104">Properties</span></span>

| <span data-ttu-id="5e2c9-105">属性</span><span class="sxs-lookup"><span data-stu-id="5e2c9-105">Property</span></span>          | <span data-ttu-id="5e2c9-106">类型</span><span class="sxs-lookup"><span data-stu-id="5e2c9-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5e2c9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5e2c9-107">reportRefreshDate</span></span> | <span data-ttu-id="5e2c9-108">Date</span><span class="sxs-lookup"><span data-stu-id="5e2c9-108">Date</span></span>   |
| <span data-ttu-id="5e2c9-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="5e2c9-109">viewedOrEdited</span></span>    | <span data-ttu-id="5e2c9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5e2c9-110">Int64</span></span>  |
| <span data-ttu-id="5e2c9-111">保持</span><span class="sxs-lookup"><span data-stu-id="5e2c9-111">synced</span></span>            | <span data-ttu-id="5e2c9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5e2c9-112">Int64</span></span>  |
| <span data-ttu-id="5e2c9-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="5e2c9-113">sharedInternally</span></span>  | <span data-ttu-id="5e2c9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5e2c9-114">Int64</span></span>  |
| <span data-ttu-id="5e2c9-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="5e2c9-115">sharedExternally</span></span>  | <span data-ttu-id="5e2c9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5e2c9-116">Int64</span></span>  |
| <span data-ttu-id="5e2c9-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="5e2c9-117">reportDate</span></span>        | <span data-ttu-id="5e2c9-118">Date</span><span class="sxs-lookup"><span data-stu-id="5e2c9-118">Date</span></span>   |
| <span data-ttu-id="5e2c9-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5e2c9-119">reportPeriod</span></span>      | <span data-ttu-id="5e2c9-120">String</span><span class="sxs-lookup"><span data-stu-id="5e2c9-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e2c9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e2c9-121">JSON representation</span></span>

<span data-ttu-id="5e2c9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e2c9-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
