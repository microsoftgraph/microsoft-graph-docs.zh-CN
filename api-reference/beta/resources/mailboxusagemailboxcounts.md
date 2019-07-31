---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b9f336e3d23cd84f79af7092463383a030336e13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009858"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="48187-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="48187-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="48187-104">属性</span><span class="sxs-lookup"><span data-stu-id="48187-104">Properties</span></span>

| <span data-ttu-id="48187-105">属性</span><span class="sxs-lookup"><span data-stu-id="48187-105">Property</span></span>          | <span data-ttu-id="48187-106">类型</span><span class="sxs-lookup"><span data-stu-id="48187-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="48187-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="48187-107">reportRefreshDate</span></span> | <span data-ttu-id="48187-108">日期</span><span class="sxs-lookup"><span data-stu-id="48187-108">Date</span></span>   |
| <span data-ttu-id="48187-109">total</span><span class="sxs-lookup"><span data-stu-id="48187-109">total</span></span>             | <span data-ttu-id="48187-110">Int64</span><span class="sxs-lookup"><span data-stu-id="48187-110">Int64</span></span>  |
| <span data-ttu-id="48187-111">工作</span><span class="sxs-lookup"><span data-stu-id="48187-111">active</span></span>            | <span data-ttu-id="48187-112">Int64</span><span class="sxs-lookup"><span data-stu-id="48187-112">Int64</span></span>  |
| <span data-ttu-id="48187-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="48187-113">reportDate</span></span>        | <span data-ttu-id="48187-114">日期</span><span class="sxs-lookup"><span data-stu-id="48187-114">Date</span></span>   |
| <span data-ttu-id="48187-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="48187-115">reportPeriod</span></span>      | <span data-ttu-id="48187-116">String</span><span class="sxs-lookup"><span data-stu-id="48187-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48187-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48187-117">JSON representation</span></span>

<span data-ttu-id="48187-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48187-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
