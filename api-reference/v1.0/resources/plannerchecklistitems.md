---
title: plannerChecklistItems 资源类型
description: '**plannerChecklistItemCollection**资源表示任务上的检查表项的集合。 它是开放类型。 它是任务详细信息对象的一部分。 属性-值对中的值是 checklistItem 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 17c1d8c0529e0d85ebc784d25c2dc284f1775c0f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462282"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="0aee0-106">plannerChecklistItems 资源类型</span><span class="sxs-lookup"><span data-stu-id="0aee0-106">plannerChecklistItems resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aee0-107">**plannerChecklistItemCollection**资源表示任务上的检查表项的集合。</span><span class="sxs-lookup"><span data-stu-id="0aee0-107">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task.</span></span> <span data-ttu-id="0aee0-108">它是开放类型。</span><span class="sxs-lookup"><span data-stu-id="0aee0-108">It is an Open Type.</span></span> <span data-ttu-id="0aee0-109">它是[任务详细信息](plannertaskdetails.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="0aee0-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="0aee0-110">属性-值对中的值是[checklistItem](plannerchecklistitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0aee0-110">The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="0aee0-111">属性</span><span class="sxs-lookup"><span data-stu-id="0aee0-111">Properties</span></span>
<span data-ttu-id="0aee0-112">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="0aee0-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="0aee0-113">在这种情况下, 客户端应将**guid**作为属性提供, 并且它们的值必须是[checklistItem](plannerchecklistitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0aee0-113">In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects.</span></span> <span data-ttu-id="0aee0-114">示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0aee0-114">Example is shown below.</span></span> <span data-ttu-id="0aee0-115">若要删除检查表中的项目, 请将该属性的值`null`设置为。</span><span class="sxs-lookup"><span data-stu-id="0aee0-115">To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0aee0-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0aee0-116">JSON representation</span></span>

<span data-ttu-id="0aee0-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aee0-117">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="0aee0-118">示例</span><span class="sxs-lookup"><span data-stu-id="0aee0-118">// Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitems.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
