---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 516322bd57dd29b8e9cd42c3662e173d4a4100fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032613"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="950b9-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="950b9-103">educationTeacher resource type</span></span>

<span data-ttu-id="950b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="950b9-105">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="950b9-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="950b9-106">属性</span><span class="sxs-lookup"><span data-stu-id="950b9-106">Properties</span></span>
| <span data-ttu-id="950b9-107">属性</span><span class="sxs-lookup"><span data-stu-id="950b9-107">Property</span></span>     | <span data-ttu-id="950b9-108">类型</span><span class="sxs-lookup"><span data-stu-id="950b9-108">Type</span></span>   |<span data-ttu-id="950b9-109">说明</span><span class="sxs-lookup"><span data-stu-id="950b9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950b9-110">externalId</span><span class="sxs-lookup"><span data-stu-id="950b9-110">externalId</span></span>|<span data-ttu-id="950b9-111">String</span><span class="sxs-lookup"><span data-stu-id="950b9-111">String</span></span>| <span data-ttu-id="950b9-112">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="950b9-112">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="950b9-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="950b9-113">teacherNumber</span></span>|<span data-ttu-id="950b9-114">String</span><span class="sxs-lookup"><span data-stu-id="950b9-114">String</span></span>|<span data-ttu-id="950b9-115">教师编号。</span><span class="sxs-lookup"><span data-stu-id="950b9-115">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="950b9-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="950b9-116">JSON representation</span></span>

<span data-ttu-id="950b9-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="950b9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

