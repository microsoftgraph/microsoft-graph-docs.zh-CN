---
title: personInterest 资源类型
description: personInterest 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0b635ab19f4cda9985de05e317316579ad60f7b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161395"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="297b3-103">personInterest 资源类型</span><span class="sxs-lookup"><span data-stu-id="297b3-103">personInterest resource type</span></span>

<span data-ttu-id="297b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="297b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="297b3-105">提供有关用户在各种服务中与自己相关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="297b3-105">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="297b3-106">继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="297b3-107">方法</span><span class="sxs-lookup"><span data-stu-id="297b3-107">Methods</span></span>

| <span data-ttu-id="297b3-108">方法</span><span class="sxs-lookup"><span data-stu-id="297b3-108">Method</span></span>                                                    | <span data-ttu-id="297b3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="297b3-109">Return Type</span></span>                         | <span data-ttu-id="297b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="297b3-110">Description</span></span>                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[<span data-ttu-id="297b3-111">列出兴趣</span><span class="sxs-lookup"><span data-stu-id="297b3-111">List interests</span></span>](../api/profile-list-interests.md)|<span data-ttu-id="297b3-112">[personInterest](../resources/personinterest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="297b3-112">[personInterest](../resources/personinterest.md) collection</span></span>|<span data-ttu-id="297b3-113">从 interests 导航属性获取 personInterest 资源。</span><span class="sxs-lookup"><span data-stu-id="297b3-113">Get the personInterest resources from the interests navigation property.</span></span>|
|[<span data-ttu-id="297b3-114">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-114">Create personInterest</span></span>](../api/profile-post-interests.md)|[<span data-ttu-id="297b3-115">personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-115">personInterest</span></span>](../resources/personinterest.md)|<span data-ttu-id="297b3-116">创建新的 personInterest 对象。</span><span class="sxs-lookup"><span data-stu-id="297b3-116">Create a new personInterest object.</span></span>|
|[<span data-ttu-id="297b3-117">获取 personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-117">Get personInterest</span></span>](../api/personinterest-get.md)|[<span data-ttu-id="297b3-118">personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-118">personInterest</span></span>](../resources/personinterest.md)|<span data-ttu-id="297b3-119">读取 [personInterest 对象的属性和](../resources/personinterest.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="297b3-119">Read the properties and relationships of a [personInterest](../resources/personinterest.md) object.</span></span>|
|[<span data-ttu-id="297b3-120">更新 personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-120">Update personInterest</span></span>](../api/personinterest-update.md)|[<span data-ttu-id="297b3-121">personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-121">personInterest</span></span>](../resources/personinterest.md)|<span data-ttu-id="297b3-122">更新 [personInterest 对象](../resources/personinterest.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="297b3-122">Update the properties of a [personInterest](../resources/personinterest.md) object.</span></span>|
|[<span data-ttu-id="297b3-123">删除 personInterest</span><span class="sxs-lookup"><span data-stu-id="297b3-123">Delete personInterest</span></span>](../api/personinterest-delete.md)|<span data-ttu-id="297b3-124">无</span><span class="sxs-lookup"><span data-stu-id="297b3-124">None</span></span>|<span data-ttu-id="297b3-125">删除 [personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="297b3-125">Deletes a [personInterest](../resources/personinterest.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="297b3-126">属性</span><span class="sxs-lookup"><span data-stu-id="297b3-126">Properties</span></span>

|<span data-ttu-id="297b3-127">属性</span><span class="sxs-lookup"><span data-stu-id="297b3-127">Property</span></span>|<span data-ttu-id="297b3-128">类型</span><span class="sxs-lookup"><span data-stu-id="297b3-128">Type</span></span>|<span data-ttu-id="297b3-129">说明</span><span class="sxs-lookup"><span data-stu-id="297b3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="297b3-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="297b3-130">allowedAudiences</span></span>|<span data-ttu-id="297b3-131">String</span><span class="sxs-lookup"><span data-stu-id="297b3-131">String</span></span>|<span data-ttu-id="297b3-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="297b3-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="297b3-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="297b3-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="297b3-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="297b3-135">categories</span><span class="sxs-lookup"><span data-stu-id="297b3-135">categories</span></span>|<span data-ttu-id="297b3-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="297b3-136">String collection</span></span>|<span data-ttu-id="297b3-137">包含用户与感兴趣的类别 (例如，个人、) 。</span><span class="sxs-lookup"><span data-stu-id="297b3-137">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="297b3-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="297b3-138">collaborationTags</span></span>|<span data-ttu-id="297b3-139">字符串集合</span><span class="sxs-lookup"><span data-stu-id="297b3-139">String collection</span></span>|<span data-ttu-id="297b3-140">包含用户与兴趣相关联的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="297b3-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="297b3-141">集合中允许的值是： `askMeAbout` ， `ableToMentor` ， `wantsToLearn` 。 `wantsToImprove`</span><span class="sxs-lookup"><span data-stu-id="297b3-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="297b3-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="297b3-142">createdBy</span></span>|[<span data-ttu-id="297b3-143">identitySet</span><span class="sxs-lookup"><span data-stu-id="297b3-143">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="297b3-144">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="297b3-144">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="297b3-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="297b3-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="297b3-146">createdDateTime</span></span>|<span data-ttu-id="297b3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297b3-147">DateTimeOffset</span></span>|<span data-ttu-id="297b3-148">提供实体创建时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="297b3-148">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="297b3-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="297b3-150">说明</span><span class="sxs-lookup"><span data-stu-id="297b3-150">description</span></span>|<span data-ttu-id="297b3-151">String</span><span class="sxs-lookup"><span data-stu-id="297b3-151">String</span></span>|<span data-ttu-id="297b3-152">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="297b3-152">Contains a description of the interest.</span></span>|
|<span data-ttu-id="297b3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="297b3-153">displayName</span></span>|<span data-ttu-id="297b3-154">String</span><span class="sxs-lookup"><span data-stu-id="297b3-154">String</span></span>|<span data-ttu-id="297b3-155">包含兴趣的友好名称。</span><span class="sxs-lookup"><span data-stu-id="297b3-155">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="297b3-156">id</span><span class="sxs-lookup"><span data-stu-id="297b3-156">id</span></span>|<span data-ttu-id="297b3-157">String</span><span class="sxs-lookup"><span data-stu-id="297b3-157">String</span></span>|<span data-ttu-id="297b3-158">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="297b3-158">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="297b3-159">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="297b3-159">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="297b3-160">inference</span><span class="sxs-lookup"><span data-stu-id="297b3-160">inference</span></span>|[<span data-ttu-id="297b3-161">inferenceData</span><span class="sxs-lookup"><span data-stu-id="297b3-161">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="297b3-162">包含通过创建或修改应用程序推断实体的推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="297b3-162">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="297b3-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="297b3-164">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="297b3-164">lastModifiedBy</span></span>|[<span data-ttu-id="297b3-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="297b3-165">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="297b3-166">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="297b3-166">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="297b3-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="297b3-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="297b3-168">lastModifiedDateTime</span></span>|<span data-ttu-id="297b3-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297b3-169">DateTimeOffset</span></span>|<span data-ttu-id="297b3-170">提供实体创建时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="297b3-170">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="297b3-171">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-171">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="297b3-172">source</span><span class="sxs-lookup"><span data-stu-id="297b3-172">source</span></span>|[<span data-ttu-id="297b3-173">personDataSource</span><span class="sxs-lookup"><span data-stu-id="297b3-173">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="297b3-174">如果从另一个服务同步，则值的来源。</span><span class="sxs-lookup"><span data-stu-id="297b3-174">Where the values originated if synced from another service.</span></span> <span data-ttu-id="297b3-175">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="297b3-175">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="297b3-176">WebUrl</span><span class="sxs-lookup"><span data-stu-id="297b3-176">webUrl</span></span>|<span data-ttu-id="297b3-177">String</span><span class="sxs-lookup"><span data-stu-id="297b3-177">String</span></span>|<span data-ttu-id="297b3-178">包含指向有关感兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="297b3-178">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="relationships"></a><span data-ttu-id="297b3-179">关系</span><span class="sxs-lookup"><span data-stu-id="297b3-179">Relationships</span></span>

<span data-ttu-id="297b3-180">无。</span><span class="sxs-lookup"><span data-stu-id="297b3-180">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="297b3-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="297b3-181">JSON representation</span></span>

<span data-ttu-id="297b3-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="297b3-182">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest"
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


