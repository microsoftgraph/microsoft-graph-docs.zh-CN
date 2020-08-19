---
title: personAward 资源类型
description: personAward 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 3031994e3b19fdd3962118c21d86a334c63781ea
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812951"
---
# <a name="personaward-resource-type"></a><span data-ttu-id="9d985-103">personAward 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d985-103">personAward resource type</span></span>

<span data-ttu-id="9d985-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d985-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d985-105">表示已与用户的 [配置文件](../resources/profile.md)关联的奖项。</span><span class="sxs-lookup"><span data-stu-id="9d985-105">Represents an award that has been associated with a user's [profile](../resources/profile.md).</span></span>

<span data-ttu-id="9d985-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9d985-107">方法</span><span class="sxs-lookup"><span data-stu-id="9d985-107">Methods</span></span>
|<span data-ttu-id="9d985-108">方法</span><span class="sxs-lookup"><span data-stu-id="9d985-108">Method</span></span>|<span data-ttu-id="9d985-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d985-109">Return type</span></span>|<span data-ttu-id="9d985-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d985-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d985-111">列表奖项</span><span class="sxs-lookup"><span data-stu-id="9d985-111">List awards</span></span>](../api/profile-list-awards.md)|<span data-ttu-id="9d985-112">[personAward](../resources/personaward.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9d985-112">[personAward](../resources/personaward.md) collection</span></span>|<span data-ttu-id="9d985-113">从奖项导航属性中获取 personAward 资源。</span><span class="sxs-lookup"><span data-stu-id="9d985-113">Get the personAward resources from the awards navigation property.</span></span>|
|[<span data-ttu-id="9d985-114">创建 personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-114">Create personAward</span></span>](../api/profile-post-awards.md)|[<span data-ttu-id="9d985-115">personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-115">personAward</span></span>](../resources/personaward.md)|<span data-ttu-id="9d985-116">创建新的 personAward 对象。</span><span class="sxs-lookup"><span data-stu-id="9d985-116">Create a new personAward object.</span></span>|
|[<span data-ttu-id="9d985-117">获取 personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-117">Get personAward</span></span>](../api/personaward-get.md)|[<span data-ttu-id="9d985-118">personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-118">personAward</span></span>](../resources/personaward.md)|<span data-ttu-id="9d985-119">读取 [personAward](../resources/personaward.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9d985-119">Read the properties and relationships of an [personAward](../resources/personaward.md) object.</span></span>|
|[<span data-ttu-id="9d985-120">更新 personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-120">Update personAward</span></span>](../api/personaward-update.md)|[<span data-ttu-id="9d985-121">personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-121">personAward</span></span>](../resources/personaward.md)|<span data-ttu-id="9d985-122">更新 [personAward](../resources/personaward.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d985-122">Update the properties of an [personAward](../resources/personaward.md) object.</span></span>|
|[<span data-ttu-id="9d985-123">删除 personAward</span><span class="sxs-lookup"><span data-stu-id="9d985-123">Delete personAward</span></span>](../api/personaward-delete.md)|<span data-ttu-id="9d985-124">无</span><span class="sxs-lookup"><span data-stu-id="9d985-124">None</span></span>|<span data-ttu-id="9d985-125">删除一个 [personAward](../resources/personaward.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d985-125">Deletes an [personAward](../resources/personaward.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d985-126">属性</span><span class="sxs-lookup"><span data-stu-id="9d985-126">Properties</span></span>
|<span data-ttu-id="9d985-127">属性</span><span class="sxs-lookup"><span data-stu-id="9d985-127">Property</span></span>|<span data-ttu-id="9d985-128">类型</span><span class="sxs-lookup"><span data-stu-id="9d985-128">Type</span></span>|<span data-ttu-id="9d985-129">说明</span><span class="sxs-lookup"><span data-stu-id="9d985-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d985-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="9d985-130">allowedAudiences</span></span>|<span data-ttu-id="9d985-131">String</span><span class="sxs-lookup"><span data-stu-id="9d985-131">String</span></span>|<span data-ttu-id="9d985-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="9d985-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="9d985-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="9d985-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9d985-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9d985-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="9d985-135">createdBy</span></span>|[<span data-ttu-id="9d985-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="9d985-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="9d985-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="9d985-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="9d985-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d985-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d985-139">createdDateTime</span></span>|<span data-ttu-id="9d985-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d985-140">DateTimeOffset</span></span>|<span data-ttu-id="9d985-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="9d985-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="9d985-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d985-143">description</span><span class="sxs-lookup"><span data-stu-id="9d985-143">description</span></span>|<span data-ttu-id="9d985-144">String</span><span class="sxs-lookup"><span data-stu-id="9d985-144">String</span></span>|<span data-ttu-id="9d985-145">奖励或荣誉的 Descpription。</span><span class="sxs-lookup"><span data-stu-id="9d985-145">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="9d985-146">displayName</span><span class="sxs-lookup"><span data-stu-id="9d985-146">displayName</span></span>|<span data-ttu-id="9d985-147">String</span><span class="sxs-lookup"><span data-stu-id="9d985-147">String</span></span>|<span data-ttu-id="9d985-148">获奖或荣誉的名称。</span><span class="sxs-lookup"><span data-stu-id="9d985-148">Name of the award or honor.</span></span> |
|<span data-ttu-id="9d985-149">id</span><span class="sxs-lookup"><span data-stu-id="9d985-149">id</span></span>|<span data-ttu-id="9d985-150">String</span><span class="sxs-lookup"><span data-stu-id="9d985-150">String</span></span>|<span data-ttu-id="9d985-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="9d985-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="9d985-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="9d985-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="9d985-153">推导</span><span class="sxs-lookup"><span data-stu-id="9d985-153">inference</span></span>|[<span data-ttu-id="9d985-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="9d985-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="9d985-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="9d985-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="9d985-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d985-157">issuedDate</span><span class="sxs-lookup"><span data-stu-id="9d985-157">issuedDate</span></span>|<span data-ttu-id="9d985-158">日期</span><span class="sxs-lookup"><span data-stu-id="9d985-158">Date</span></span>|<span data-ttu-id="9d985-159">授予获奖或荣誉的日期。</span><span class="sxs-lookup"><span data-stu-id="9d985-159">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="9d985-160">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="9d985-160">issuingAuthority</span></span>|<span data-ttu-id="9d985-161">String</span><span class="sxs-lookup"><span data-stu-id="9d985-161">String</span></span>|<span data-ttu-id="9d985-162">授予奖项的证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="9d985-162">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="9d985-163">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9d985-163">lastModifiedBy</span></span>|[<span data-ttu-id="9d985-164">identitySet</span><span class="sxs-lookup"><span data-stu-id="9d985-164">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="9d985-165">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="9d985-165">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="9d985-166">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-166">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d985-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d985-167">lastModifiedDateTime</span></span>|<span data-ttu-id="9d985-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d985-168">DateTimeOffset</span></span>|<span data-ttu-id="9d985-169">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="9d985-169">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="9d985-170">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-170">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d985-171">source</span><span class="sxs-lookup"><span data-stu-id="9d985-171">source</span></span>|[<span data-ttu-id="9d985-172">personDataSource</span><span class="sxs-lookup"><span data-stu-id="9d985-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="9d985-173">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="9d985-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="9d985-174">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d985-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d985-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="9d985-175">thumbnailUrl</span></span>|<span data-ttu-id="9d985-176">String</span><span class="sxs-lookup"><span data-stu-id="9d985-176">String</span></span>|<span data-ttu-id="9d985-177">URL 引用获奖或荣誉的缩略图。</span><span class="sxs-lookup"><span data-stu-id="9d985-177">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="9d985-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="9d985-178">webUrl</span></span>|<span data-ttu-id="9d985-179">String</span><span class="sxs-lookup"><span data-stu-id="9d985-179">String</span></span>|<span data-ttu-id="9d985-180">引用奖项或荣誉的 URL。</span><span class="sxs-lookup"><span data-stu-id="9d985-180">URL referencing the award or honor.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d985-181">关系</span><span class="sxs-lookup"><span data-stu-id="9d985-181">Relationships</span></span>
<span data-ttu-id="9d985-182">无。</span><span class="sxs-lookup"><span data-stu-id="9d985-182">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d985-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d985-183">JSON representation</span></span>
<span data-ttu-id="9d985-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d985-184">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAward",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAward",
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
  "description": "String",
  "displayName": "String",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```
