---
title: educationSubmissionIndividualRecipient 资源类型
description: 'EducationSubmissionRecipient 的一个子类, 该子类指示向班级中的个人分配提交。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2eecdc7e7ddd30ecad9a520b42cd11df9565fa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972507"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="f9ff0-103">educationSubmissionIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9ff0-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ff0-104">[EducationSubmissionRecipient](educationsubmissionrecipient.md)的一个子类, 该子类指示向班级中的个人分配提交。</span><span class="sxs-lookup"><span data-stu-id="f9ff0-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="f9ff0-105">属性</span><span class="sxs-lookup"><span data-stu-id="f9ff0-105">Properties</span></span>
| <span data-ttu-id="f9ff0-106">属性</span><span class="sxs-lookup"><span data-stu-id="f9ff0-106">Property</span></span>     | <span data-ttu-id="f9ff0-107">类型</span><span class="sxs-lookup"><span data-stu-id="f9ff0-107">Type</span></span>   |<span data-ttu-id="f9ff0-108">说明</span><span class="sxs-lookup"><span data-stu-id="f9ff0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9ff0-109">userId</span><span class="sxs-lookup"><span data-stu-id="f9ff0-109">userId</span></span>|<span data-ttu-id="f9ff0-110">String</span><span class="sxs-lookup"><span data-stu-id="f9ff0-110">String</span></span>|<span data-ttu-id="f9ff0-111">向其分配提交的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="f9ff0-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9ff0-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9ff0-112">JSON representation</span></span>

<span data-ttu-id="f9ff0-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9ff0-113">The following is a JSON representation of the resource.</span></span>

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
