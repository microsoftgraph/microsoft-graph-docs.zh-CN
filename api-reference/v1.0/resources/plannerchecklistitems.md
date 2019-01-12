---
title: plannerChecklistItems 资源类型
description: '**plannerChecklistItemCollection** 资源表示任务上的清单项集合。它是开放类型。它是任务详细信息对象的组成部分。该属性值对中的值是 checklistItem 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 17c1d8c0529e0d85ebc784d25c2dc284f1775c0f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982699"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="82524-106">plannerChecklistItems 资源类型</span><span class="sxs-lookup"><span data-stu-id="82524-106">plannerChecklistItems resource type</span></span>

<span data-ttu-id="82524-p102">**plannerChecklistItemCollection** 资源表示任务上的清单项集合。它是开放类型。它是[任务详细信息](plannertaskdetails.md)对象的组成部分。该属性值对中的值是 [checklistItem](plannerchecklistitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82524-p102">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task. It is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="82524-111">属性</span><span class="sxs-lookup"><span data-stu-id="82524-111">Properties</span></span>
<span data-ttu-id="82524-p103">开放类型的属性可以由客户端定义。在这种情况下，客户端应将 **GUID** 作为属性，并且其值必须为 [checklistItem](plannerchecklistitem.md) 对象。下面是一个示例。若要删除清单中的项，请将该属性值设置为 `null`。</span><span class="sxs-lookup"><span data-stu-id="82524-p103">Properties of an Open Type can be defined by the client. In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects. Example is shown below. To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82524-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82524-116">JSON representation</span></span>

<span data-ttu-id="82524-117">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82524-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerChecklistItems"
}-->

```json
{
  "String-value":
  {
    "isChecked": true,
    "lastModifiedBy": "String-value",
    "lastModifiedByDateTime": "String(timestamp)",
    "orderHint": "String-value",
    "title": "String-value"
  }
}
```
<span data-ttu-id="82524-118">// 示例</span><span class="sxs-lookup"><span data-stu-id="82524-118">// Example</span></span>

```json
{
  "3a73c9dd-fb47-4230-9c0f-b80788fb0f9b": // client-generated GUID
  {
    "@odata.type": "microsoft.graph.checklistItem", // required in PATCH requests to edit the checklist on a task
    "isChecked": true,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0009005756397228702",
    "title": "Get stamps"
  },
  "5f36f5b2-1ec0-4c48-9c75-ed59429516c5":
  {
     "@odata.type": "microsoft.graph.checklistItem",
    "isChecked": false,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0004105723397228784",
    "title": "Mail card at UPS"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
