---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dd30bb496cb6591b3bde11d1c0c38b4099175891
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499587"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="d099d-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d099d-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="d099d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d099d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d099d-105">属性</span><span class="sxs-lookup"><span data-stu-id="d099d-105">Properties</span></span>

| <span data-ttu-id="d099d-106">属性</span><span class="sxs-lookup"><span data-stu-id="d099d-106">Property</span></span>          | <span data-ttu-id="d099d-107">类型</span><span class="sxs-lookup"><span data-stu-id="d099d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d099d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d099d-108">reportRefreshDate</span></span> | <span data-ttu-id="d099d-109">日期</span><span class="sxs-lookup"><span data-stu-id="d099d-109">Date</span></span>   |
| <span data-ttu-id="d099d-110">发送</span><span class="sxs-lookup"><span data-stu-id="d099d-110">send</span></span>              | <span data-ttu-id="d099d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d099d-111">Int64</span></span>  |
| <span data-ttu-id="d099d-112">享受</span><span class="sxs-lookup"><span data-stu-id="d099d-112">receive</span></span>           | <span data-ttu-id="d099d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d099d-113">Int64</span></span>  |
| <span data-ttu-id="d099d-114">自述</span><span class="sxs-lookup"><span data-stu-id="d099d-114">read</span></span>              | <span data-ttu-id="d099d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d099d-115">Int64</span></span>  |
| <span data-ttu-id="d099d-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="d099d-116">reportDate</span></span>        | <span data-ttu-id="d099d-117">日期</span><span class="sxs-lookup"><span data-stu-id="d099d-117">Date</span></span>   |
| <span data-ttu-id="d099d-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d099d-118">reportPeriod</span></span>      | <span data-ttu-id="d099d-119">String</span><span class="sxs-lookup"><span data-stu-id="d099d-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d099d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d099d-120">JSON representation</span></span>

<span data-ttu-id="d099d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d099d-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
