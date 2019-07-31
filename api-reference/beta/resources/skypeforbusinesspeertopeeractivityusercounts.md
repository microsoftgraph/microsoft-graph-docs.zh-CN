---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: baafa0ba3ddf59efdfe049c324b21f1294b155f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964793"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="b846f-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b846f-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b846f-104">属性</span><span class="sxs-lookup"><span data-stu-id="b846f-104">Properties</span></span>

| <span data-ttu-id="b846f-105">属性</span><span class="sxs-lookup"><span data-stu-id="b846f-105">Property</span></span>          | <span data-ttu-id="b846f-106">类型</span><span class="sxs-lookup"><span data-stu-id="b846f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b846f-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="b846f-107">im</span></span>                | <span data-ttu-id="b846f-108">Int64</span><span class="sxs-lookup"><span data-stu-id="b846f-108">Int64</span></span>  |
| <span data-ttu-id="b846f-109">audio</span><span class="sxs-lookup"><span data-stu-id="b846f-109">audio</span></span>             | <span data-ttu-id="b846f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b846f-110">Int64</span></span>  |
| <span data-ttu-id="b846f-111">video</span><span class="sxs-lookup"><span data-stu-id="b846f-111">video</span></span>             | <span data-ttu-id="b846f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b846f-112">Int64</span></span>  |
| <span data-ttu-id="b846f-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="b846f-113">appSharing</span></span>        | <span data-ttu-id="b846f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b846f-114">Int64</span></span>  |
| <span data-ttu-id="b846f-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="b846f-115">fileTransfer</span></span>      | <span data-ttu-id="b846f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b846f-116">Int64</span></span>  |
| <span data-ttu-id="b846f-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b846f-117">reportRefreshDate</span></span> | <span data-ttu-id="b846f-118">日期</span><span class="sxs-lookup"><span data-stu-id="b846f-118">Date</span></span>   |
| <span data-ttu-id="b846f-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="b846f-119">reportDate</span></span>        | <span data-ttu-id="b846f-120">日期</span><span class="sxs-lookup"><span data-stu-id="b846f-120">Date</span></span>   |
| <span data-ttu-id="b846f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b846f-121">reportPeriod</span></span>      | <span data-ttu-id="b846f-122">String</span><span class="sxs-lookup"><span data-stu-id="b846f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b846f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b846f-123">JSON representation</span></span>

<span data-ttu-id="b846f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b846f-124">The following is a JSON representation of the resource.</span></span>

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
