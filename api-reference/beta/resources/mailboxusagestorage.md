---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4fedb101fbab2b14ec2d1ada1e02faa4bc729e0d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982199"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="fdb9f-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdb9f-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="fdb9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdb9f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fdb9f-105">属性</span><span class="sxs-lookup"><span data-stu-id="fdb9f-105">Properties</span></span>

| <span data-ttu-id="fdb9f-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdb9f-106">Property</span></span>           | <span data-ttu-id="fdb9f-107">类型</span><span class="sxs-lookup"><span data-stu-id="fdb9f-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="fdb9f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fdb9f-108">reportRefreshDate</span></span>  | <span data-ttu-id="fdb9f-109">日期</span><span class="sxs-lookup"><span data-stu-id="fdb9f-109">Date</span></span>   |
| <span data-ttu-id="fdb9f-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="fdb9f-110">storageUsedInBytes</span></span> | <span data-ttu-id="fdb9f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="fdb9f-111">Int64</span></span>  |
| <span data-ttu-id="fdb9f-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="fdb9f-112">reportDate</span></span>         | <span data-ttu-id="fdb9f-113">日期</span><span class="sxs-lookup"><span data-stu-id="fdb9f-113">Date</span></span>   |
| <span data-ttu-id="fdb9f-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fdb9f-114">reportPeriod</span></span>       | <span data-ttu-id="fdb9f-115">String</span><span class="sxs-lookup"><span data-stu-id="fdb9f-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fdb9f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdb9f-116">JSON representation</span></span>

<span data-ttu-id="fdb9f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdb9f-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


