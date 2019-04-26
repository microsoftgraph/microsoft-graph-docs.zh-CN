---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: dd70875c272f63a1c9a7988c001225c2d200e0c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554847"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="2bc44-103">oneDriveUsageAccountCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bc44-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2bc44-104">属性</span><span class="sxs-lookup"><span data-stu-id="2bc44-104">Properties</span></span>

| <span data-ttu-id="2bc44-105">属性</span><span class="sxs-lookup"><span data-stu-id="2bc44-105">Property</span></span>          | <span data-ttu-id="2bc44-106">类型</span><span class="sxs-lookup"><span data-stu-id="2bc44-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2bc44-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2bc44-107">reportRefreshDate</span></span> | <span data-ttu-id="2bc44-108">Date</span><span class="sxs-lookup"><span data-stu-id="2bc44-108">Date</span></span>   |
| <span data-ttu-id="2bc44-109">siteType</span><span class="sxs-lookup"><span data-stu-id="2bc44-109">siteType</span></span>          | <span data-ttu-id="2bc44-110">String</span><span class="sxs-lookup"><span data-stu-id="2bc44-110">String</span></span> |
| <span data-ttu-id="2bc44-111">total</span><span class="sxs-lookup"><span data-stu-id="2bc44-111">total</span></span>             | <span data-ttu-id="2bc44-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2bc44-112">Int64</span></span>  |
| <span data-ttu-id="2bc44-113">工作</span><span class="sxs-lookup"><span data-stu-id="2bc44-113">active</span></span>            | <span data-ttu-id="2bc44-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2bc44-114">Int64</span></span>  |
| <span data-ttu-id="2bc44-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="2bc44-115">reportDate</span></span>        | <span data-ttu-id="2bc44-116">Date</span><span class="sxs-lookup"><span data-stu-id="2bc44-116">Date</span></span>   |
| <span data-ttu-id="2bc44-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2bc44-117">reportPeriod</span></span>      | <span data-ttu-id="2bc44-118">String</span><span class="sxs-lookup"><span data-stu-id="2bc44-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2bc44-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bc44-119">JSON representation</span></span>

<span data-ttu-id="2bc44-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bc44-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
