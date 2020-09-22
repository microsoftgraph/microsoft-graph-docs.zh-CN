---
title: educationFormResource 资源类型
description: EducationResource 的子类。 此资源是窗体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0c8748c725f7289eadbca8119b47bf8a81b28c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095437"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="a29f0-104">educationFormResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a29f0-104">educationFormResource resource type</span></span>

<span data-ttu-id="a29f0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a29f0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a29f0-106">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="a29f0-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="a29f0-107">此资源是窗体。</span><span class="sxs-lookup"><span data-stu-id="a29f0-107">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="a29f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="a29f0-108">Properties</span></span>
| <span data-ttu-id="a29f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="a29f0-109">Property</span></span>     | <span data-ttu-id="a29f0-110">类型</span><span class="sxs-lookup"><span data-stu-id="a29f0-110">Type</span></span>   |<span data-ttu-id="a29f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="a29f0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a29f0-112">originalFormId</span><span class="sxs-lookup"><span data-stu-id="a29f0-112">originalFormId</span></span>|<span data-ttu-id="a29f0-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a29f0-113">String</span></span>|<span data-ttu-id="a29f0-114">表单的原始 id。</span><span class="sxs-lookup"><span data-stu-id="a29f0-114">Original id of the Form.</span></span>|
|<span data-ttu-id="a29f0-115">formId</span><span class="sxs-lookup"><span data-stu-id="a29f0-115">formId</span></span>|<span data-ttu-id="a29f0-116">字符串</span><span class="sxs-lookup"><span data-stu-id="a29f0-116">String</span></span>|<span data-ttu-id="a29f0-117">表单的 Id。</span><span class="sxs-lookup"><span data-stu-id="a29f0-117">Id of the Form.</span></span>|
|<span data-ttu-id="a29f0-118">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="a29f0-118">isGroupForm</span></span>|<span data-ttu-id="a29f0-119">布尔</span><span class="sxs-lookup"><span data-stu-id="a29f0-119">Boolean</span></span>|<span data-ttu-id="a29f0-120">表单是否属于类组。</span><span class="sxs-lookup"><span data-stu-id="a29f0-120">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="a29f0-121">viewUrl</span><span class="sxs-lookup"><span data-stu-id="a29f0-121">viewUrl</span></span>|<span data-ttu-id="a29f0-122">字符串</span><span class="sxs-lookup"><span data-stu-id="a29f0-122">String</span></span>|<span data-ttu-id="a29f0-123">表单的学生 URL。</span><span class="sxs-lookup"><span data-stu-id="a29f0-123">Student URL for the Form.</span></span>|
|<span data-ttu-id="a29f0-124">viewUrl</span><span class="sxs-lookup"><span data-stu-id="a29f0-124">viewUrl</span></span>|<span data-ttu-id="a29f0-125">字符串</span><span class="sxs-lookup"><span data-stu-id="a29f0-125">String</span></span>|<span data-ttu-id="a29f0-126">表单的学生 URL。</span><span class="sxs-lookup"><span data-stu-id="a29f0-126">Student URL for the Form.</span></span>|
|<span data-ttu-id="a29f0-127">editUrl</span><span class="sxs-lookup"><span data-stu-id="a29f0-127">editUrl</span></span>|<span data-ttu-id="a29f0-128">字符串</span><span class="sxs-lookup"><span data-stu-id="a29f0-128">String</span></span>|<span data-ttu-id="a29f0-129">表单的教师 URL。</span><span class="sxs-lookup"><span data-stu-id="a29f0-129">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a29f0-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a29f0-130">JSON representation</span></span>

<span data-ttu-id="a29f0-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a29f0-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String",
  "formId": "String",
  "isGroupForm": "Boolean",
  "viewUrl": "String",
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
  "suppressions": []
}
-->


