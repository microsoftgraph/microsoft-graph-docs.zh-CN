---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 612e319699bac9bbb5776f7692d6d6f3b7da3867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849523"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="0ca76-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ca76-103">educationTeacher resource type</span></span>

<span data-ttu-id="0ca76-104">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="0ca76-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="0ca76-105">属性</span><span class="sxs-lookup"><span data-stu-id="0ca76-105">Properties</span></span>
| <span data-ttu-id="0ca76-106">属性</span><span class="sxs-lookup"><span data-stu-id="0ca76-106">Property</span></span>     | <span data-ttu-id="0ca76-107">类型</span><span class="sxs-lookup"><span data-stu-id="0ca76-107">Type</span></span>   |<span data-ttu-id="0ca76-108">说明</span><span class="sxs-lookup"><span data-stu-id="0ca76-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ca76-109">externalId</span><span class="sxs-lookup"><span data-stu-id="0ca76-109">externalId</span></span>|<span data-ttu-id="0ca76-110">String</span><span class="sxs-lookup"><span data-stu-id="0ca76-110">String</span></span>| <span data-ttu-id="0ca76-111">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="0ca76-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="0ca76-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="0ca76-112">teacherNumber</span></span>|<span data-ttu-id="0ca76-113">String</span><span class="sxs-lookup"><span data-stu-id="0ca76-113">String</span></span>|<span data-ttu-id="0ca76-114">教师编号。</span><span class="sxs-lookup"><span data-stu-id="0ca76-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ca76-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ca76-115">JSON representation</span></span>

<span data-ttu-id="0ca76-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ca76-116">The following is a JSON representation of the resource.</span></span>

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
