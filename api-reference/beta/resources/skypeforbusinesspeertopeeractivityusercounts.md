---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2df9cd9e7887c955190c8478cd8075a077929133
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520455"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="b373f-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b373f-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

<span data-ttu-id="b373f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b373f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b373f-105">属性</span><span class="sxs-lookup"><span data-stu-id="b373f-105">Properties</span></span>

| <span data-ttu-id="b373f-106">属性</span><span class="sxs-lookup"><span data-stu-id="b373f-106">Property</span></span>          | <span data-ttu-id="b373f-107">类型</span><span class="sxs-lookup"><span data-stu-id="b373f-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b373f-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="b373f-108">im</span></span>                | <span data-ttu-id="b373f-109">Int64</span><span class="sxs-lookup"><span data-stu-id="b373f-109">Int64</span></span>  |
| <span data-ttu-id="b373f-110">audio</span><span class="sxs-lookup"><span data-stu-id="b373f-110">audio</span></span>             | <span data-ttu-id="b373f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b373f-111">Int64</span></span>  |
| <span data-ttu-id="b373f-112">video</span><span class="sxs-lookup"><span data-stu-id="b373f-112">video</span></span>             | <span data-ttu-id="b373f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b373f-113">Int64</span></span>  |
| <span data-ttu-id="b373f-114">appSharing</span><span class="sxs-lookup"><span data-stu-id="b373f-114">appSharing</span></span>        | <span data-ttu-id="b373f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b373f-115">Int64</span></span>  |
| <span data-ttu-id="b373f-116">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="b373f-116">fileTransfer</span></span>      | <span data-ttu-id="b373f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b373f-117">Int64</span></span>  |
| <span data-ttu-id="b373f-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b373f-118">reportRefreshDate</span></span> | <span data-ttu-id="b373f-119">日期</span><span class="sxs-lookup"><span data-stu-id="b373f-119">Date</span></span>   |
| <span data-ttu-id="b373f-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="b373f-120">reportDate</span></span>        | <span data-ttu-id="b373f-121">日期</span><span class="sxs-lookup"><span data-stu-id="b373f-121">Date</span></span>   |
| <span data-ttu-id="b373f-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b373f-122">reportPeriod</span></span>      | <span data-ttu-id="b373f-123">String</span><span class="sxs-lookup"><span data-stu-id="b373f-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b373f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b373f-124">JSON representation</span></span>

<span data-ttu-id="b373f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b373f-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
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
