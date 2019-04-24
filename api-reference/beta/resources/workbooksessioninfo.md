---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453281"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="7546f-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="7546f-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="7546f-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="7546f-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7546f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7546f-105">JSON representation</span></span>

<span data-ttu-id="7546f-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7546f-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7546f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7546f-107">Properties</span></span>

| <span data-ttu-id="7546f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7546f-108">Property</span></span> | <span data-ttu-id="7546f-109">类型</span><span class="sxs-lookup"><span data-stu-id="7546f-109">Type</span></span>  | <span data-ttu-id="7546f-110">说明</span><span class="sxs-lookup"><span data-stu-id="7546f-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="7546f-111">id</span><span class="sxs-lookup"><span data-stu-id="7546f-111">id</span></span>  | <span data-ttu-id="7546f-112">string</span><span class="sxs-lookup"><span data-stu-id="7546f-112">string</span></span> | <span data-ttu-id="7546f-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="7546f-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="7546f-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="7546f-114">persistChanges</span></span> | <span data-ttu-id="7546f-115">string</span><span class="sxs-lookup"><span data-stu-id="7546f-115">string</span></span> |  <span data-ttu-id="7546f-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="7546f-116">`true` for persistent session.</span></span> <span data-ttu-id="7546f-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="7546f-117">`false` for non-persistent session (view mode)</span></span> |

