---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 710265ba7352b2c589b4096139714ecb192a8fb8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522370"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="0b47a-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b47a-103">oneDriveUsageFileCounts resource type</span></span>

<span data-ttu-id="0b47a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0b47a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0b47a-105">属性</span><span class="sxs-lookup"><span data-stu-id="0b47a-105">Properties</span></span>

| <span data-ttu-id="0b47a-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b47a-106">Property</span></span>          | <span data-ttu-id="0b47a-107">类型</span><span class="sxs-lookup"><span data-stu-id="0b47a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0b47a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0b47a-108">reportRefreshDate</span></span> | <span data-ttu-id="0b47a-109">日期</span><span class="sxs-lookup"><span data-stu-id="0b47a-109">Date</span></span>   |
| <span data-ttu-id="0b47a-110">siteType</span><span class="sxs-lookup"><span data-stu-id="0b47a-110">siteType</span></span>          | <span data-ttu-id="0b47a-111">String</span><span class="sxs-lookup"><span data-stu-id="0b47a-111">String</span></span> |
| <span data-ttu-id="0b47a-112">total</span><span class="sxs-lookup"><span data-stu-id="0b47a-112">total</span></span>             | <span data-ttu-id="0b47a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0b47a-113">Int64</span></span>  |
| <span data-ttu-id="0b47a-114">工作</span><span class="sxs-lookup"><span data-stu-id="0b47a-114">active</span></span>            | <span data-ttu-id="0b47a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="0b47a-115">Int64</span></span>  |
| <span data-ttu-id="0b47a-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="0b47a-116">reportDate</span></span>        | <span data-ttu-id="0b47a-117">日期</span><span class="sxs-lookup"><span data-stu-id="0b47a-117">Date</span></span>   |
| <span data-ttu-id="0b47a-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0b47a-118">reportPeriod</span></span>      | <span data-ttu-id="0b47a-119">String</span><span class="sxs-lookup"><span data-stu-id="0b47a-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b47a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b47a-120">JSON representation</span></span>

<span data-ttu-id="0b47a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b47a-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
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
