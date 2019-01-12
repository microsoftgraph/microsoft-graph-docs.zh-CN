---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2c485ec7816f20951df5f2a91cb8dd7577614cad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967579"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="16bbb-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="16bbb-103">educationTeacher resource type</span></span>

> <span data-ttu-id="16bbb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="16bbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16bbb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16bbb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16bbb-106">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="16bbb-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="16bbb-107">属性</span><span class="sxs-lookup"><span data-stu-id="16bbb-107">Properties</span></span>
| <span data-ttu-id="16bbb-108">属性</span><span class="sxs-lookup"><span data-stu-id="16bbb-108">Property</span></span>     | <span data-ttu-id="16bbb-109">类型</span><span class="sxs-lookup"><span data-stu-id="16bbb-109">Type</span></span>   |<span data-ttu-id="16bbb-110">说明</span><span class="sxs-lookup"><span data-stu-id="16bbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16bbb-111">externalId</span><span class="sxs-lookup"><span data-stu-id="16bbb-111">externalId</span></span>|<span data-ttu-id="16bbb-112">String</span><span class="sxs-lookup"><span data-stu-id="16bbb-112">String</span></span>| <span data-ttu-id="16bbb-113">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="16bbb-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="16bbb-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="16bbb-114">teacherNumber</span></span>|<span data-ttu-id="16bbb-115">String</span><span class="sxs-lookup"><span data-stu-id="16bbb-115">String</span></span>|<span data-ttu-id="16bbb-116">教师编号。</span><span class="sxs-lookup"><span data-stu-id="16bbb-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16bbb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16bbb-117">JSON representation</span></span>

<span data-ttu-id="16bbb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16bbb-118">The following is a JSON representation of the resource.</span></span>

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
