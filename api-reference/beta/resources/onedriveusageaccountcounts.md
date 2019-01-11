---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 021d0089969a6272996f604630b900af61a7a5a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868192"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="a3b99-103">oneDriveUsageAccountCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3b99-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a3b99-104">属性</span><span class="sxs-lookup"><span data-stu-id="a3b99-104">Properties</span></span>

| <span data-ttu-id="a3b99-105">属性</span><span class="sxs-lookup"><span data-stu-id="a3b99-105">Property</span></span>          | <span data-ttu-id="a3b99-106">类型</span><span class="sxs-lookup"><span data-stu-id="a3b99-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a3b99-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a3b99-107">reportRefreshDate</span></span> | <span data-ttu-id="a3b99-108">日期</span><span class="sxs-lookup"><span data-stu-id="a3b99-108">Date</span></span>   |
| <span data-ttu-id="a3b99-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="a3b99-109">siteType</span></span>          | <span data-ttu-id="a3b99-110">字符串</span><span class="sxs-lookup"><span data-stu-id="a3b99-110">String</span></span> |
| <span data-ttu-id="a3b99-111">total</span><span class="sxs-lookup"><span data-stu-id="a3b99-111">total</span></span>             | <span data-ttu-id="a3b99-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a3b99-112">Int64</span></span>  |
| <span data-ttu-id="a3b99-113">活动</span><span class="sxs-lookup"><span data-stu-id="a3b99-113">active</span></span>            | <span data-ttu-id="a3b99-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a3b99-114">Int64</span></span>  |
| <span data-ttu-id="a3b99-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="a3b99-115">reportDate</span></span>        | <span data-ttu-id="a3b99-116">日期</span><span class="sxs-lookup"><span data-stu-id="a3b99-116">Date</span></span>   |
| <span data-ttu-id="a3b99-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a3b99-117">reportPeriod</span></span>      | <span data-ttu-id="a3b99-118">String</span><span class="sxs-lookup"><span data-stu-id="a3b99-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a3b99-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3b99-119">JSON representation</span></span>

<span data-ttu-id="a3b99-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3b99-120">The following is a JSON representation of the resource.</span></span>

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
