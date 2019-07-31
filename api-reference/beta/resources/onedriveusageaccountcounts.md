---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: bafc7ae26af6c94d61febb30c5a121f6f22ec7f0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009410"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="88c9b-103">oneDriveUsageAccountCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="88c9b-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="88c9b-104">属性</span><span class="sxs-lookup"><span data-stu-id="88c9b-104">Properties</span></span>

| <span data-ttu-id="88c9b-105">属性</span><span class="sxs-lookup"><span data-stu-id="88c9b-105">Property</span></span>          | <span data-ttu-id="88c9b-106">类型</span><span class="sxs-lookup"><span data-stu-id="88c9b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="88c9b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="88c9b-107">reportRefreshDate</span></span> | <span data-ttu-id="88c9b-108">日期</span><span class="sxs-lookup"><span data-stu-id="88c9b-108">Date</span></span>   |
| <span data-ttu-id="88c9b-109">siteType</span><span class="sxs-lookup"><span data-stu-id="88c9b-109">siteType</span></span>          | <span data-ttu-id="88c9b-110">String</span><span class="sxs-lookup"><span data-stu-id="88c9b-110">String</span></span> |
| <span data-ttu-id="88c9b-111">total</span><span class="sxs-lookup"><span data-stu-id="88c9b-111">total</span></span>             | <span data-ttu-id="88c9b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="88c9b-112">Int64</span></span>  |
| <span data-ttu-id="88c9b-113">工作</span><span class="sxs-lookup"><span data-stu-id="88c9b-113">active</span></span>            | <span data-ttu-id="88c9b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="88c9b-114">Int64</span></span>  |
| <span data-ttu-id="88c9b-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="88c9b-115">reportDate</span></span>        | <span data-ttu-id="88c9b-116">日期</span><span class="sxs-lookup"><span data-stu-id="88c9b-116">Date</span></span>   |
| <span data-ttu-id="88c9b-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="88c9b-117">reportPeriod</span></span>      | <span data-ttu-id="88c9b-118">String</span><span class="sxs-lookup"><span data-stu-id="88c9b-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88c9b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88c9b-119">JSON representation</span></span>

<span data-ttu-id="88c9b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88c9b-120">The following is a JSON representation of the resource.</span></span>

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
