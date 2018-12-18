---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
ms.openlocfilehash: ca174381fe8722c5b96848ced1d0e09b469068f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351658"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="a24d3-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="a24d3-103">educationTeacher resource type</span></span>

> <span data-ttu-id="a24d3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a24d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a24d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a24d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a24d3-106">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="a24d3-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="a24d3-107">属性</span><span class="sxs-lookup"><span data-stu-id="a24d3-107">Properties</span></span>
| <span data-ttu-id="a24d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="a24d3-108">Property</span></span>     | <span data-ttu-id="a24d3-109">类型</span><span class="sxs-lookup"><span data-stu-id="a24d3-109">Type</span></span>   |<span data-ttu-id="a24d3-110">说明</span><span class="sxs-lookup"><span data-stu-id="a24d3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a24d3-111">externalId</span><span class="sxs-lookup"><span data-stu-id="a24d3-111">externalId</span></span>|<span data-ttu-id="a24d3-112">String</span><span class="sxs-lookup"><span data-stu-id="a24d3-112">String</span></span>| <span data-ttu-id="a24d3-113">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="a24d3-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="a24d3-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="a24d3-114">teacherNumber</span></span>|<span data-ttu-id="a24d3-115">String</span><span class="sxs-lookup"><span data-stu-id="a24d3-115">String</span></span>|<span data-ttu-id="a24d3-116">教师编号。</span><span class="sxs-lookup"><span data-stu-id="a24d3-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a24d3-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a24d3-117">JSON representation</span></span>

<span data-ttu-id="a24d3-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a24d3-118">The following is a JSON representation of the resource.</span></span>

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