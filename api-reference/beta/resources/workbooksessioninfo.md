---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
ms.openlocfilehash: c04afe17c10edd8b136465d6d7ae3dbedb6307ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044826"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="79edd-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="79edd-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="79edd-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="79edd-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="79edd-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79edd-105">JSON representation</span></span>

<span data-ttu-id="79edd-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79edd-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="79edd-107">属性</span><span class="sxs-lookup"><span data-stu-id="79edd-107">Properties</span></span>

| <span data-ttu-id="79edd-108">属性</span><span class="sxs-lookup"><span data-stu-id="79edd-108">Property</span></span> | <span data-ttu-id="79edd-109">类型</span><span class="sxs-lookup"><span data-stu-id="79edd-109">Type</span></span>  | <span data-ttu-id="79edd-110">说明</span><span class="sxs-lookup"><span data-stu-id="79edd-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="79edd-111">ID</span><span class="sxs-lookup"><span data-stu-id="79edd-111">id</span></span>  | <span data-ttu-id="79edd-112">string</span><span class="sxs-lookup"><span data-stu-id="79edd-112">string</span></span> | <span data-ttu-id="79edd-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="79edd-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="79edd-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="79edd-114">persistChanges</span></span> | <span data-ttu-id="79edd-115">string</span><span class="sxs-lookup"><span data-stu-id="79edd-115">string</span></span> |  <span data-ttu-id="79edd-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="79edd-116">`true` for persistent session.</span></span> <span data-ttu-id="79edd-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="79edd-117">`false` for non-persistent session (view mode)</span></span> |

