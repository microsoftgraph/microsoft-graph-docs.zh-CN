---
title: educationAssignmentIndividualRecipient 资源类型
description: '在 assignTo 属性中使用。 当设置为 "单个收件人列表" 时，课程中的 "选定学生" 将 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5bccdf98bbba4c0965daf5d5aba93cf1a34b758
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502548"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="d30a5-104">educationAssignmentIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="d30a5-104">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="d30a5-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d30a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30a5-106">在[assignTo](educationassignment.md)属性中使用。</span><span class="sxs-lookup"><span data-stu-id="d30a5-106">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="d30a5-107">如果设置为 "单个收件人列表"，则在发布工作分配时，类中的所选学生将收到提交对象。</span><span class="sxs-lookup"><span data-stu-id="d30a5-107">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="d30a5-108">此资源是[educationAssignmentRecipient](educationassignmentrecipient.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="d30a5-108">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d30a5-109">属性</span><span class="sxs-lookup"><span data-stu-id="d30a5-109">Properties</span></span>
| <span data-ttu-id="d30a5-110">属性</span><span class="sxs-lookup"><span data-stu-id="d30a5-110">Property</span></span>     | <span data-ttu-id="d30a5-111">类型</span><span class="sxs-lookup"><span data-stu-id="d30a5-111">Type</span></span>   |<span data-ttu-id="d30a5-112">说明</span><span class="sxs-lookup"><span data-stu-id="d30a5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d30a5-113">recipients</span><span class="sxs-lookup"><span data-stu-id="d30a5-113">recipients</span></span>|<span data-ttu-id="d30a5-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="d30a5-114">String collection</span></span>|<span data-ttu-id="d30a5-115">收件人的 id 的集合。</span><span class="sxs-lookup"><span data-stu-id="d30a5-115">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d30a5-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d30a5-116">JSON representation</span></span>

<span data-ttu-id="d30a5-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d30a5-117">The following is a JSON representation of the resource.</span></span>

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
