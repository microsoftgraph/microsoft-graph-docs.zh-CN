---
title: projectParticipation 资源类型
description: projectParticipation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2e292795eeccc25029063763c0e1a2c4883009d7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227678"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="001f8-103">projectParticipation 资源类型</span><span class="sxs-lookup"><span data-stu-id="001f8-103">projectParticipation resource type</span></span>

<span data-ttu-id="001f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="001f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="001f8-105">表示有关与用户关联的项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="001f8-105">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="001f8-106">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="001f8-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="001f8-107">方法</span><span class="sxs-lookup"><span data-stu-id="001f8-107">Methods</span></span>

| <span data-ttu-id="001f8-108">方法</span><span class="sxs-lookup"><span data-stu-id="001f8-108">Method</span></span>                                                                | <span data-ttu-id="001f8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="001f8-109">Return Type</span></span>                                     | <span data-ttu-id="001f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="001f8-110">Description</span></span>                                                                 |
|:----------------------------------------------------------------------|:------------------------------------------------|:----------------------------------------------------------------------------|
| [<span data-ttu-id="001f8-111">获取 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="001f8-111">Get projectParticipation</span></span>](../api/projectparticipation-get.md)        | [<span data-ttu-id="001f8-112">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="001f8-112">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="001f8-113">读取**projectParticipation**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="001f8-113">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="001f8-114">更新 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="001f8-114">Update projectParticipation</span></span>](../api/projectparticipation-update.md)  | [<span data-ttu-id="001f8-115">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="001f8-115">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="001f8-116">更新**projectParticipation**对象。</span><span class="sxs-lookup"><span data-stu-id="001f8-116">Update a **projectParticipation** object.</span></span>                                   |
| [<span data-ttu-id="001f8-117">删除 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="001f8-117">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)  | <span data-ttu-id="001f8-118">无。</span><span class="sxs-lookup"><span data-stu-id="001f8-118">None.</span></span>                                           | <span data-ttu-id="001f8-119">删除**projectParticipation**对象。</span><span class="sxs-lookup"><span data-stu-id="001f8-119">Delete a **projectParticipation** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="001f8-120">属性</span><span class="sxs-lookup"><span data-stu-id="001f8-120">Properties</span></span>

| <span data-ttu-id="001f8-121">属性</span><span class="sxs-lookup"><span data-stu-id="001f8-121">Property</span></span>     | <span data-ttu-id="001f8-122">类型</span><span class="sxs-lookup"><span data-stu-id="001f8-122">Type</span></span>                                        | <span data-ttu-id="001f8-123">说明</span><span class="sxs-lookup"><span data-stu-id="001f8-123">Description</span></span>                                                                                                |
|:-------------|:--------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="001f8-124">categories</span><span class="sxs-lookup"><span data-stu-id="001f8-124">categories</span></span>    | <span data-ttu-id="001f8-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="001f8-125">String collection</span></span>                           | <span data-ttu-id="001f8-126">包含用户与项目相关联的类别（例如，数字转换、石油远程测试机组）。</span><span class="sxs-lookup"><span data-stu-id="001f8-126">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="001f8-127">客户端</span><span class="sxs-lookup"><span data-stu-id="001f8-127">client</span></span>        |[<span data-ttu-id="001f8-128">companyDetail</span><span class="sxs-lookup"><span data-stu-id="001f8-128">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="001f8-129">包含有关项目所针对的客户端的详细信息。</span><span class="sxs-lookup"><span data-stu-id="001f8-129">Contains detailed information about the client the project was for.</span></span>                                        |
|<span data-ttu-id="001f8-130">征求</span><span class="sxs-lookup"><span data-stu-id="001f8-130">colleagues</span></span>    |<span data-ttu-id="001f8-131">[relatedPerson](relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="001f8-131">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="001f8-132">列出也在项目中工作的人员。</span><span class="sxs-lookup"><span data-stu-id="001f8-132">Lists people that also worked on the project.</span></span>                                                              |
|<span data-ttu-id="001f8-133">介绍</span><span class="sxs-lookup"><span data-stu-id="001f8-133">detail</span></span>        |[<span data-ttu-id="001f8-134">positionDetail</span><span class="sxs-lookup"><span data-stu-id="001f8-134">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="001f8-135">包含有关用户在项目上的角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="001f8-135">Contains detail about the user's role on the project.</span></span>                                                      |
|<span data-ttu-id="001f8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="001f8-136">displayName</span></span>   |<span data-ttu-id="001f8-137">String</span><span class="sxs-lookup"><span data-stu-id="001f8-137">String</span></span>                                       |<span data-ttu-id="001f8-138">包含项目的友好名称。</span><span class="sxs-lookup"><span data-stu-id="001f8-138">Contains a friendly name for the project.</span></span>                                                                   |
|<span data-ttu-id="001f8-139">人</span><span class="sxs-lookup"><span data-stu-id="001f8-139">sponsors</span></span>      |<span data-ttu-id="001f8-140">[relatedPerson](relatedperson.md)集合</span><span class="sxs-lookup"><span data-stu-id="001f8-140">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="001f8-141">发起项目的人员或人员。</span><span class="sxs-lookup"><span data-stu-id="001f8-141">The Person or people who sponsored the project.</span></span>                                                            |

## <a name="relationships"></a><span data-ttu-id="001f8-142">关系</span><span class="sxs-lookup"><span data-stu-id="001f8-142">Relationships</span></span>

<span data-ttu-id="001f8-143">无。</span><span class="sxs-lookup"><span data-stu-id="001f8-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="001f8-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="001f8-144">JSON representation</span></span>

<span data-ttu-id="001f8-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="001f8-145">The following is a JSON representation of the resource.</span></span>

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
