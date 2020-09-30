---
title: directorySizeQuota 资源类型
description: 表示公司的已用和总目录配额。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8f5f172cb8f090b71b7e0fd3c89151668c167afd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315597"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="c5ba0-103">directorySizeQuota 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5ba0-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5ba0-104">表示公司的已用和总目录配额。</span><span class="sxs-lookup"><span data-stu-id="c5ba0-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="c5ba0-105">属性</span><span class="sxs-lookup"><span data-stu-id="c5ba0-105">Properties</span></span>
| <span data-ttu-id="c5ba0-106">属性</span><span class="sxs-lookup"><span data-stu-id="c5ba0-106">Property</span></span>   | <span data-ttu-id="c5ba0-107">类型</span><span class="sxs-lookup"><span data-stu-id="c5ba0-107">Type</span></span>|<span data-ttu-id="c5ba0-108">说明</span><span class="sxs-lookup"><span data-stu-id="c5ba0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5ba0-109">使用的内容</span><span class="sxs-lookup"><span data-stu-id="c5ba0-109">used</span></span>|<span data-ttu-id="c5ba0-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c5ba0-110">Int32</span></span>| <span data-ttu-id="c5ba0-111">已用的目录配额量。</span><span class="sxs-lookup"><span data-stu-id="c5ba0-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="c5ba0-112">total</span><span class="sxs-lookup"><span data-stu-id="c5ba0-112">total</span></span>|<span data-ttu-id="c5ba0-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c5ba0-113">Int32</span></span>| <span data-ttu-id="c5ba0-114">目录配额总量。</span><span class="sxs-lookup"><span data-stu-id="c5ba0-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5ba0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5ba0-115">JSON representation</span></span>

<span data-ttu-id="c5ba0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5ba0-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
