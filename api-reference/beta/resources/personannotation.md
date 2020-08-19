---
title: personAnnotation 资源类型
description: personAnnotation 资源类型
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 757797a8a252f934050cb8425f49042707734ed5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812952"
---
# <a name="personannotation-resource-type"></a><span data-ttu-id="365be-103">personAnnotation 资源类型</span><span class="sxs-lookup"><span data-stu-id="365be-103">personAnnotation resource type</span></span>

<span data-ttu-id="365be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="365be-105">提供笔记中的信息，用户在各种服务中与自身关联，并与其他人共享。</span><span class="sxs-lookup"><span data-stu-id="365be-105">Provides information within notes that the user has associated with themselves in various services and shared with others.</span></span>

<span data-ttu-id="365be-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="365be-107">方法</span><span class="sxs-lookup"><span data-stu-id="365be-107">Methods</span></span>
|<span data-ttu-id="365be-108">方法</span><span class="sxs-lookup"><span data-stu-id="365be-108">Method</span></span>|<span data-ttu-id="365be-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="365be-109">Return type</span></span>|<span data-ttu-id="365be-110">说明</span><span class="sxs-lookup"><span data-stu-id="365be-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="365be-111">列出笔记</span><span class="sxs-lookup"><span data-stu-id="365be-111">List notes</span></span>](../api/profile-list-notes.md)|<span data-ttu-id="365be-112">[personAnnotation](../resources/personannotation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="365be-112">[personAnnotation](../resources/personannotation.md) collection</span></span>|<span data-ttu-id="365be-113">从 "便笺" 导航属性中获取 personAnnotation 资源。</span><span class="sxs-lookup"><span data-stu-id="365be-113">Get the personAnnotation resources from the notes navigation property.</span></span>|
|[<span data-ttu-id="365be-114">创建 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-114">Create personAnnotation</span></span>](../api/profile-post-notes.md)|[<span data-ttu-id="365be-115">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-115">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="365be-116">创建新的 personAnnotation 对象。</span><span class="sxs-lookup"><span data-stu-id="365be-116">Create a new personAnnotation object.</span></span>|
|[<span data-ttu-id="365be-117">获取 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-117">Get personAnnotation</span></span>](../api/personannotation-get.md)|[<span data-ttu-id="365be-118">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-118">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="365be-119">读取 [personAnnotation](../resources/personannotation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="365be-119">Read the properties and relationships of a [personAnnotation](../resources/personannotation.md) object.</span></span>|
|[<span data-ttu-id="365be-120">更新 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-120">Update personAnnotation</span></span>](../api/personannotation-update.md)|[<span data-ttu-id="365be-121">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-121">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="365be-122">更新 [personAnnotation](../resources/personannotation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="365be-122">Update the properties of a [personAnnotation](../resources/personannotation.md) object.</span></span>|
|[<span data-ttu-id="365be-123">删除 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="365be-123">Delete personAnnotation</span></span>](../api/personannotation-delete.md)|<span data-ttu-id="365be-124">无</span><span class="sxs-lookup"><span data-stu-id="365be-124">None</span></span>|<span data-ttu-id="365be-125">删除一个 [personAnnotation](../resources/personannotation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="365be-125">Deletes a [personAnnotation](../resources/personannotation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="365be-126">属性</span><span class="sxs-lookup"><span data-stu-id="365be-126">Properties</span></span>
|<span data-ttu-id="365be-127">属性</span><span class="sxs-lookup"><span data-stu-id="365be-127">Property</span></span>|<span data-ttu-id="365be-128">类型</span><span class="sxs-lookup"><span data-stu-id="365be-128">Type</span></span>|<span data-ttu-id="365be-129">说明</span><span class="sxs-lookup"><span data-stu-id="365be-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365be-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="365be-130">allowedAudiences</span></span>|<span data-ttu-id="365be-131">String</span><span class="sxs-lookup"><span data-stu-id="365be-131">String</span></span>|<span data-ttu-id="365be-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="365be-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="365be-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="365be-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="365be-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="365be-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="365be-135">createdBy</span></span>|[<span data-ttu-id="365be-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="365be-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="365be-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="365be-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="365be-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="365be-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="365be-139">createdDateTime</span></span>|<span data-ttu-id="365be-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365be-140">DateTimeOffset</span></span>|<span data-ttu-id="365be-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="365be-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="365be-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="365be-143">介绍</span><span class="sxs-lookup"><span data-stu-id="365be-143">detail</span></span>|[<span data-ttu-id="365be-144">itemBody</span><span class="sxs-lookup"><span data-stu-id="365be-144">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="365be-145">包含注释本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="365be-145">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="365be-146">displayName</span><span class="sxs-lookup"><span data-stu-id="365be-146">displayName</span></span>|<span data-ttu-id="365be-147">String</span><span class="sxs-lookup"><span data-stu-id="365be-147">String</span></span>|<span data-ttu-id="365be-148">包含注解的友好名称。</span><span class="sxs-lookup"><span data-stu-id="365be-148">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="365be-149">id</span><span class="sxs-lookup"><span data-stu-id="365be-149">id</span></span>|<span data-ttu-id="365be-150">String</span><span class="sxs-lookup"><span data-stu-id="365be-150">String</span></span>|<span data-ttu-id="365be-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="365be-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="365be-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="365be-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="365be-153">推导</span><span class="sxs-lookup"><span data-stu-id="365be-153">inference</span></span>|[<span data-ttu-id="365be-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="365be-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="365be-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="365be-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="365be-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="365be-157">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="365be-157">lastModifiedBy</span></span>|[<span data-ttu-id="365be-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="365be-158">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="365be-159">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="365be-159">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="365be-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="365be-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="365be-161">lastModifiedDateTime</span></span>|<span data-ttu-id="365be-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365be-162">DateTimeOffset</span></span>|<span data-ttu-id="365be-163">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="365be-163">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="365be-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="365be-165">source</span><span class="sxs-lookup"><span data-stu-id="365be-165">source</span></span>|[<span data-ttu-id="365be-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="365be-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="365be-167">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="365be-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="365be-168">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="365be-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="365be-169">关系</span><span class="sxs-lookup"><span data-stu-id="365be-169">Relationships</span></span>
<span data-ttu-id="365be-170">无。</span><span class="sxs-lookup"><span data-stu-id="365be-170">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="365be-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="365be-171">JSON representation</span></span>
<span data-ttu-id="365be-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="365be-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnnotation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnnotation",
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
  "detail": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "displayName": "String"
}
```
