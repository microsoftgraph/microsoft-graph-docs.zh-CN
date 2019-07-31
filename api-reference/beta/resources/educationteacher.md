---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2a94eb2c6a1d145c51fef8c35b3b2f9083cf598a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972321"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="1d5e0-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d5e0-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d5e0-104">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="1d5e0-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="1d5e0-105">属性</span><span class="sxs-lookup"><span data-stu-id="1d5e0-105">Properties</span></span>
| <span data-ttu-id="1d5e0-106">属性</span><span class="sxs-lookup"><span data-stu-id="1d5e0-106">Property</span></span>     | <span data-ttu-id="1d5e0-107">类型</span><span class="sxs-lookup"><span data-stu-id="1d5e0-107">Type</span></span>   |<span data-ttu-id="1d5e0-108">说明</span><span class="sxs-lookup"><span data-stu-id="1d5e0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d5e0-109">externalId</span><span class="sxs-lookup"><span data-stu-id="1d5e0-109">externalId</span></span>|<span data-ttu-id="1d5e0-110">String</span><span class="sxs-lookup"><span data-stu-id="1d5e0-110">String</span></span>| <span data-ttu-id="1d5e0-111">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d5e0-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="1d5e0-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="1d5e0-112">teacherNumber</span></span>|<span data-ttu-id="1d5e0-113">String</span><span class="sxs-lookup"><span data-stu-id="1d5e0-113">String</span></span>|<span data-ttu-id="1d5e0-114">教师编号。</span><span class="sxs-lookup"><span data-stu-id="1d5e0-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d5e0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d5e0-115">JSON representation</span></span>

<span data-ttu-id="1d5e0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d5e0-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
