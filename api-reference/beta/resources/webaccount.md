---
title: webAccount 资源类型
description: webAccount 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 29d66809d14cfc72d43286aef801490cef20cb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057675"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="bc34b-103">webAccount 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc34b-103">webAccount resource type</span></span>

<span data-ttu-id="bc34b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc34b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc34b-105">表示用户已向其用户 [配置文件](profile.md)中添加或已添加的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="bc34b-105">Represents web accounts the user has indicated they use or have added to their user [profile](profile.md).</span></span>

<span data-ttu-id="bc34b-106">此资源类型继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bc34b-107">方法</span><span class="sxs-lookup"><span data-stu-id="bc34b-107">Methods</span></span>

|<span data-ttu-id="bc34b-108">方法</span><span class="sxs-lookup"><span data-stu-id="bc34b-108">Method</span></span>|<span data-ttu-id="bc34b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc34b-109">Return type</span></span>|<span data-ttu-id="bc34b-110">说明</span><span class="sxs-lookup"><span data-stu-id="bc34b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc34b-111">列出 webAccounts</span><span class="sxs-lookup"><span data-stu-id="bc34b-111">List webAccounts</span></span>](../api/profile-list-webaccounts.md)|<span data-ttu-id="bc34b-112">[webAccount](../resources/webaccount.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc34b-112">[webAccount](../resources/webaccount.md) collection</span></span>|<span data-ttu-id="bc34b-113">从 webAccounts 导航属性中获取 webAccount 资源。</span><span class="sxs-lookup"><span data-stu-id="bc34b-113">Get the webAccount resources from the webAccounts navigation property.</span></span>|
|[<span data-ttu-id="bc34b-114">创建 webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-114">Create webAccount</span></span>](../api/profile-post-webaccounts.md)|[<span data-ttu-id="bc34b-115">webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-115">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="bc34b-116">创建新的 webAccount 对象。</span><span class="sxs-lookup"><span data-stu-id="bc34b-116">Create a new webAccount object.</span></span>|
|[<span data-ttu-id="bc34b-117">获取 webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-117">Get webAccount</span></span>](../api/webaccount-get.md)|[<span data-ttu-id="bc34b-118">webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-118">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="bc34b-119">读取 [webAccount](../resources/webaccount.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc34b-119">Read the properties and relationships of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="bc34b-120">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-120">Update webAccount</span></span>](../api/webaccount-update.md)|[<span data-ttu-id="bc34b-121">webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-121">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="bc34b-122">更新 [webAccount](../resources/webaccount.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc34b-122">Update the properties of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="bc34b-123">删除 webAccount</span><span class="sxs-lookup"><span data-stu-id="bc34b-123">Delete webAccount</span></span>](../api/webaccount-delete.md)|<span data-ttu-id="bc34b-124">无</span><span class="sxs-lookup"><span data-stu-id="bc34b-124">None</span></span>|<span data-ttu-id="bc34b-125">删除一个 [webAccount](../resources/webaccount.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc34b-125">Deletes a [webAccount](../resources/webaccount.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc34b-126">属性</span><span class="sxs-lookup"><span data-stu-id="bc34b-126">Properties</span></span>

|<span data-ttu-id="bc34b-127">属性</span><span class="sxs-lookup"><span data-stu-id="bc34b-127">Property</span></span>|<span data-ttu-id="bc34b-128">类型</span><span class="sxs-lookup"><span data-stu-id="bc34b-128">Type</span></span>|<span data-ttu-id="bc34b-129">说明</span><span class="sxs-lookup"><span data-stu-id="bc34b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc34b-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="bc34b-130">allowedAudiences</span></span>|<span data-ttu-id="bc34b-131">String</span><span class="sxs-lookup"><span data-stu-id="bc34b-131">String</span></span>|<span data-ttu-id="bc34b-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="bc34b-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="bc34b-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="bc34b-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bc34b-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bc34b-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="bc34b-135">createdBy</span></span>|[<span data-ttu-id="bc34b-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="bc34b-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="bc34b-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="bc34b-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="bc34b-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc34b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc34b-139">createdDateTime</span></span>|<span data-ttu-id="bc34b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc34b-140">DateTimeOffset</span></span>|<span data-ttu-id="bc34b-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="bc34b-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="bc34b-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc34b-143">说明</span><span class="sxs-lookup"><span data-stu-id="bc34b-143">description</span></span>|<span data-ttu-id="bc34b-144">String</span><span class="sxs-lookup"><span data-stu-id="bc34b-144">String</span></span>|<span data-ttu-id="bc34b-145">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="bc34b-145">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="bc34b-146">id</span><span class="sxs-lookup"><span data-stu-id="bc34b-146">id</span></span>|<span data-ttu-id="bc34b-147">String</span><span class="sxs-lookup"><span data-stu-id="bc34b-147">String</span></span>|<span data-ttu-id="bc34b-148">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="bc34b-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="bc34b-149">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="bc34b-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="bc34b-150">推导</span><span class="sxs-lookup"><span data-stu-id="bc34b-150">inference</span></span>|[<span data-ttu-id="bc34b-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="bc34b-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="bc34b-152">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="bc34b-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="bc34b-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc34b-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bc34b-154">lastModifiedBy</span></span>|[<span data-ttu-id="bc34b-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="bc34b-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="bc34b-156">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="bc34b-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="bc34b-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc34b-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc34b-158">lastModifiedDateTime</span></span>|<span data-ttu-id="bc34b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc34b-159">DateTimeOffset</span></span>|<span data-ttu-id="bc34b-160">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="bc34b-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="bc34b-161">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc34b-162">service</span><span class="sxs-lookup"><span data-stu-id="bc34b-162">service</span></span>|[<span data-ttu-id="bc34b-163">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="bc34b-163">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="bc34b-164">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="bc34b-164">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="bc34b-165">source</span><span class="sxs-lookup"><span data-stu-id="bc34b-165">source</span></span>|[<span data-ttu-id="bc34b-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="bc34b-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="bc34b-167">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="bc34b-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="bc34b-168">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bc34b-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bc34b-169">statusMessage</span><span class="sxs-lookup"><span data-stu-id="bc34b-169">statusMessage</span></span>|<span data-ttu-id="bc34b-170">String</span><span class="sxs-lookup"><span data-stu-id="bc34b-170">String</span></span>|<span data-ttu-id="bc34b-171">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="bc34b-171">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="bc34b-172">userId</span><span class="sxs-lookup"><span data-stu-id="bc34b-172">userId</span></span>|<span data-ttu-id="bc34b-173">String</span><span class="sxs-lookup"><span data-stu-id="bc34b-173">String</span></span>|<span data-ttu-id="bc34b-174">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="bc34b-174">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="bc34b-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="bc34b-175">webUrl</span></span>|<span data-ttu-id="bc34b-176">String</span><span class="sxs-lookup"><span data-stu-id="bc34b-176">String</span></span>|<span data-ttu-id="bc34b-177">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="bc34b-177">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc34b-178">关系</span><span class="sxs-lookup"><span data-stu-id="bc34b-178">Relationships</span></span>
<span data-ttu-id="bc34b-179">无。</span><span class="sxs-lookup"><span data-stu-id="bc34b-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc34b-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc34b-180">JSON representation</span></span>
<span data-ttu-id="bc34b-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc34b-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webAccount",
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
  "userId": "String",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation"
  },
  "statusMessage": "String",
  "webUrl": "String"
}
```


