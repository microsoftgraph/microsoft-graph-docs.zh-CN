---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
ms.openlocfilehash: a880c3908b70e0b9d7c580492f45183b8f15425d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334459"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="60cc5-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="60cc5-103">educationTeacher resource type</span></span>

<span data-ttu-id="60cc5-104">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="60cc5-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="60cc5-105">属性</span><span class="sxs-lookup"><span data-stu-id="60cc5-105">Properties</span></span>
| <span data-ttu-id="60cc5-106">属性</span><span class="sxs-lookup"><span data-stu-id="60cc5-106">Property</span></span>     | <span data-ttu-id="60cc5-107">类型</span><span class="sxs-lookup"><span data-stu-id="60cc5-107">Type</span></span>   |<span data-ttu-id="60cc5-108">说明</span><span class="sxs-lookup"><span data-stu-id="60cc5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60cc5-109">externalId</span><span class="sxs-lookup"><span data-stu-id="60cc5-109">externalId</span></span>|<span data-ttu-id="60cc5-110">String</span><span class="sxs-lookup"><span data-stu-id="60cc5-110">String</span></span>| <span data-ttu-id="60cc5-111">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="60cc5-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="60cc5-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="60cc5-112">teacherNumber</span></span>|<span data-ttu-id="60cc5-113">String</span><span class="sxs-lookup"><span data-stu-id="60cc5-113">String</span></span>|<span data-ttu-id="60cc5-114">教师编号。</span><span class="sxs-lookup"><span data-stu-id="60cc5-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60cc5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60cc5-115">JSON representation</span></span>

<span data-ttu-id="60cc5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60cc5-116">The following is a JSON representation of the resource.</span></span>

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