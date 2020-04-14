---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 32a2aba9aab207cede8118baed4435708995192a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473430"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="f06db-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f06db-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="f06db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f06db-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f06db-105">属性</span><span class="sxs-lookup"><span data-stu-id="f06db-105">Properties</span></span>

| <span data-ttu-id="f06db-106">属性</span><span class="sxs-lookup"><span data-stu-id="f06db-106">Property</span></span>          | <span data-ttu-id="f06db-107">类型</span><span class="sxs-lookup"><span data-stu-id="f06db-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f06db-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f06db-108">reportRefreshDate</span></span> | <span data-ttu-id="f06db-109">日期</span><span class="sxs-lookup"><span data-stu-id="f06db-109">Date</span></span>   |
| <span data-ttu-id="f06db-110">total</span><span class="sxs-lookup"><span data-stu-id="f06db-110">total</span></span>             | <span data-ttu-id="f06db-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f06db-111">Int64</span></span>  |
| <span data-ttu-id="f06db-112">工作</span><span class="sxs-lookup"><span data-stu-id="f06db-112">active</span></span>            | <span data-ttu-id="f06db-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f06db-113">Int64</span></span>  |
| <span data-ttu-id="f06db-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="f06db-114">reportDate</span></span>        | <span data-ttu-id="f06db-115">日期</span><span class="sxs-lookup"><span data-stu-id="f06db-115">Date</span></span>   |
| <span data-ttu-id="f06db-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f06db-116">reportPeriod</span></span>      | <span data-ttu-id="f06db-117">String</span><span class="sxs-lookup"><span data-stu-id="f06db-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f06db-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f06db-118">JSON representation</span></span>

<span data-ttu-id="f06db-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f06db-119">The following is a JSON representation of the resource.</span></span>

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
