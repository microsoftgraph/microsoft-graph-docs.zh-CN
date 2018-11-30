---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 959d6602cec98f7351ec3d9819fb9a59599d3e6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045341"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="36c06-103">oneDriveUsageAccountCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="36c06-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="36c06-104">属性</span><span class="sxs-lookup"><span data-stu-id="36c06-104">Properties</span></span>

| <span data-ttu-id="36c06-105">属性</span><span class="sxs-lookup"><span data-stu-id="36c06-105">Property</span></span>          | <span data-ttu-id="36c06-106">类型</span><span class="sxs-lookup"><span data-stu-id="36c06-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="36c06-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="36c06-107">reportRefreshDate</span></span> | <span data-ttu-id="36c06-108">日期</span><span class="sxs-lookup"><span data-stu-id="36c06-108">Date</span></span>   |
| <span data-ttu-id="36c06-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="36c06-109">siteType</span></span>          | <span data-ttu-id="36c06-110">字符串</span><span class="sxs-lookup"><span data-stu-id="36c06-110">String</span></span> |
| <span data-ttu-id="36c06-111">total</span><span class="sxs-lookup"><span data-stu-id="36c06-111">total</span></span>             | <span data-ttu-id="36c06-112">Int64</span><span class="sxs-lookup"><span data-stu-id="36c06-112">Int64</span></span>  |
| <span data-ttu-id="36c06-113">活动</span><span class="sxs-lookup"><span data-stu-id="36c06-113">active</span></span>            | <span data-ttu-id="36c06-114">Int64</span><span class="sxs-lookup"><span data-stu-id="36c06-114">Int64</span></span>  |
| <span data-ttu-id="36c06-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="36c06-115">reportDate</span></span>        | <span data-ttu-id="36c06-116">日期</span><span class="sxs-lookup"><span data-stu-id="36c06-116">Date</span></span>   |
| <span data-ttu-id="36c06-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="36c06-117">reportPeriod</span></span>      | <span data-ttu-id="36c06-118">String</span><span class="sxs-lookup"><span data-stu-id="36c06-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="36c06-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36c06-119">JSON representation</span></span>

<span data-ttu-id="36c06-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36c06-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
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
