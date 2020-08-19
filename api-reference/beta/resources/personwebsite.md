---
title: personWebsite 资源类型
description: personWebsite 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e3f41b352af77073d6338888c8349e38145daff9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811082"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="d2060-103">personWebsite 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2060-103">personWebsite resource type</span></span>

<span data-ttu-id="d2060-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2060-105">表示有关与各种服务中的用户相关联的网站的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2060-105">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="d2060-106">继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d2060-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2060-107">Methods</span></span>
|<span data-ttu-id="d2060-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2060-108">Method</span></span>|<span data-ttu-id="d2060-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2060-109">Return type</span></span>|<span data-ttu-id="d2060-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2060-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2060-111">列出网站</span><span class="sxs-lookup"><span data-stu-id="d2060-111">List websites</span></span>](../api/profile-list-websites.md)|<span data-ttu-id="d2060-112">[personWebsite](../resources/personwebsite.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2060-112">[personWebsite](../resources/personwebsite.md) collection</span></span>|<span data-ttu-id="d2060-113">从 "网站" 导航属性中获取 personWebsite 资源。</span><span class="sxs-lookup"><span data-stu-id="d2060-113">Get the personWebsite resources from the websites navigation property.</span></span>|
|[<span data-ttu-id="d2060-114">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-114">Create personWebsite</span></span>](../api/profile-post-websites.md)|[<span data-ttu-id="d2060-115">personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-115">personWebsite</span></span>](../resources/personwebsite.md)|<span data-ttu-id="d2060-116">创建新的 personWebsite 对象。</span><span class="sxs-lookup"><span data-stu-id="d2060-116">Create a new personWebsite object.</span></span>|
|[<span data-ttu-id="d2060-117">获取 personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-117">Get personWebsite</span></span>](../api/personwebsite-get.md)|[<span data-ttu-id="d2060-118">personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-118">personWebsite</span></span>](../resources/personwebsite.md)|<span data-ttu-id="d2060-119">读取 [personWebsite](../resources/personwebsite.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2060-119">Read the properties and relationships of a [personWebsite](../resources/personwebsite.md) object.</span></span>|
|[<span data-ttu-id="d2060-120">更新 personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-120">Update personWebsite</span></span>](../api/personwebsite-update.md)|[<span data-ttu-id="d2060-121">personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-121">personWebsite</span></span>](../resources/personwebsite.md)|<span data-ttu-id="d2060-122">更新 [personWebsite](../resources/personwebsite.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2060-122">Update the properties of a [personWebsite](../resources/personwebsite.md) object.</span></span>|
|[<span data-ttu-id="d2060-123">删除 personWebsite</span><span class="sxs-lookup"><span data-stu-id="d2060-123">Delete personWebsite</span></span>](../api/personwebsite-delete.md)|<span data-ttu-id="d2060-124">无</span><span class="sxs-lookup"><span data-stu-id="d2060-124">None</span></span>|<span data-ttu-id="d2060-125">删除一个 [personWebsite](../resources/personwebsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2060-125">Deletes a [personWebsite](../resources/personwebsite.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2060-126">属性</span><span class="sxs-lookup"><span data-stu-id="d2060-126">Properties</span></span>

| <span data-ttu-id="d2060-127">属性</span><span class="sxs-lookup"><span data-stu-id="d2060-127">Property</span></span>     | <span data-ttu-id="d2060-128">类型</span><span class="sxs-lookup"><span data-stu-id="d2060-128">Type</span></span>              | <span data-ttu-id="d2060-129">说明</span><span class="sxs-lookup"><span data-stu-id="d2060-129">Description</span></span>                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|<span data-ttu-id="d2060-130">categories</span><span class="sxs-lookup"><span data-stu-id="d2060-130">categories</span></span>    |<span data-ttu-id="d2060-131">String collection</span><span class="sxs-lookup"><span data-stu-id="d2060-131">String collection</span></span>  | <span data-ttu-id="d2060-132">包含用户与网站相关联的类别 (例如，个人、食谱) 。</span><span class="sxs-lookup"><span data-stu-id="d2060-132">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="d2060-133">description</span><span class="sxs-lookup"><span data-stu-id="d2060-133">description</span></span>   |<span data-ttu-id="d2060-134">String</span><span class="sxs-lookup"><span data-stu-id="d2060-134">String</span></span>             | <span data-ttu-id="d2060-135">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="d2060-135">Contains a description of the website.</span></span>                                                        |
|<span data-ttu-id="d2060-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d2060-136">displayName</span></span>   |<span data-ttu-id="d2060-137">String</span><span class="sxs-lookup"><span data-stu-id="d2060-137">String</span></span>             | <span data-ttu-id="d2060-138">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d2060-138">Contains a friendly name for the website.</span></span>                                                     |
|<span data-ttu-id="d2060-139">webUrl</span><span class="sxs-lookup"><span data-stu-id="d2060-139">webUrl</span></span>        |<span data-ttu-id="d2060-140">String</span><span class="sxs-lookup"><span data-stu-id="d2060-140">String</span></span>             | <span data-ttu-id="d2060-141">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="d2060-141">Contains a link to the website itself.</span></span>                                                        |

## <a name="properties"></a><span data-ttu-id="d2060-142">属性</span><span class="sxs-lookup"><span data-stu-id="d2060-142">Properties</span></span>
|<span data-ttu-id="d2060-143">属性</span><span class="sxs-lookup"><span data-stu-id="d2060-143">Property</span></span>|<span data-ttu-id="d2060-144">类型</span><span class="sxs-lookup"><span data-stu-id="d2060-144">Type</span></span>|<span data-ttu-id="d2060-145">说明</span><span class="sxs-lookup"><span data-stu-id="d2060-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2060-146">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d2060-146">allowedAudiences</span></span>|<span data-ttu-id="d2060-147">String</span><span class="sxs-lookup"><span data-stu-id="d2060-147">String</span></span>|<span data-ttu-id="d2060-148">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="d2060-148">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d2060-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d2060-150">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d2060-150">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d2060-151">categories</span><span class="sxs-lookup"><span data-stu-id="d2060-151">categories</span></span>|<span data-ttu-id="d2060-152">String collection</span><span class="sxs-lookup"><span data-stu-id="d2060-152">String collection</span></span>|<span data-ttu-id="d2060-153">包含用户与网站相关联的类别 (例如，个人、食谱) 。</span><span class="sxs-lookup"><span data-stu-id="d2060-153">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="d2060-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="d2060-154">createdBy</span></span>|[<span data-ttu-id="d2060-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="d2060-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="d2060-156">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="d2060-156">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="d2060-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2060-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2060-158">createdDateTime</span></span>|<span data-ttu-id="d2060-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2060-159">DateTimeOffset</span></span>|<span data-ttu-id="d2060-160">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="d2060-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="d2060-161">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2060-162">description</span><span class="sxs-lookup"><span data-stu-id="d2060-162">description</span></span>|<span data-ttu-id="d2060-163">String</span><span class="sxs-lookup"><span data-stu-id="d2060-163">String</span></span>|<span data-ttu-id="d2060-164">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="d2060-164">Contains a description of the website.</span></span>|
|<span data-ttu-id="d2060-165">displayName</span><span class="sxs-lookup"><span data-stu-id="d2060-165">displayName</span></span>|<span data-ttu-id="d2060-166">String</span><span class="sxs-lookup"><span data-stu-id="d2060-166">String</span></span>|<span data-ttu-id="d2060-167">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d2060-167">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="d2060-168">id</span><span class="sxs-lookup"><span data-stu-id="d2060-168">id</span></span>|<span data-ttu-id="d2060-169">String</span><span class="sxs-lookup"><span data-stu-id="d2060-169">String</span></span>|<span data-ttu-id="d2060-170">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="d2060-170">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="d2060-171">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="d2060-171">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="d2060-172">推导</span><span class="sxs-lookup"><span data-stu-id="d2060-172">inference</span></span>|[<span data-ttu-id="d2060-173">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d2060-173">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d2060-174">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2060-174">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d2060-175">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-175">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2060-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d2060-176">lastModifiedBy</span></span>|[<span data-ttu-id="d2060-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="d2060-177">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="d2060-178">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="d2060-178">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="d2060-179">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-179">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2060-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2060-180">lastModifiedDateTime</span></span>|<span data-ttu-id="d2060-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2060-181">DateTimeOffset</span></span>|<span data-ttu-id="d2060-182">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="d2060-182">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="d2060-183">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-183">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2060-184">source</span><span class="sxs-lookup"><span data-stu-id="d2060-184">source</span></span>|[<span data-ttu-id="d2060-185">personDataSource</span><span class="sxs-lookup"><span data-stu-id="d2060-185">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="d2060-186">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="d2060-186">Where the values originated if synced from another service.</span></span> <span data-ttu-id="d2060-187">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d2060-187">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d2060-188">webUrl</span><span class="sxs-lookup"><span data-stu-id="d2060-188">webUrl</span></span>|<span data-ttu-id="d2060-189">String</span><span class="sxs-lookup"><span data-stu-id="d2060-189">String</span></span>|<span data-ttu-id="d2060-190">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="d2060-190">Contains a link to the website itself.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2060-191">关系</span><span class="sxs-lookup"><span data-stu-id="d2060-191">Relationships</span></span>
<span data-ttu-id="d2060-192">无。</span><span class="sxs-lookup"><span data-stu-id="d2060-192">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2060-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2060-193">JSON representation</span></span>
<span data-ttu-id="d2060-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2060-194">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
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
  "webUrl": "String"
}
```
