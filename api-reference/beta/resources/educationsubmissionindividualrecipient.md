---
title: educationSubmissionIndividualRecipient 资源类型
description: 'educationSubmissionRecipient 的一个子类, 该子类指示向班级中的个人分配提交。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8660ec569362d8170d15de86073c0ef59c9ec0a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507053"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="c9b60-103">educationSubmissionIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9b60-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9b60-104">[educationSubmissionRecipient](educationsubmissionrecipient.md)的一个子类, 该子类指示向班级中的个人分配提交。</span><span class="sxs-lookup"><span data-stu-id="c9b60-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="c9b60-105">属性</span><span class="sxs-lookup"><span data-stu-id="c9b60-105">Properties</span></span>
| <span data-ttu-id="c9b60-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9b60-106">Property</span></span>     | <span data-ttu-id="c9b60-107">类型</span><span class="sxs-lookup"><span data-stu-id="c9b60-107">Type</span></span>   |<span data-ttu-id="c9b60-108">说明</span><span class="sxs-lookup"><span data-stu-id="c9b60-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9b60-109">userId</span><span class="sxs-lookup"><span data-stu-id="c9b60-109">userId</span></span>|<span data-ttu-id="c9b60-110">String</span><span class="sxs-lookup"><span data-stu-id="c9b60-110">String</span></span>|<span data-ttu-id="c9b60-111">向其分配提交的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="c9b60-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9b60-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9b60-112">JSON representation</span></span>

<span data-ttu-id="c9b60-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9b60-113">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
