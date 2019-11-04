---
title: projectParticipation 资源类型
description: projectParticipation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 465a45a2ba8a607d0537e66b96207b3d60626517
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950470"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="4b7c5-103">projectParticipation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b7c5-103">projectParticipation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b7c5-104">表示有关与用户关联的项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-104">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="4b7c5-105">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4b7c5-106">方法</span><span class="sxs-lookup"><span data-stu-id="4b7c5-106">Methods</span></span>

| <span data-ttu-id="4b7c5-107">方法</span><span class="sxs-lookup"><span data-stu-id="4b7c5-107">Method</span></span>                                                         | <span data-ttu-id="4b7c5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b7c5-108">Return Type</span></span>                                     | <span data-ttu-id="4b7c5-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b7c5-109">Description</span></span>                                                       |
|:---------------------------------------------------------------|:------------------------------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="4b7c5-110">获取 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4b7c5-110">Get projectParticipation</span></span>](../api/projectparticipation-get.md) | [<span data-ttu-id="4b7c5-111">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4b7c5-111">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="4b7c5-112">读取**projectParticipation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-112">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="4b7c5-113">更新 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4b7c5-113">Update projectParticipation</span></span>](../api/projectparticipation-update.md)                | [<span data-ttu-id="4b7c5-114">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4b7c5-114">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="4b7c5-115">更新**projectParticipation**对象。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-115">Update a **projectParticipation** object.</span></span>                               |
| [<span data-ttu-id="4b7c5-116">删除 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4b7c5-116">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)                | <span data-ttu-id="4b7c5-117">无。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-117">None.</span></span>                                            | <span data-ttu-id="4b7c5-118">删除**projectParticipation**对象。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-118">Delete a **projectParticipation** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="4b7c5-119">属性</span><span class="sxs-lookup"><span data-stu-id="4b7c5-119">Properties</span></span>

| <span data-ttu-id="4b7c5-120">属性</span><span class="sxs-lookup"><span data-stu-id="4b7c5-120">Property</span></span>     | <span data-ttu-id="4b7c5-121">类型</span><span class="sxs-lookup"><span data-stu-id="4b7c5-121">Type</span></span>                                        | <span data-ttu-id="4b7c5-122">描述</span><span class="sxs-lookup"><span data-stu-id="4b7c5-122">Description</span></span>                                                                                      |
|:-------------|:--------------------------------------------|:-------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4b7c5-123">类别</span><span class="sxs-lookup"><span data-stu-id="4b7c5-123">categories</span></span>    | <span data-ttu-id="4b7c5-124">String collection</span><span class="sxs-lookup"><span data-stu-id="4b7c5-124">String collection</span></span>                           | <span data-ttu-id="4b7c5-125">包含用户与项目相关联的类别（例如，数字转换、石油远程测试机组）。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-125">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="4b7c5-126">客户端</span><span class="sxs-lookup"><span data-stu-id="4b7c5-126">client</span></span>        |[<span data-ttu-id="4b7c5-127">companyDetail</span><span class="sxs-lookup"><span data-stu-id="4b7c5-127">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="4b7c5-128">包含有关项目所针对的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-128">Contains detailed information about the client the project was for.</span></span>                              |
|<span data-ttu-id="4b7c5-129">征求</span><span class="sxs-lookup"><span data-stu-id="4b7c5-129">colleagues</span></span>    |<span data-ttu-id="4b7c5-130">[relatedPerson](relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b7c5-130">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="4b7c5-131">列出也在项目中工作的人员。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-131">Lists people that also worked on the project.</span></span>                                                          |
|<span data-ttu-id="4b7c5-132">介绍</span><span class="sxs-lookup"><span data-stu-id="4b7c5-132">detail</span></span>        |[<span data-ttu-id="4b7c5-133">positionDetail</span><span class="sxs-lookup"><span data-stu-id="4b7c5-133">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="4b7c5-134">包含有关用户在项目上的角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-134">Contains detail about the user's role on the project.</span></span>                                             |
|<span data-ttu-id="4b7c5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4b7c5-135">displayName</span></span>   |<span data-ttu-id="4b7c5-136">String</span><span class="sxs-lookup"><span data-stu-id="4b7c5-136">String</span></span>                                       |<span data-ttu-id="4b7c5-137">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-137">Contains a friendly name for the project.</span></span>                                                         |
|<span data-ttu-id="4b7c5-138">人</span><span class="sxs-lookup"><span data-stu-id="4b7c5-138">sponsors</span></span>      |<span data-ttu-id="4b7c5-139">[relatedPerson](relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b7c5-139">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="4b7c5-140">发起项目的人员或人员。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-140">The Person or people who sponsored the project.</span></span>                                                         |

## <a name="relationships"></a><span data-ttu-id="4b7c5-141">关系</span><span class="sxs-lookup"><span data-stu-id="4b7c5-141">Relationships</span></span>

<span data-ttu-id="4b7c5-142">无。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b7c5-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b7c5-143">JSON representation</span></span>

<span data-ttu-id="4b7c5-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b7c5-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "client": {"@odata.type": "microsoft.graph.companyDetail"},
  "colleagues": [{"@odata.type": "microsoft.graph.relatedPerson"}],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"},
  "displayName": "String",
  "sponsors": [{"@odata.type": "microsoft.graph.relatedPerson"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "projectParticipation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
