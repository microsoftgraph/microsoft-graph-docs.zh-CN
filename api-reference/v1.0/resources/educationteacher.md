---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b58d74e6b53b1721a5139d050c7e89197b8721be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463654"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="4d178-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d178-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d178-104">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="4d178-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="4d178-105">属性</span><span class="sxs-lookup"><span data-stu-id="4d178-105">Properties</span></span>
| <span data-ttu-id="4d178-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d178-106">Property</span></span>     | <span data-ttu-id="4d178-107">类型</span><span class="sxs-lookup"><span data-stu-id="4d178-107">Type</span></span>   |<span data-ttu-id="4d178-108">说明</span><span class="sxs-lookup"><span data-stu-id="4d178-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d178-109">externalId</span><span class="sxs-lookup"><span data-stu-id="4d178-109">externalId</span></span>|<span data-ttu-id="4d178-110">字符串</span><span class="sxs-lookup"><span data-stu-id="4d178-110">String</span></span>| <span data-ttu-id="4d178-111">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="4d178-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="4d178-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="4d178-112">teacherNumber</span></span>|<span data-ttu-id="4d178-113">String</span><span class="sxs-lookup"><span data-stu-id="4d178-113">String</span></span>|<span data-ttu-id="4d178-114">教师编号。</span><span class="sxs-lookup"><span data-stu-id="4d178-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d178-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d178-115">JSON representation</span></span>

<span data-ttu-id="4d178-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d178-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationteacher.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
