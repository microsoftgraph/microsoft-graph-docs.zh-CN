---
title: personAnnotation 资源类型
description: personAnnotation 资源类型
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 403df171498bcde62d113ce2a2f2a27cf3987285
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997968"
---
# <a name="personannotation-resource-type"></a><span data-ttu-id="ee140-103">personAnnotation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee140-103">personAnnotation resource type</span></span>

<span data-ttu-id="ee140-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee140-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee140-105">提供笔记中的信息，用户在各种服务中与自身关联，并与其他人共享。</span><span class="sxs-lookup"><span data-stu-id="ee140-105">Provides information within notes that the user has associated with themselves in various services and shared with others.</span></span>

<span data-ttu-id="ee140-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ee140-107">方法</span><span class="sxs-lookup"><span data-stu-id="ee140-107">Methods</span></span>
|<span data-ttu-id="ee140-108">方法</span><span class="sxs-lookup"><span data-stu-id="ee140-108">Method</span></span>|<span data-ttu-id="ee140-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ee140-109">Return type</span></span>|<span data-ttu-id="ee140-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee140-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee140-111">列出笔记</span><span class="sxs-lookup"><span data-stu-id="ee140-111">List notes</span></span>](../api/profile-list-notes.md)|<span data-ttu-id="ee140-112">[personAnnotation](../resources/personannotation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee140-112">[personAnnotation](../resources/personannotation.md) collection</span></span>|<span data-ttu-id="ee140-113">从 "便笺" 导航属性中获取 personAnnotation 资源。</span><span class="sxs-lookup"><span data-stu-id="ee140-113">Get the personAnnotation resources from the notes navigation property.</span></span>|
|[<span data-ttu-id="ee140-114">创建 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-114">Create personAnnotation</span></span>](../api/profile-post-notes.md)|[<span data-ttu-id="ee140-115">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-115">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="ee140-116">创建新的 personAnnotation 对象。</span><span class="sxs-lookup"><span data-stu-id="ee140-116">Create a new personAnnotation object.</span></span>|
|[<span data-ttu-id="ee140-117">获取 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-117">Get personAnnotation</span></span>](../api/personannotation-get.md)|[<span data-ttu-id="ee140-118">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-118">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="ee140-119">读取 [personAnnotation](../resources/personannotation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ee140-119">Read the properties and relationships of a [personAnnotation](../resources/personannotation.md) object.</span></span>|
|[<span data-ttu-id="ee140-120">更新 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-120">Update personAnnotation</span></span>](../api/personannotation-update.md)|[<span data-ttu-id="ee140-121">personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-121">personAnnotation</span></span>](../resources/personannotation.md)|<span data-ttu-id="ee140-122">更新 [personAnnotation](../resources/personannotation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ee140-122">Update the properties of a [personAnnotation](../resources/personannotation.md) object.</span></span>|
|[<span data-ttu-id="ee140-123">删除 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="ee140-123">Delete personAnnotation</span></span>](../api/personannotation-delete.md)|<span data-ttu-id="ee140-124">无</span><span class="sxs-lookup"><span data-stu-id="ee140-124">None</span></span>|<span data-ttu-id="ee140-125">删除一个 [personAnnotation](../resources/personannotation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee140-125">Deletes a [personAnnotation](../resources/personannotation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee140-126">属性</span><span class="sxs-lookup"><span data-stu-id="ee140-126">Properties</span></span>
|<span data-ttu-id="ee140-127">属性</span><span class="sxs-lookup"><span data-stu-id="ee140-127">Property</span></span>|<span data-ttu-id="ee140-128">类型</span><span class="sxs-lookup"><span data-stu-id="ee140-128">Type</span></span>|<span data-ttu-id="ee140-129">说明</span><span class="sxs-lookup"><span data-stu-id="ee140-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee140-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ee140-130">allowedAudiences</span></span>|<span data-ttu-id="ee140-131">String</span><span class="sxs-lookup"><span data-stu-id="ee140-131">String</span></span>|<span data-ttu-id="ee140-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="ee140-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ee140-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ee140-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ee140-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ee140-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="ee140-135">createdBy</span></span>|[<span data-ttu-id="ee140-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee140-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ee140-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="ee140-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="ee140-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ee140-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee140-139">createdDateTime</span></span>|<span data-ttu-id="ee140-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee140-140">DateTimeOffset</span></span>|<span data-ttu-id="ee140-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="ee140-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="ee140-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ee140-143">介绍</span><span class="sxs-lookup"><span data-stu-id="ee140-143">detail</span></span>|[<span data-ttu-id="ee140-144">itemBody</span><span class="sxs-lookup"><span data-stu-id="ee140-144">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="ee140-145">包含注释本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee140-145">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="ee140-146">displayName</span><span class="sxs-lookup"><span data-stu-id="ee140-146">displayName</span></span>|<span data-ttu-id="ee140-147">String</span><span class="sxs-lookup"><span data-stu-id="ee140-147">String</span></span>|<span data-ttu-id="ee140-148">包含注解的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ee140-148">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="ee140-149">id</span><span class="sxs-lookup"><span data-stu-id="ee140-149">id</span></span>|<span data-ttu-id="ee140-150">String</span><span class="sxs-lookup"><span data-stu-id="ee140-150">String</span></span>|<span data-ttu-id="ee140-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="ee140-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="ee140-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="ee140-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="ee140-153">推导</span><span class="sxs-lookup"><span data-stu-id="ee140-153">inference</span></span>|[<span data-ttu-id="ee140-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ee140-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ee140-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee140-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ee140-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ee140-157">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ee140-157">lastModifiedBy</span></span>|[<span data-ttu-id="ee140-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee140-158">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ee140-159">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="ee140-159">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="ee140-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ee140-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee140-161">lastModifiedDateTime</span></span>|<span data-ttu-id="ee140-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee140-162">DateTimeOffset</span></span>|<span data-ttu-id="ee140-163">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="ee140-163">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="ee140-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ee140-165">source</span><span class="sxs-lookup"><span data-stu-id="ee140-165">source</span></span>|[<span data-ttu-id="ee140-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="ee140-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ee140-167">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="ee140-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ee140-168">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee140-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee140-169">关系</span><span class="sxs-lookup"><span data-stu-id="ee140-169">Relationships</span></span>
<span data-ttu-id="ee140-170">无。</span><span class="sxs-lookup"><span data-stu-id="ee140-170">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee140-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee140-171">JSON representation</span></span>
<span data-ttu-id="ee140-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee140-172">The following is a JSON representation of the resource.</span></span>
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


