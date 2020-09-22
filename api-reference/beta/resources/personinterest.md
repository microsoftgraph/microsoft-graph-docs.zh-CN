---
title: personInterest 资源类型
description: personInterest 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7071f089c7dbc9ff309dfc1d45628ef24c367567
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997958"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="21424-103">personInterest 资源类型</span><span class="sxs-lookup"><span data-stu-id="21424-103">personInterest resource type</span></span>

<span data-ttu-id="21424-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21424-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21424-105">提供有关用户在各种服务中与其自身关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="21424-105">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="21424-106">继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="21424-107">方法</span><span class="sxs-lookup"><span data-stu-id="21424-107">Methods</span></span>

| <span data-ttu-id="21424-108">方法</span><span class="sxs-lookup"><span data-stu-id="21424-108">Method</span></span>                                                    | <span data-ttu-id="21424-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="21424-109">Return Type</span></span>                         | <span data-ttu-id="21424-110">说明</span><span class="sxs-lookup"><span data-stu-id="21424-110">Description</span></span>                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[<span data-ttu-id="21424-111">列出兴趣</span><span class="sxs-lookup"><span data-stu-id="21424-111">List interests</span></span>](../api/profile-list-interests.md)|<span data-ttu-id="21424-112">[personInterest](../resources/personinterest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21424-112">[personInterest](../resources/personinterest.md) collection</span></span>|<span data-ttu-id="21424-113">从 "兴趣" 导航属性中获取 personInterest 资源。</span><span class="sxs-lookup"><span data-stu-id="21424-113">Get the personInterest resources from the interests navigation property.</span></span>|
|[<span data-ttu-id="21424-114">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-114">Create personInterest</span></span>](../api/profile-post-interests.md)|[<span data-ttu-id="21424-115">personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-115">personInterest</span></span>](../resources/personinterest.md)|<span data-ttu-id="21424-116">创建新的 personInterest 对象。</span><span class="sxs-lookup"><span data-stu-id="21424-116">Create a new personInterest object.</span></span>|
|[<span data-ttu-id="21424-117">获取 personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-117">Get personInterest</span></span>](../api/personinterest-get.md)|[<span data-ttu-id="21424-118">personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-118">personInterest</span></span>](../resources/personinterest.md)|<span data-ttu-id="21424-119">读取 [personInterest](../resources/personinterest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21424-119">Read the properties and relationships of a [personInterest](../resources/personinterest.md) object.</span></span>|
|[<span data-ttu-id="21424-120">更新 personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-120">Update personInterest</span></span>](../api/personinterest-update.md)|[<span data-ttu-id="21424-121">personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-121">personInterest</span></span>](../resources/personinterest.md)|<span data-ttu-id="21424-122">更新 [personInterest](../resources/personinterest.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="21424-122">Update the properties of a [personInterest](../resources/personinterest.md) object.</span></span>|
|[<span data-ttu-id="21424-123">删除 personInterest</span><span class="sxs-lookup"><span data-stu-id="21424-123">Delete personInterest</span></span>](../api/personinterest-delete.md)|<span data-ttu-id="21424-124">无</span><span class="sxs-lookup"><span data-stu-id="21424-124">None</span></span>|<span data-ttu-id="21424-125">删除一个 [personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21424-125">Deletes a [personInterest](../resources/personinterest.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21424-126">属性</span><span class="sxs-lookup"><span data-stu-id="21424-126">Properties</span></span>

|<span data-ttu-id="21424-127">属性</span><span class="sxs-lookup"><span data-stu-id="21424-127">Property</span></span>|<span data-ttu-id="21424-128">类型</span><span class="sxs-lookup"><span data-stu-id="21424-128">Type</span></span>|<span data-ttu-id="21424-129">说明</span><span class="sxs-lookup"><span data-stu-id="21424-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21424-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="21424-130">allowedAudiences</span></span>|<span data-ttu-id="21424-131">String</span><span class="sxs-lookup"><span data-stu-id="21424-131">String</span></span>|<span data-ttu-id="21424-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="21424-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="21424-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="21424-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="21424-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21424-135">类别</span><span class="sxs-lookup"><span data-stu-id="21424-135">categories</span></span>|<span data-ttu-id="21424-136">String collection</span><span class="sxs-lookup"><span data-stu-id="21424-136">String collection</span></span>|<span data-ttu-id="21424-137">包含用户与兴趣相关联的类别 (例如，个人 recipies) 。</span><span class="sxs-lookup"><span data-stu-id="21424-137">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="21424-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="21424-138">collaborationTags</span></span>|<span data-ttu-id="21424-139">String collection</span><span class="sxs-lookup"><span data-stu-id="21424-139">String collection</span></span>|<span data-ttu-id="21424-140">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="21424-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="21424-141">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="21424-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="21424-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="21424-142">createdBy</span></span>|[<span data-ttu-id="21424-143">identitySet</span><span class="sxs-lookup"><span data-stu-id="21424-143">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="21424-144">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="21424-144">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="21424-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21424-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21424-146">createdDateTime</span></span>|<span data-ttu-id="21424-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21424-147">DateTimeOffset</span></span>|<span data-ttu-id="21424-148">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="21424-148">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="21424-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21424-150">description</span><span class="sxs-lookup"><span data-stu-id="21424-150">description</span></span>|<span data-ttu-id="21424-151">String</span><span class="sxs-lookup"><span data-stu-id="21424-151">String</span></span>|<span data-ttu-id="21424-152">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="21424-152">Contains a description of the interest.</span></span>|
|<span data-ttu-id="21424-153">displayName</span><span class="sxs-lookup"><span data-stu-id="21424-153">displayName</span></span>|<span data-ttu-id="21424-154">String</span><span class="sxs-lookup"><span data-stu-id="21424-154">String</span></span>|<span data-ttu-id="21424-155">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="21424-155">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="21424-156">id</span><span class="sxs-lookup"><span data-stu-id="21424-156">id</span></span>|<span data-ttu-id="21424-157">String</span><span class="sxs-lookup"><span data-stu-id="21424-157">String</span></span>|<span data-ttu-id="21424-158">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="21424-158">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="21424-159">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="21424-159">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="21424-160">推导</span><span class="sxs-lookup"><span data-stu-id="21424-160">inference</span></span>|[<span data-ttu-id="21424-161">inferenceData</span><span class="sxs-lookup"><span data-stu-id="21424-161">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="21424-162">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="21424-162">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="21424-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21424-164">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="21424-164">lastModifiedBy</span></span>|[<span data-ttu-id="21424-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="21424-165">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="21424-166">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="21424-166">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="21424-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21424-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21424-168">lastModifiedDateTime</span></span>|<span data-ttu-id="21424-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21424-169">DateTimeOffset</span></span>|<span data-ttu-id="21424-170">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="21424-170">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="21424-171">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-171">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21424-172">source</span><span class="sxs-lookup"><span data-stu-id="21424-172">source</span></span>|[<span data-ttu-id="21424-173">personDataSource</span><span class="sxs-lookup"><span data-stu-id="21424-173">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="21424-174">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="21424-174">Where the values originated if synced from another service.</span></span> <span data-ttu-id="21424-175">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="21424-175">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="21424-176">webUrl</span><span class="sxs-lookup"><span data-stu-id="21424-176">webUrl</span></span>|<span data-ttu-id="21424-177">String</span><span class="sxs-lookup"><span data-stu-id="21424-177">String</span></span>|<span data-ttu-id="21424-178">包含指向有关该兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="21424-178">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="relationships"></a><span data-ttu-id="21424-179">关系</span><span class="sxs-lookup"><span data-stu-id="21424-179">Relationships</span></span>

<span data-ttu-id="21424-180">无。</span><span class="sxs-lookup"><span data-stu-id="21424-180">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21424-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21424-181">JSON representation</span></span>

<span data-ttu-id="21424-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21424-182">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
  "baseType": ""
}-->

```json
{
  "@odata.type": "#microsoft.graph.personInterest",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "categories": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```


