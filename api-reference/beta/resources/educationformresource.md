---
title: educationFormResource 资源类型
description: educationResource 的子类。 此资源是窗体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800969"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="abe48-104">educationFormResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="abe48-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe48-105">[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="abe48-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="abe48-106">此资源是窗体。</span><span class="sxs-lookup"><span data-stu-id="abe48-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="abe48-107">属性</span><span class="sxs-lookup"><span data-stu-id="abe48-107">Properties</span></span>
| <span data-ttu-id="abe48-108">属性</span><span class="sxs-lookup"><span data-stu-id="abe48-108">Property</span></span>     | <span data-ttu-id="abe48-109">类型</span><span class="sxs-lookup"><span data-stu-id="abe48-109">Type</span></span>   |<span data-ttu-id="abe48-110">说明</span><span class="sxs-lookup"><span data-stu-id="abe48-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abe48-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="abe48-111">originalFormId</span></span>|<span data-ttu-id="abe48-112">String</span><span class="sxs-lookup"><span data-stu-id="abe48-112">String</span></span>|<span data-ttu-id="abe48-113">表单的原始 id。</span><span class="sxs-lookup"><span data-stu-id="abe48-113">Original id of the Form.</span></span>|
|<span data-ttu-id="abe48-114">formId</span><span class="sxs-lookup"><span data-stu-id="abe48-114">formId</span></span>|<span data-ttu-id="abe48-115">String</span><span class="sxs-lookup"><span data-stu-id="abe48-115">String</span></span>|<span data-ttu-id="abe48-116">表单的 Id。</span><span class="sxs-lookup"><span data-stu-id="abe48-116">Id of the Form.</span></span>|
|<span data-ttu-id="abe48-117">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="abe48-117">isGroupForm</span></span>|<span data-ttu-id="abe48-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="abe48-118">Boolean</span></span>|<span data-ttu-id="abe48-119">表单是否属于类组。</span><span class="sxs-lookup"><span data-stu-id="abe48-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="abe48-120">viewUrl</span><span class="sxs-lookup"><span data-stu-id="abe48-120">viewUrl</span></span>|<span data-ttu-id="abe48-121">String</span><span class="sxs-lookup"><span data-stu-id="abe48-121">String</span></span>|<span data-ttu-id="abe48-122">表单的学生 URL。</span><span class="sxs-lookup"><span data-stu-id="abe48-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="abe48-123">viewUrl</span><span class="sxs-lookup"><span data-stu-id="abe48-123">viewUrl</span></span>|<span data-ttu-id="abe48-124">String</span><span class="sxs-lookup"><span data-stu-id="abe48-124">String</span></span>|<span data-ttu-id="abe48-125">表单的学生 URL。</span><span class="sxs-lookup"><span data-stu-id="abe48-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="abe48-126">editUrl</span><span class="sxs-lookup"><span data-stu-id="abe48-126">editUrl</span></span>|<span data-ttu-id="abe48-127">String</span><span class="sxs-lookup"><span data-stu-id="abe48-127">String</span></span>|<span data-ttu-id="abe48-128">表单的教师 URL。</span><span class="sxs-lookup"><span data-stu-id="abe48-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abe48-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abe48-129">JSON representation</span></span>

<span data-ttu-id="abe48-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abe48-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String"
  "formId": "String"
  "isGroupForm": "Boolean"
  "viewUrl": "String"
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationformresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
