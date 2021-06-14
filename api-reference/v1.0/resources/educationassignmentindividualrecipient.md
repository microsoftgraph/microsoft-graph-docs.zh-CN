---
title: educationAssignmentIndividualRecipient 资源类型
description: 在 assignment.assignTo 属性内使用。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 147697685f58723d940102333abd9ffc378bee28
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912313"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="9aac5-103">educationAssignmentIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="9aac5-103">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="9aac5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9aac5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9aac5-105">在 [assignment.assignTo 属性内](educationassignment.md) 使用。</span><span class="sxs-lookup"><span data-stu-id="9aac5-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="9aac5-106">设置为单个收件人列表时，课堂中选定的学生将在作业发布时收到提交对象。</span><span class="sxs-lookup"><span data-stu-id="9aac5-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="9aac5-107">此资源是 [educationAssignmentRecipient 的子类](educationassignmentrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="9aac5-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9aac5-108">属性</span><span class="sxs-lookup"><span data-stu-id="9aac5-108">Properties</span></span>
| <span data-ttu-id="9aac5-109">属性</span><span class="sxs-lookup"><span data-stu-id="9aac5-109">Property</span></span>     | <span data-ttu-id="9aac5-110">类型</span><span class="sxs-lookup"><span data-stu-id="9aac5-110">Type</span></span>   |<span data-ttu-id="9aac5-111">说明</span><span class="sxs-lookup"><span data-stu-id="9aac5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aac5-112">recipients</span><span class="sxs-lookup"><span data-stu-id="9aac5-112">recipients</span></span>|<span data-ttu-id="9aac5-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9aac5-113">String collection</span></span>|<span data-ttu-id="9aac5-114">收件人的 ID 集合。</span><span class="sxs-lookup"><span data-stu-id="9aac5-114">A collection of IDs of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9aac5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9aac5-115">JSON representation</span></span>

<span data-ttu-id="9aac5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aac5-116">The following is a JSON representation of the resource.</span></span>

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


