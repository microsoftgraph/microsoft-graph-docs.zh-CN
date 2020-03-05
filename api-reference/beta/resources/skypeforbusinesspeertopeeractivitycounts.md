---
title: skypeForBusinessPeerToPeerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6ea09965bb598072eda36eb46a2f9edef63de050
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520357"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="d4cad-103">skypeForBusinessPeerToPeerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4cad-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

<span data-ttu-id="d4cad-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d4cad-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d4cad-105">属性</span><span class="sxs-lookup"><span data-stu-id="d4cad-105">Properties</span></span>

| <span data-ttu-id="d4cad-106">属性</span><span class="sxs-lookup"><span data-stu-id="d4cad-106">Property</span></span>          | <span data-ttu-id="d4cad-107">类型</span><span class="sxs-lookup"><span data-stu-id="d4cad-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d4cad-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="d4cad-108">im</span></span>                | <span data-ttu-id="d4cad-109">Int64</span><span class="sxs-lookup"><span data-stu-id="d4cad-109">Int64</span></span>  |
| <span data-ttu-id="d4cad-110">audio</span><span class="sxs-lookup"><span data-stu-id="d4cad-110">audio</span></span>             | <span data-ttu-id="d4cad-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d4cad-111">Int64</span></span>  |
| <span data-ttu-id="d4cad-112">video</span><span class="sxs-lookup"><span data-stu-id="d4cad-112">video</span></span>             | <span data-ttu-id="d4cad-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d4cad-113">Int64</span></span>  |
| <span data-ttu-id="d4cad-114">appSharing</span><span class="sxs-lookup"><span data-stu-id="d4cad-114">appSharing</span></span>        | <span data-ttu-id="d4cad-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d4cad-115">Int64</span></span>  |
| <span data-ttu-id="d4cad-116">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="d4cad-116">fileTransfer</span></span>      | <span data-ttu-id="d4cad-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d4cad-117">Int64</span></span>  |
| <span data-ttu-id="d4cad-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d4cad-118">reportRefreshDate</span></span> | <span data-ttu-id="d4cad-119">日期</span><span class="sxs-lookup"><span data-stu-id="d4cad-119">Date</span></span>   |
| <span data-ttu-id="d4cad-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="d4cad-120">reportDate</span></span>        | <span data-ttu-id="d4cad-121">日期</span><span class="sxs-lookup"><span data-stu-id="d4cad-121">Date</span></span>   |
| <span data-ttu-id="d4cad-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d4cad-122">reportPeriod</span></span>      | <span data-ttu-id="d4cad-123">String</span><span class="sxs-lookup"><span data-stu-id="d4cad-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4cad-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4cad-124">JSON representation</span></span>

<span data-ttu-id="d4cad-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4cad-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
