---
title: itemEmail 资源类型
description: itemEmail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a8a69ae484afab6b558890fbd186a4850235ead
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809425"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="0e0ed-103">itemEmail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e0ed-103">itemEmail resource type</span></span>

<span data-ttu-id="0e0ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e0ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e0ed-105">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-105">Represents detailed information about email addresses associated with the user.</span></span>

<span data-ttu-id="0e0ed-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0e0ed-107">方法</span><span class="sxs-lookup"><span data-stu-id="0e0ed-107">Methods</span></span>
|<span data-ttu-id="0e0ed-108">方法</span><span class="sxs-lookup"><span data-stu-id="0e0ed-108">Method</span></span>|<span data-ttu-id="0e0ed-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e0ed-109">Return type</span></span>|<span data-ttu-id="0e0ed-110">说明</span><span class="sxs-lookup"><span data-stu-id="0e0ed-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e0ed-111">列出电子邮件</span><span class="sxs-lookup"><span data-stu-id="0e0ed-111">List emails</span></span>](../api/profile-list-emails.md)|<span data-ttu-id="0e0ed-112">[itemEmail](../resources/itememail.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e0ed-112">[itemEmail](../resources/itememail.md) collection</span></span>|<span data-ttu-id="0e0ed-113">从 "电子邮件" 导航属性中获取 itemEmail 资源。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-113">Get the itemEmail resources from the emails navigation property.</span></span>|
|[<span data-ttu-id="0e0ed-114">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-114">Create itemEmail</span></span>](../api/profile-post-emails.md)|[<span data-ttu-id="0e0ed-115">itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-115">itemEmail</span></span>](../resources/itememail.md)|<span data-ttu-id="0e0ed-116">创建新的 itemEmail 对象。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-116">Create a new itemEmail object.</span></span>|
|[<span data-ttu-id="0e0ed-117">获取 itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-117">Get itemEmail</span></span>](../api/itememail-get.md)|[<span data-ttu-id="0e0ed-118">itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-118">itemEmail</span></span>](../resources/itememail.md)|<span data-ttu-id="0e0ed-119">读取 [itemEmail](../resources/itememail.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-119">Read the properties and relationships of an [itemEmail](../resources/itememail.md) object.</span></span>|
|[<span data-ttu-id="0e0ed-120">更新 itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-120">Update itemEmail</span></span>](../api/itememail-update.md)|[<span data-ttu-id="0e0ed-121">itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-121">itemEmail</span></span>](../resources/itememail.md)|<span data-ttu-id="0e0ed-122">更新 [itemEmail](../resources/itememail.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-122">Update the properties of an [itemEmail](../resources/itememail.md) object.</span></span>|
|[<span data-ttu-id="0e0ed-123">删除 itemEmail</span><span class="sxs-lookup"><span data-stu-id="0e0ed-123">Delete itemEmail</span></span>](../api/itememail-delete.md)|<span data-ttu-id="0e0ed-124">无</span><span class="sxs-lookup"><span data-stu-id="0e0ed-124">None</span></span>|<span data-ttu-id="0e0ed-125">删除一个 [itemEmail](../resources/itememail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-125">Deletes an [itemEmail](../resources/itememail.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e0ed-126">属性</span><span class="sxs-lookup"><span data-stu-id="0e0ed-126">Properties</span></span>
|<span data-ttu-id="0e0ed-127">属性</span><span class="sxs-lookup"><span data-stu-id="0e0ed-127">Property</span></span>|<span data-ttu-id="0e0ed-128">类型</span><span class="sxs-lookup"><span data-stu-id="0e0ed-128">Type</span></span>|<span data-ttu-id="0e0ed-129">说明</span><span class="sxs-lookup"><span data-stu-id="0e0ed-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e0ed-130">address</span><span class="sxs-lookup"><span data-stu-id="0e0ed-130">address</span></span>|<span data-ttu-id="0e0ed-131">String</span><span class="sxs-lookup"><span data-stu-id="0e0ed-131">String</span></span>|<span data-ttu-id="0e0ed-132">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-132">The email address itself.</span></span>|
|<span data-ttu-id="0e0ed-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="0e0ed-133">allowedAudiences</span></span>|<span data-ttu-id="0e0ed-134">String</span><span class="sxs-lookup"><span data-stu-id="0e0ed-134">String</span></span>|<span data-ttu-id="0e0ed-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0e0ed-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0e0ed-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0e0ed-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="0e0ed-138">createdBy</span></span>|[<span data-ttu-id="0e0ed-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="0e0ed-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="0e0ed-140">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="0e0ed-141">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0e0ed-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e0ed-142">createdDateTime</span></span>|<span data-ttu-id="0e0ed-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e0ed-143">DateTimeOffset</span></span>|<span data-ttu-id="0e0ed-144">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="0e0ed-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0e0ed-146">displayName</span><span class="sxs-lookup"><span data-stu-id="0e0ed-146">displayName</span></span>|<span data-ttu-id="0e0ed-147">String</span><span class="sxs-lookup"><span data-stu-id="0e0ed-147">String</span></span>|<span data-ttu-id="0e0ed-148">用户与特定电子邮件地址相关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-148">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="0e0ed-149">id</span><span class="sxs-lookup"><span data-stu-id="0e0ed-149">id</span></span>|<span data-ttu-id="0e0ed-150">String</span><span class="sxs-lookup"><span data-stu-id="0e0ed-150">String</span></span>|<span data-ttu-id="0e0ed-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="0e0ed-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="0e0ed-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="0e0ed-153">推导</span><span class="sxs-lookup"><span data-stu-id="0e0ed-153">inference</span></span>|[<span data-ttu-id="0e0ed-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="0e0ed-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0e0ed-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0e0ed-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0e0ed-157">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0e0ed-157">lastModifiedBy</span></span>|[<span data-ttu-id="0e0ed-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="0e0ed-158">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="0e0ed-159">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-159">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="0e0ed-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0e0ed-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e0ed-161">lastModifiedDateTime</span></span>|<span data-ttu-id="0e0ed-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e0ed-162">DateTimeOffset</span></span>|<span data-ttu-id="0e0ed-163">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-163">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="0e0ed-164">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0e0ed-165">source</span><span class="sxs-lookup"><span data-stu-id="0e0ed-165">source</span></span>|[<span data-ttu-id="0e0ed-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="0e0ed-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="0e0ed-167">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="0e0ed-168">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0e0ed-169">type</span><span class="sxs-lookup"><span data-stu-id="0e0ed-169">type</span></span>|<span data-ttu-id="0e0ed-170">emailType</span><span class="sxs-lookup"><span data-stu-id="0e0ed-170">emailType</span></span>|<span data-ttu-id="0e0ed-171">电子邮件地址的类型。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-171">The type of email address.</span></span> <span data-ttu-id="0e0ed-172">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-172">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e0ed-173">关系</span><span class="sxs-lookup"><span data-stu-id="0e0ed-173">Relationships</span></span>
<span data-ttu-id="0e0ed-174">无。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e0ed-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e0ed-175">JSON representation</span></span>
<span data-ttu-id="0e0ed-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e0ed-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemEmail",
  "id": "0f30bf5d-bf5d-0f30-5dbf-300f5dbf300f",
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
  "address": "String",
  "displayName": "String",
  "type": "String"
}
```
