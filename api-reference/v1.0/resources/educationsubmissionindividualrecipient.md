---
title: educationSubmissionIndividualRecipient 资源类型
description: 'educationSubmissionRecipient 的子类，指示提交已分配给班级中的个人。  '
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f9557f29edbd5e21db9de5b4c36ceb186b54ff34
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912238"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="cc0ea-103">educationSubmissionIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc0ea-103">educationSubmissionIndividualRecipient resource type</span></span>

<span data-ttu-id="cc0ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc0ea-105">[educationSubmissionRecipient](educationsubmissionrecipient.md)的子类，指示提交已分配给班级中的个人。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-105">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="cc0ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="cc0ea-106">Properties</span></span>
| <span data-ttu-id="cc0ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc0ea-107">Property</span></span>     | <span data-ttu-id="cc0ea-108">类型</span><span class="sxs-lookup"><span data-stu-id="cc0ea-108">Type</span></span>   |<span data-ttu-id="cc0ea-109">描述</span><span class="sxs-lookup"><span data-stu-id="cc0ea-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc0ea-110">userId</span><span class="sxs-lookup"><span data-stu-id="cc0ea-110">userId</span></span>|<span data-ttu-id="cc0ea-111">String</span><span class="sxs-lookup"><span data-stu-id="cc0ea-111">String</span></span>|<span data-ttu-id="cc0ea-112">为其分配提交的用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-112">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc0ea-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc0ea-113">JSON representation</span></span>

<span data-ttu-id="cc0ea-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-114">The following is a JSON representation of the resource.</span></span>

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


