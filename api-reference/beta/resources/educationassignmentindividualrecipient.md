---
title: educationAssignmentIndividualRecipient 资源类型
description: '在 assignTo 属性中使用。 当设置为 "单个收件人列表" 时，课程中的 "选定学生" 将 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 695145ae8819efc66df29d752e7a95101c9fef9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013712"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="cd629-104">educationAssignmentIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd629-104">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="cd629-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd629-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd629-106">在 [assignTo](educationassignment.md) 属性中使用。</span><span class="sxs-lookup"><span data-stu-id="cd629-106">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="cd629-107">如果设置为 "单个收件人列表"，则在发布工作分配时，类中的所选学生将收到提交对象。</span><span class="sxs-lookup"><span data-stu-id="cd629-107">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="cd629-108">此资源是 [educationAssignmentRecipient](educationassignmentrecipient.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="cd629-108">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cd629-109">属性</span><span class="sxs-lookup"><span data-stu-id="cd629-109">Properties</span></span>
| <span data-ttu-id="cd629-110">属性</span><span class="sxs-lookup"><span data-stu-id="cd629-110">Property</span></span>     | <span data-ttu-id="cd629-111">类型</span><span class="sxs-lookup"><span data-stu-id="cd629-111">Type</span></span>   |<span data-ttu-id="cd629-112">说明</span><span class="sxs-lookup"><span data-stu-id="cd629-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd629-113">recipients</span><span class="sxs-lookup"><span data-stu-id="cd629-113">recipients</span></span>|<span data-ttu-id="cd629-114">String collection</span><span class="sxs-lookup"><span data-stu-id="cd629-114">String collection</span></span>|<span data-ttu-id="cd629-115">收件人的 id 的集合。</span><span class="sxs-lookup"><span data-stu-id="cd629-115">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd629-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd629-116">JSON representation</span></span>

<span data-ttu-id="cd629-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd629-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


