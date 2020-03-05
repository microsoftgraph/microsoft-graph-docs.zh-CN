---
title: educationFormResource 资源类型
description: EducationResource 的子类。 此资源是窗体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ed81e1e9e74ad311e4102963649ff4a4015bb093
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501960"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="6dfe3-104">educationFormResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="6dfe3-104">educationFormResource resource type</span></span>

<span data-ttu-id="6dfe3-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6dfe3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dfe3-106">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="6dfe3-107">此资源是窗体。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-107">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="6dfe3-108">属性</span><span class="sxs-lookup"><span data-stu-id="6dfe3-108">Properties</span></span>
| <span data-ttu-id="6dfe3-109">属性</span><span class="sxs-lookup"><span data-stu-id="6dfe3-109">Property</span></span>     | <span data-ttu-id="6dfe3-110">类型</span><span class="sxs-lookup"><span data-stu-id="6dfe3-110">Type</span></span>   |<span data-ttu-id="6dfe3-111">说明</span><span class="sxs-lookup"><span data-stu-id="6dfe3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dfe3-112">originalFormId</span><span class="sxs-lookup"><span data-stu-id="6dfe3-112">originalFormId</span></span>|<span data-ttu-id="6dfe3-113">String</span><span class="sxs-lookup"><span data-stu-id="6dfe3-113">String</span></span>|<span data-ttu-id="6dfe3-114">表单的原始 id。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-114">Original id of the Form.</span></span>|
|<span data-ttu-id="6dfe3-115">formId</span><span class="sxs-lookup"><span data-stu-id="6dfe3-115">formId</span></span>|<span data-ttu-id="6dfe3-116">String</span><span class="sxs-lookup"><span data-stu-id="6dfe3-116">String</span></span>|<span data-ttu-id="6dfe3-117">表单的 Id。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-117">Id of the Form.</span></span>|
|<span data-ttu-id="6dfe3-118">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="6dfe3-118">isGroupForm</span></span>|<span data-ttu-id="6dfe3-119">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfe3-119">Boolean</span></span>|<span data-ttu-id="6dfe3-120">表单是否属于类组。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-120">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="6dfe3-121">viewUrl</span><span class="sxs-lookup"><span data-stu-id="6dfe3-121">viewUrl</span></span>|<span data-ttu-id="6dfe3-122">String</span><span class="sxs-lookup"><span data-stu-id="6dfe3-122">String</span></span>|<span data-ttu-id="6dfe3-123">表单的学生 URL。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-123">Student URL for the Form.</span></span>|
|<span data-ttu-id="6dfe3-124">viewUrl</span><span class="sxs-lookup"><span data-stu-id="6dfe3-124">viewUrl</span></span>|<span data-ttu-id="6dfe3-125">String</span><span class="sxs-lookup"><span data-stu-id="6dfe3-125">String</span></span>|<span data-ttu-id="6dfe3-126">表单的学生 URL。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-126">Student URL for the Form.</span></span>|
|<span data-ttu-id="6dfe3-127">editUrl</span><span class="sxs-lookup"><span data-stu-id="6dfe3-127">editUrl</span></span>|<span data-ttu-id="6dfe3-128">String</span><span class="sxs-lookup"><span data-stu-id="6dfe3-128">String</span></span>|<span data-ttu-id="6dfe3-129">表单的教师 URL。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-129">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6dfe3-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6dfe3-130">JSON representation</span></span>

<span data-ttu-id="6dfe3-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dfe3-131">The following is a JSON representation of the resource.</span></span>

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
