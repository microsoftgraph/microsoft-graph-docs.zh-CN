---
title: itemPatent 资源类型
description: itemPatent 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4b8a5c72117e20a73fb3c3b6b8a2af308219b69d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809636"
---
# <a name="itempatent-resource-type"></a><span data-ttu-id="732d9-103">itemPatent 资源类型</span><span class="sxs-lookup"><span data-stu-id="732d9-103">itemPatent resource type</span></span>
 
<span data-ttu-id="732d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="732d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="732d9-105">代表已添加到用户 [配置文件](../resources/profile.md)中的已授权或已存档的专利。</span><span class="sxs-lookup"><span data-stu-id="732d9-105">Represents a granted or filed patent which has been added to a user's [profile](../resources/profile.md).</span></span>

<span data-ttu-id="732d9-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="732d9-107">方法</span><span class="sxs-lookup"><span data-stu-id="732d9-107">Methods</span></span>
|<span data-ttu-id="732d9-108">方法</span><span class="sxs-lookup"><span data-stu-id="732d9-108">Method</span></span>|<span data-ttu-id="732d9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="732d9-109">Return type</span></span>|<span data-ttu-id="732d9-110">说明</span><span class="sxs-lookup"><span data-stu-id="732d9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="732d9-111">列出专利</span><span class="sxs-lookup"><span data-stu-id="732d9-111">List patents</span></span>](../api/profile-list-patents.md)|<span data-ttu-id="732d9-112">[itemPatent](../resources/itempatent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="732d9-112">[itemPatent](../resources/itempatent.md) collection</span></span>|<span data-ttu-id="732d9-113">从专利导航属性中获取 itemPatent 资源。</span><span class="sxs-lookup"><span data-stu-id="732d9-113">Get the itemPatent resources from the patents navigation property.</span></span>|
|[<span data-ttu-id="732d9-114">创建 itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-114">Create itemPatent</span></span>](../api/profile-post-patents.md)|[<span data-ttu-id="732d9-115">itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-115">itemPatent</span></span>](../resources/itempatent.md)|<span data-ttu-id="732d9-116">创建新的 itemPatent 对象。</span><span class="sxs-lookup"><span data-stu-id="732d9-116">Create a new itemPatent object.</span></span>|
|[<span data-ttu-id="732d9-117">获取 itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-117">Get itemPatent</span></span>](../api/itempatent-get.md)|[<span data-ttu-id="732d9-118">itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-118">itemPatent</span></span>](../resources/itempatent.md)|<span data-ttu-id="732d9-119">读取 [itemPatent](../resources/itempatent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="732d9-119">Read the properties and relationships of an [itemPatent](../resources/itempatent.md) object.</span></span>|
|[<span data-ttu-id="732d9-120">更新 itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-120">Update itemPatent</span></span>](../api/itempatent-update.md)|[<span data-ttu-id="732d9-121">itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-121">itemPatent</span></span>](../resources/itempatent.md)|<span data-ttu-id="732d9-122">更新 [itemPatent](../resources/itempatent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="732d9-122">Update the properties of an [itemPatent](../resources/itempatent.md) object.</span></span>|
|[<span data-ttu-id="732d9-123">删除 itemPatent</span><span class="sxs-lookup"><span data-stu-id="732d9-123">Delete itemPatent</span></span>](../api/itempatent-delete.md)|<span data-ttu-id="732d9-124">无</span><span class="sxs-lookup"><span data-stu-id="732d9-124">None</span></span>|<span data-ttu-id="732d9-125">删除一个 [itemPatent](../resources/itempatent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="732d9-125">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="732d9-126">属性</span><span class="sxs-lookup"><span data-stu-id="732d9-126">Properties</span></span>
|<span data-ttu-id="732d9-127">属性</span><span class="sxs-lookup"><span data-stu-id="732d9-127">Property</span></span>|<span data-ttu-id="732d9-128">类型</span><span class="sxs-lookup"><span data-stu-id="732d9-128">Type</span></span>|<span data-ttu-id="732d9-129">说明</span><span class="sxs-lookup"><span data-stu-id="732d9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="732d9-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="732d9-130">allowedAudiences</span></span>|<span data-ttu-id="732d9-131">String</span><span class="sxs-lookup"><span data-stu-id="732d9-131">String</span></span>|<span data-ttu-id="732d9-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="732d9-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="732d9-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="732d9-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="732d9-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="732d9-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="732d9-135">createdBy</span></span>|[<span data-ttu-id="732d9-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="732d9-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="732d9-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="732d9-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="732d9-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="732d9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="732d9-139">createdDateTime</span></span>|<span data-ttu-id="732d9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732d9-140">DateTimeOffset</span></span>|<span data-ttu-id="732d9-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="732d9-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="732d9-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="732d9-143">description</span><span class="sxs-lookup"><span data-stu-id="732d9-143">description</span></span>|<span data-ttu-id="732d9-144">String</span><span class="sxs-lookup"><span data-stu-id="732d9-144">String</span></span>|<span data-ttu-id="732d9-145">专利或档案的 Descpription。</span><span class="sxs-lookup"><span data-stu-id="732d9-145">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="732d9-146">displayName</span><span class="sxs-lookup"><span data-stu-id="732d9-146">displayName</span></span>|<span data-ttu-id="732d9-147">String</span><span class="sxs-lookup"><span data-stu-id="732d9-147">String</span></span>|<span data-ttu-id="732d9-148">专利或档案的标题。</span><span class="sxs-lookup"><span data-stu-id="732d9-148">Title of the patent or filing.</span></span> |
|<span data-ttu-id="732d9-149">id</span><span class="sxs-lookup"><span data-stu-id="732d9-149">id</span></span>|<span data-ttu-id="732d9-150">String</span><span class="sxs-lookup"><span data-stu-id="732d9-150">String</span></span>|<span data-ttu-id="732d9-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="732d9-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="732d9-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="732d9-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="732d9-153">推导</span><span class="sxs-lookup"><span data-stu-id="732d9-153">inference</span></span>|[<span data-ttu-id="732d9-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="732d9-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="732d9-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="732d9-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="732d9-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="732d9-157">isPending</span><span class="sxs-lookup"><span data-stu-id="732d9-157">isPending</span></span>        |<span data-ttu-id="732d9-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="732d9-158">Boolean</span></span>     |<span data-ttu-id="732d9-159">指示专利处于待处理状态。</span><span class="sxs-lookup"><span data-stu-id="732d9-159">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="732d9-160">issuedDate</span><span class="sxs-lookup"><span data-stu-id="732d9-160">issuedDate</span></span>       |<span data-ttu-id="732d9-161">日期</span><span class="sxs-lookup"><span data-stu-id="732d9-161">Date</span></span>        |<span data-ttu-id="732d9-162">授予专利的日期。</span><span class="sxs-lookup"><span data-stu-id="732d9-162">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="732d9-163">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="732d9-163">issuingAuthority</span></span> |<span data-ttu-id="732d9-164">String</span><span class="sxs-lookup"><span data-stu-id="732d9-164">String</span></span>      |<span data-ttu-id="732d9-165">授予专利的证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="732d9-165">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="732d9-166">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="732d9-166">lastModifiedBy</span></span>|[<span data-ttu-id="732d9-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="732d9-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="732d9-168">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="732d9-168">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="732d9-169">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-169">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="732d9-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="732d9-170">lastModifiedDateTime</span></span>|<span data-ttu-id="732d9-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732d9-171">DateTimeOffset</span></span>|<span data-ttu-id="732d9-172">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="732d9-172">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="732d9-173">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-173">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="732d9-174">数字</span><span class="sxs-lookup"><span data-stu-id="732d9-174">number</span></span>           |<span data-ttu-id="732d9-175">String</span><span class="sxs-lookup"><span data-stu-id="732d9-175">String</span></span>      |<span data-ttu-id="732d9-176">专利号码。</span><span class="sxs-lookup"><span data-stu-id="732d9-176">The patent number.</span></span>                      |
|<span data-ttu-id="732d9-177">source</span><span class="sxs-lookup"><span data-stu-id="732d9-177">source</span></span>|[<span data-ttu-id="732d9-178">personDataSource</span><span class="sxs-lookup"><span data-stu-id="732d9-178">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="732d9-179">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="732d9-179">Where the values originated if synced from another service.</span></span> <span data-ttu-id="732d9-180">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="732d9-180">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="732d9-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="732d9-181">webUrl</span></span>           |<span data-ttu-id="732d9-182">String</span><span class="sxs-lookup"><span data-stu-id="732d9-182">String</span></span>      |<span data-ttu-id="732d9-183">引用专利或档案的 URL。</span><span class="sxs-lookup"><span data-stu-id="732d9-183">URL referencing the patent or filing.</span></span> |


## <a name="relationships"></a><span data-ttu-id="732d9-184">关系</span><span class="sxs-lookup"><span data-stu-id="732d9-184">Relationships</span></span>
<span data-ttu-id="732d9-185">无。</span><span class="sxs-lookup"><span data-stu-id="732d9-185">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="732d9-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="732d9-186">JSON representation</span></span>
<span data-ttu-id="732d9-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="732d9-187">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPatent",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemPatent",
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
  "isPending": "Boolean",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "number": "String",
  "webUrl": "String"
}
```
