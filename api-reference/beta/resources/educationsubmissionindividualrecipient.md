---
title: educationSubmissionIndividualRecipient 资源类型
description: 'educationSubmissionRecipient 的一个子类, 该子类指示向班级中的个人分配提交。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: de58dc743cd50f0e31021b4651bb0a3b3b192197
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340538"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="d1ac6-103">educationSubmissionIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1ac6-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1ac6-104">[educationSubmissionRecipient](educationsubmissionrecipient.md)的一个子类, 该子类指示向班级中的个人分配提交。</span><span class="sxs-lookup"><span data-stu-id="d1ac6-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="d1ac6-105">属性</span><span class="sxs-lookup"><span data-stu-id="d1ac6-105">Properties</span></span>
| <span data-ttu-id="d1ac6-106">属性</span><span class="sxs-lookup"><span data-stu-id="d1ac6-106">Property</span></span>     | <span data-ttu-id="d1ac6-107">类型</span><span class="sxs-lookup"><span data-stu-id="d1ac6-107">Type</span></span>   |<span data-ttu-id="d1ac6-108">说明</span><span class="sxs-lookup"><span data-stu-id="d1ac6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1ac6-109">userId</span><span class="sxs-lookup"><span data-stu-id="d1ac6-109">userId</span></span>|<span data-ttu-id="d1ac6-110">String</span><span class="sxs-lookup"><span data-stu-id="d1ac6-110">String</span></span>|<span data-ttu-id="d1ac6-111">向其分配提交的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d1ac6-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1ac6-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1ac6-112">JSON representation</span></span>

<span data-ttu-id="d1ac6-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1ac6-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
