---
title: plannerChecklistItems 资源类型
description: '**plannerChecklistItemCollection** 资源表示任务上的清单项集合。它是开放类型。它是任务详细信息对象的组成部分。该属性值对中的值是 checklistItem 对象。'
ms.openlocfilehash: 44e64872c34a70062e847889576bd226d4fe51fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045630"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="c6607-106">plannerChecklistItems 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6607-106">plannerChecklistItems resource type</span></span>

> <span data-ttu-id="c6607-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6607-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6607-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6607-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6607-p103">**plannerChecklistItemCollection** 资源表示任务上的清单项集合。它是开放类型。它是[任务详细信息](plannertaskdetails.md)对象的组成部分。该属性值对中的值是 [checklistItem](plannerchecklistitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6607-p103">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task. It is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="c6607-113">属性</span><span class="sxs-lookup"><span data-stu-id="c6607-113">Properties</span></span>
<span data-ttu-id="c6607-p104">开放类型的属性可以由客户端定义。在这种情况下，客户端应将 **GUID** 作为属性，并且其值必须为 [checklistItem](plannerchecklistitem.md) 对象。下面是一个示例。若要删除清单中的项，请将该属性值设置为 `null`。</span><span class="sxs-lookup"><span data-stu-id="c6607-p104">Properties of an Open Type can be defined by the client. In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects. Example is shown below. To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6607-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6607-118">JSON representation</span></span>

<span data-ttu-id="c6607-119">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6607-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<span data-ttu-id="c6607-120">// 示例</span><span class="sxs-lookup"><span data-stu-id="c6607-120">// Example</span></span>

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