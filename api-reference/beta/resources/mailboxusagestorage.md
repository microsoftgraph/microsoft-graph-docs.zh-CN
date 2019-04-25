---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524543"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="e8adc-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8adc-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e8adc-104">属性</span><span class="sxs-lookup"><span data-stu-id="e8adc-104">Properties</span></span>

| <span data-ttu-id="e8adc-105">属性</span><span class="sxs-lookup"><span data-stu-id="e8adc-105">Property</span></span>           | <span data-ttu-id="e8adc-106">类型</span><span class="sxs-lookup"><span data-stu-id="e8adc-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="e8adc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e8adc-107">reportRefreshDate</span></span>  | <span data-ttu-id="e8adc-108">Date</span><span class="sxs-lookup"><span data-stu-id="e8adc-108">Date</span></span>   |
| <span data-ttu-id="e8adc-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="e8adc-109">storageUsedInBytes</span></span> | <span data-ttu-id="e8adc-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e8adc-110">Int64</span></span>  |
| <span data-ttu-id="e8adc-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="e8adc-111">reportDate</span></span>         | <span data-ttu-id="e8adc-112">Date</span><span class="sxs-lookup"><span data-stu-id="e8adc-112">Date</span></span>   |
| <span data-ttu-id="e8adc-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e8adc-113">reportPeriod</span></span>       | <span data-ttu-id="e8adc-114">String</span><span class="sxs-lookup"><span data-stu-id="e8adc-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e8adc-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8adc-115">JSON representation</span></span>

<span data-ttu-id="e8adc-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8adc-116">The following is a JSON representation of the resource.</span></span>

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
