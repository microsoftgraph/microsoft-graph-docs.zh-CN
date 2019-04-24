---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503882"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="1823d-103">skypeForBusinessPeerToPeerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="1823d-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1823d-104">属性</span><span class="sxs-lookup"><span data-stu-id="1823d-104">Properties</span></span>

| <span data-ttu-id="1823d-105">属性</span><span class="sxs-lookup"><span data-stu-id="1823d-105">Property</span></span>          | <span data-ttu-id="1823d-106">类型</span><span class="sxs-lookup"><span data-stu-id="1823d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1823d-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="1823d-107">im</span></span>                | <span data-ttu-id="1823d-108">Int64</span><span class="sxs-lookup"><span data-stu-id="1823d-108">Int64</span></span>  |
| <span data-ttu-id="1823d-109">audio</span><span class="sxs-lookup"><span data-stu-id="1823d-109">audio</span></span>             | <span data-ttu-id="1823d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1823d-110">Int64</span></span>  |
| <span data-ttu-id="1823d-111">video</span><span class="sxs-lookup"><span data-stu-id="1823d-111">video</span></span>             | <span data-ttu-id="1823d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1823d-112">Int64</span></span>  |
| <span data-ttu-id="1823d-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="1823d-113">appSharing</span></span>        | <span data-ttu-id="1823d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1823d-114">Int64</span></span>  |
| <span data-ttu-id="1823d-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="1823d-115">fileTransfer</span></span>      | <span data-ttu-id="1823d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1823d-116">Int64</span></span>  |
| <span data-ttu-id="1823d-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1823d-117">reportRefreshDate</span></span> | <span data-ttu-id="1823d-118">Date</span><span class="sxs-lookup"><span data-stu-id="1823d-118">Date</span></span>   |
| <span data-ttu-id="1823d-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="1823d-119">reportDate</span></span>        | <span data-ttu-id="1823d-120">Date</span><span class="sxs-lookup"><span data-stu-id="1823d-120">Date</span></span>   |
| <span data-ttu-id="1823d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1823d-121">reportPeriod</span></span>      | <span data-ttu-id="1823d-122">字符串</span><span class="sxs-lookup"><span data-stu-id="1823d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1823d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1823d-123">JSON representation</span></span>

<span data-ttu-id="1823d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1823d-124">The following is a JSON representation of the resource.</span></span>

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
