---
title: educationSubmissionIndividualRecipient 资源类型
description: 'EducationSubmissionRecipient 的一个子类，该子类指示向班级中的个人分配提交。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a18c6cc00ef72e7222296f65d1bdae6293d2211f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055645"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="3283c-103">educationSubmissionIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="3283c-103">educationSubmissionIndividualRecipient resource type</span></span>

<span data-ttu-id="3283c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3283c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3283c-105">[EducationSubmissionRecipient](educationsubmissionrecipient.md)的一个子类，该子类指示向班级中的个人分配提交。</span><span class="sxs-lookup"><span data-stu-id="3283c-105">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="3283c-106">属性</span><span class="sxs-lookup"><span data-stu-id="3283c-106">Properties</span></span>
| <span data-ttu-id="3283c-107">属性</span><span class="sxs-lookup"><span data-stu-id="3283c-107">Property</span></span>     | <span data-ttu-id="3283c-108">类型</span><span class="sxs-lookup"><span data-stu-id="3283c-108">Type</span></span>   |<span data-ttu-id="3283c-109">描述</span><span class="sxs-lookup"><span data-stu-id="3283c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3283c-110">userId</span><span class="sxs-lookup"><span data-stu-id="3283c-110">userId</span></span>|<span data-ttu-id="3283c-111">String</span><span class="sxs-lookup"><span data-stu-id="3283c-111">String</span></span>|<span data-ttu-id="3283c-112">向其分配提交的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3283c-112">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3283c-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3283c-113">JSON representation</span></span>

<span data-ttu-id="3283c-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3283c-114">The following is a JSON representation of the resource.</span></span>

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


