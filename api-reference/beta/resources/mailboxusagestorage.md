---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 40cc5f9b9cab7f17e185619d7fccdec028ae6250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522832"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="a5929-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5929-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="a5929-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a5929-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a5929-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5929-105">Properties</span></span>

| <span data-ttu-id="a5929-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5929-106">Property</span></span>           | <span data-ttu-id="a5929-107">类型</span><span class="sxs-lookup"><span data-stu-id="a5929-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="a5929-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a5929-108">reportRefreshDate</span></span>  | <span data-ttu-id="a5929-109">日期</span><span class="sxs-lookup"><span data-stu-id="a5929-109">Date</span></span>   |
| <span data-ttu-id="a5929-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="a5929-110">storageUsedInBytes</span></span> | <span data-ttu-id="a5929-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a5929-111">Int64</span></span>  |
| <span data-ttu-id="a5929-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="a5929-112">reportDate</span></span>         | <span data-ttu-id="a5929-113">日期</span><span class="sxs-lookup"><span data-stu-id="a5929-113">Date</span></span>   |
| <span data-ttu-id="a5929-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a5929-114">reportPeriod</span></span>       | <span data-ttu-id="a5929-115">String</span><span class="sxs-lookup"><span data-stu-id="a5929-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5929-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5929-116">JSON representation</span></span>

<span data-ttu-id="a5929-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5929-117">The following is a JSON representation of the resource.</span></span>

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
