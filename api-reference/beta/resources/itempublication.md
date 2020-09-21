---
title: itemPublication 资源类型
description: itemPublication 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 59b30c08e78db52af9e10c6aac2550dc02c11e62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084000"
---
# <a name="itempublication-resource-type"></a><span data-ttu-id="12630-103">itemPublication 资源类型</span><span class="sxs-lookup"><span data-stu-id="12630-103">itemPublication resource type</span></span>

<span data-ttu-id="12630-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12630-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12630-105">表示已与用户的 [配置文件](../resources/profile.md)相关联的出版物或文章。</span><span class="sxs-lookup"><span data-stu-id="12630-105">Represents a publication or article that has been associated with a user's [profile](../resources/profile.md).</span></span>

<span data-ttu-id="12630-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="12630-107">方法</span><span class="sxs-lookup"><span data-stu-id="12630-107">Methods</span></span>
|<span data-ttu-id="12630-108">方法</span><span class="sxs-lookup"><span data-stu-id="12630-108">Method</span></span>|<span data-ttu-id="12630-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="12630-109">Return type</span></span>|<span data-ttu-id="12630-110">说明</span><span class="sxs-lookup"><span data-stu-id="12630-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12630-111">列出出版物</span><span class="sxs-lookup"><span data-stu-id="12630-111">List publications</span></span>](../api/profile-list-publications.md)|<span data-ttu-id="12630-112">[itemPublication](../resources/itempublication.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12630-112">[itemPublication](../resources/itempublication.md) collection</span></span>|<span data-ttu-id="12630-113">从 "发布" 导航属性中获取 itemPublication 资源。</span><span class="sxs-lookup"><span data-stu-id="12630-113">Get the itemPublication resources from the publications navigation property.</span></span>|
|[<span data-ttu-id="12630-114">创建 itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-114">Create itemPublication</span></span>](../api/profile-post-publications.md)|[<span data-ttu-id="12630-115">itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-115">itemPublication</span></span>](../resources/itempublication.md)|<span data-ttu-id="12630-116">创建新的 itemPublication 对象。</span><span class="sxs-lookup"><span data-stu-id="12630-116">Create a new itemPublication object.</span></span>|
|[<span data-ttu-id="12630-117">获取 itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-117">Get itemPublication</span></span>](../api/itempublication-get.md)|[<span data-ttu-id="12630-118">itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-118">itemPublication</span></span>](../resources/itempublication.md)|<span data-ttu-id="12630-119">读取 [itemPublication](../resources/itempublication.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12630-119">Read the properties and relationships of an [itemPublication](../resources/itempublication.md) object.</span></span>|
|[<span data-ttu-id="12630-120">更新 itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-120">Update itemPublication</span></span>](../api/itempublication-update.md)|[<span data-ttu-id="12630-121">itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-121">itemPublication</span></span>](../resources/itempublication.md)|<span data-ttu-id="12630-122">更新 [itemPublication](../resources/itempublication.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12630-122">Update the properties of an [itemPublication](../resources/itempublication.md) object.</span></span>|
|[<span data-ttu-id="12630-123">删除 itemPublication</span><span class="sxs-lookup"><span data-stu-id="12630-123">Delete itemPublication</span></span>](../api/itempublication-delete.md)|<span data-ttu-id="12630-124">无</span><span class="sxs-lookup"><span data-stu-id="12630-124">None</span></span>|<span data-ttu-id="12630-125">删除一个 [itemPublication](../resources/itempublication.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12630-125">Deletes an [itemPublication](../resources/itempublication.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12630-126">属性</span><span class="sxs-lookup"><span data-stu-id="12630-126">Properties</span></span>
|<span data-ttu-id="12630-127">属性</span><span class="sxs-lookup"><span data-stu-id="12630-127">Property</span></span>|<span data-ttu-id="12630-128">类型</span><span class="sxs-lookup"><span data-stu-id="12630-128">Type</span></span>|<span data-ttu-id="12630-129">说明</span><span class="sxs-lookup"><span data-stu-id="12630-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12630-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="12630-130">allowedAudiences</span></span>|<span data-ttu-id="12630-131">字符串</span><span class="sxs-lookup"><span data-stu-id="12630-131">String</span></span>|<span data-ttu-id="12630-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="12630-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="12630-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="12630-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="12630-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="12630-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="12630-135">createdBy</span></span>|[<span data-ttu-id="12630-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="12630-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="12630-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="12630-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="12630-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="12630-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12630-139">createdDateTime</span></span>|<span data-ttu-id="12630-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12630-140">DateTimeOffset</span></span>|<span data-ttu-id="12630-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="12630-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="12630-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="12630-143">说明</span><span class="sxs-lookup"><span data-stu-id="12630-143">description</span></span>    |<span data-ttu-id="12630-144">字符串</span><span class="sxs-lookup"><span data-stu-id="12630-144">String</span></span>      |<span data-ttu-id="12630-145">出版物的说明。</span><span class="sxs-lookup"><span data-stu-id="12630-145">Description of the publication.</span></span>                   |
|<span data-ttu-id="12630-146">displayName</span><span class="sxs-lookup"><span data-stu-id="12630-146">displayName</span></span>    |<span data-ttu-id="12630-147">字符串</span><span class="sxs-lookup"><span data-stu-id="12630-147">String</span></span>      |<span data-ttu-id="12630-148">出版物的标题。</span><span class="sxs-lookup"><span data-stu-id="12630-148">Title of the publication.</span></span>                         |
|<span data-ttu-id="12630-149">id</span><span class="sxs-lookup"><span data-stu-id="12630-149">id</span></span>|<span data-ttu-id="12630-150">字符串</span><span class="sxs-lookup"><span data-stu-id="12630-150">String</span></span>|<span data-ttu-id="12630-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="12630-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="12630-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="12630-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="12630-153">推导</span><span class="sxs-lookup"><span data-stu-id="12630-153">inference</span></span>|[<span data-ttu-id="12630-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="12630-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="12630-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="12630-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="12630-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="12630-157">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="12630-157">lastModifiedBy</span></span>|[<span data-ttu-id="12630-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="12630-158">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="12630-159">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="12630-159">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="12630-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="12630-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12630-161">lastModifiedDateTime</span></span>|<span data-ttu-id="12630-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12630-162">DateTimeOffset</span></span>|<span data-ttu-id="12630-163">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="12630-163">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="12630-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="12630-165">publishedDate</span><span class="sxs-lookup"><span data-stu-id="12630-165">publishedDate</span></span>  |<span data-ttu-id="12630-166">日期</span><span class="sxs-lookup"><span data-stu-id="12630-166">Date</span></span>        |<span data-ttu-id="12630-167">发布出版物的日期。</span><span class="sxs-lookup"><span data-stu-id="12630-167">The date that the publication was published.</span></span>      |
|<span data-ttu-id="12630-168">发布者</span><span class="sxs-lookup"><span data-stu-id="12630-168">publisher</span></span>      |<span data-ttu-id="12630-169">String</span><span class="sxs-lookup"><span data-stu-id="12630-169">String</span></span>      |<span data-ttu-id="12630-170">出版物的出版物或发布者。</span><span class="sxs-lookup"><span data-stu-id="12630-170">Publication or publisher for the publication.</span></span>     |
|<span data-ttu-id="12630-171">source</span><span class="sxs-lookup"><span data-stu-id="12630-171">source</span></span>|[<span data-ttu-id="12630-172">personDataSource</span><span class="sxs-lookup"><span data-stu-id="12630-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="12630-173">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="12630-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="12630-174">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="12630-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="12630-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="12630-175">thumbnailUrl</span></span>   |<span data-ttu-id="12630-176">字符串</span><span class="sxs-lookup"><span data-stu-id="12630-176">String</span></span>      |<span data-ttu-id="12630-177">URL 引用出版物的缩略图。</span><span class="sxs-lookup"><span data-stu-id="12630-177">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="12630-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="12630-178">webUrl</span></span>         |<span data-ttu-id="12630-179">String</span><span class="sxs-lookup"><span data-stu-id="12630-179">String</span></span>      |<span data-ttu-id="12630-180">引用发布的 URL。</span><span class="sxs-lookup"><span data-stu-id="12630-180">URL referencing the publication.</span></span>                  |

## <a name="relationships"></a><span data-ttu-id="12630-181">关系</span><span class="sxs-lookup"><span data-stu-id="12630-181">Relationships</span></span>
<span data-ttu-id="12630-182">无。</span><span class="sxs-lookup"><span data-stu-id="12630-182">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12630-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12630-183">JSON representation</span></span>
<span data-ttu-id="12630-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12630-184">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPublication",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPublication",
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
  "publishedDate": "Date",
  "publisher": "String",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```


