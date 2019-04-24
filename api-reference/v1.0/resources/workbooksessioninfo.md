---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456834"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="19399-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="19399-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="19399-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="19399-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="19399-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19399-105">JSON representation</span></span>

<span data-ttu-id="19399-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19399-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="19399-107">属性</span><span class="sxs-lookup"><span data-stu-id="19399-107">Properties</span></span>

| <span data-ttu-id="19399-108">属性</span><span class="sxs-lookup"><span data-stu-id="19399-108">Property</span></span> | <span data-ttu-id="19399-109">类型</span><span class="sxs-lookup"><span data-stu-id="19399-109">Type</span></span>  | <span data-ttu-id="19399-110">说明</span><span class="sxs-lookup"><span data-stu-id="19399-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="19399-111">id</span><span class="sxs-lookup"><span data-stu-id="19399-111">id</span></span>  | <span data-ttu-id="19399-112">string</span><span class="sxs-lookup"><span data-stu-id="19399-112">string</span></span> | <span data-ttu-id="19399-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="19399-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="19399-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="19399-114">persistChanges</span></span> | <span data-ttu-id="19399-115">布尔</span><span class="sxs-lookup"><span data-stu-id="19399-115">boolean</span></span> |  <span data-ttu-id="19399-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="19399-116">`true` for persistent session.</span></span> <span data-ttu-id="19399-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="19399-117">`false` for non-persistent session (view mode)</span></span> |

