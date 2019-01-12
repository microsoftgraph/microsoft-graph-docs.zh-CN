---
title: educationSubmissionIndividualRecipient 资源类型
description: 'EducationSubmissionRecipient 指示提交分配给单个类中的一个子类。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4b412b95577f3f111233f78aaa033bb12daab308
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912930"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="ffb5f-103">educationSubmissionIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffb5f-103">educationSubmissionIndividualRecipient resource type</span></span>

> <span data-ttu-id="ffb5f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ffb5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffb5f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ffb5f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ffb5f-106">[EducationSubmissionRecipient](educationsubmissionrecipient.md)指示提交分配给单个类中的一个子类。</span><span class="sxs-lookup"><span data-stu-id="ffb5f-106">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="ffb5f-107">属性</span><span class="sxs-lookup"><span data-stu-id="ffb5f-107">Properties</span></span>
| <span data-ttu-id="ffb5f-108">属性</span><span class="sxs-lookup"><span data-stu-id="ffb5f-108">Property</span></span>     | <span data-ttu-id="ffb5f-109">类型</span><span class="sxs-lookup"><span data-stu-id="ffb5f-109">Type</span></span>   |<span data-ttu-id="ffb5f-110">说明</span><span class="sxs-lookup"><span data-stu-id="ffb5f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffb5f-111">userId</span><span class="sxs-lookup"><span data-stu-id="ffb5f-111">userId</span></span>|<span data-ttu-id="ffb5f-112">String</span><span class="sxs-lookup"><span data-stu-id="ffb5f-112">String</span></span>|<span data-ttu-id="ffb5f-113">向其分配提交的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="ffb5f-113">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffb5f-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffb5f-114">JSON representation</span></span>

<span data-ttu-id="ffb5f-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffb5f-115">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
