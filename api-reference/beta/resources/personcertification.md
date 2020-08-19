---
title: personCertification 资源类型
description: personCertification 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef4ebe3bc870bafd0edf6a5315589c8f823286df
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812925"
---
# <a name="personcertification-resource-type"></a><span data-ttu-id="bd7ae-103">personCertification 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd7ae-103">personCertification resource type</span></span>

<span data-ttu-id="bd7ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd7ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd7ae-105">表示已与用户的 [配置文件](../resources/profile.md)关联的证书或称号。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-105">Represents a certification or designation which has been associated with a user's [profile](../resources/profile.md).</span></span>

<span data-ttu-id="bd7ae-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bd7ae-107">方法</span><span class="sxs-lookup"><span data-stu-id="bd7ae-107">Methods</span></span>
|<span data-ttu-id="bd7ae-108">方法</span><span class="sxs-lookup"><span data-stu-id="bd7ae-108">Method</span></span>|<span data-ttu-id="bd7ae-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bd7ae-109">Return type</span></span>|<span data-ttu-id="bd7ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd7ae-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bd7ae-111">列出证书</span><span class="sxs-lookup"><span data-stu-id="bd7ae-111">List certifications</span></span>](../api/profile-list-certifications.md)|<span data-ttu-id="bd7ae-112">[personCertification](../resources/personcertification.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bd7ae-112">[personCertification](../resources/personcertification.md) collection</span></span>|<span data-ttu-id="bd7ae-113">从认证导航属性中获取 personCertification 资源。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-113">Get the personCertification resources from the certifications navigation property.</span></span>|
|[<span data-ttu-id="bd7ae-114">创建 personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-114">Create personCertification</span></span>](../api/profile-post-certifications.md)|[<span data-ttu-id="bd7ae-115">personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-115">personCertification</span></span>](../resources/personcertification.md)|<span data-ttu-id="bd7ae-116">创建新的 personCertification 对象。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-116">Create a new personCertification object.</span></span>|
|[<span data-ttu-id="bd7ae-117">获取 personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-117">Get personCertification</span></span>](../api/personCertification-get.md)|[<span data-ttu-id="bd7ae-118">personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-118">personCertification</span></span>](../resources/personcertification.md)|<span data-ttu-id="bd7ae-119">读取 [personCertification](../resources/personcertification.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-119">Read the properties and relationships of an [personCertification](../resources/personcertification.md) object.</span></span>|
|[<span data-ttu-id="bd7ae-120">更新 personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-120">Update personCertification</span></span>](../api/personCertification-update.md)|[<span data-ttu-id="bd7ae-121">personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-121">personCertification</span></span>](../resources/personcertification.md)|<span data-ttu-id="bd7ae-122">更新 [personCertification](../resources/personcertification.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-122">Update the properties of an [personCertification](../resources/personcertification.md) object.</span></span>|
|[<span data-ttu-id="bd7ae-123">删除 personCertification</span><span class="sxs-lookup"><span data-stu-id="bd7ae-123">Delete personCertification</span></span>](../api/personCertification-delete.md)|<span data-ttu-id="bd7ae-124">无</span><span class="sxs-lookup"><span data-stu-id="bd7ae-124">None</span></span>|<span data-ttu-id="bd7ae-125">删除一个 [personCertification](../resources/personcertification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-125">Deletes an [personCertification](../resources/personcertification.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd7ae-126">属性</span><span class="sxs-lookup"><span data-stu-id="bd7ae-126">Properties</span></span>
|<span data-ttu-id="bd7ae-127">属性</span><span class="sxs-lookup"><span data-stu-id="bd7ae-127">Property</span></span>|<span data-ttu-id="bd7ae-128">类型</span><span class="sxs-lookup"><span data-stu-id="bd7ae-128">Type</span></span>|<span data-ttu-id="bd7ae-129">说明</span><span class="sxs-lookup"><span data-stu-id="bd7ae-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd7ae-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="bd7ae-130">allowedAudiences</span></span>|<span data-ttu-id="bd7ae-131">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-131">String</span></span>|<span data-ttu-id="bd7ae-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="bd7ae-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="bd7ae-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bd7ae-135">certificationId</span><span class="sxs-lookup"><span data-stu-id="bd7ae-135">certificationId</span></span>  |<span data-ttu-id="bd7ae-136">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-136">String</span></span>      |<span data-ttu-id="bd7ae-137">证书的 referenceable 标识符。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-137">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="bd7ae-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="bd7ae-138">createdBy</span></span>|[<span data-ttu-id="bd7ae-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="bd7ae-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="bd7ae-140">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="bd7ae-141">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bd7ae-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7ae-142">createdDateTime</span></span>|<span data-ttu-id="bd7ae-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7ae-143">DateTimeOffset</span></span>|<span data-ttu-id="bd7ae-144">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="bd7ae-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bd7ae-146">description</span><span class="sxs-lookup"><span data-stu-id="bd7ae-146">description</span></span>      |<span data-ttu-id="bd7ae-147">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-147">String</span></span>      |<span data-ttu-id="bd7ae-148">证书的说明。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-148">Description of the certification.</span></span>                   |
|<span data-ttu-id="bd7ae-149">displayName</span><span class="sxs-lookup"><span data-stu-id="bd7ae-149">displayName</span></span>      |<span data-ttu-id="bd7ae-150">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-150">String</span></span>      |<span data-ttu-id="bd7ae-151">证书的标题。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-151">Title of the certification.</span></span>                         |
|<span data-ttu-id="bd7ae-152">endDate</span><span class="sxs-lookup"><span data-stu-id="bd7ae-152">endDate</span></span>          |<span data-ttu-id="bd7ae-153">日期</span><span class="sxs-lookup"><span data-stu-id="bd7ae-153">Date</span></span>        |<span data-ttu-id="bd7ae-154">证书到期的日期。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-154">The date that the certification expires.</span></span>            |
|<span data-ttu-id="bd7ae-155">id</span><span class="sxs-lookup"><span data-stu-id="bd7ae-155">id</span></span>|<span data-ttu-id="bd7ae-156">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-156">String</span></span>|<span data-ttu-id="bd7ae-157">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-157">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="bd7ae-158">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="bd7ae-158">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="bd7ae-159">推导</span><span class="sxs-lookup"><span data-stu-id="bd7ae-159">inference</span></span>|[<span data-ttu-id="bd7ae-160">inferenceData</span><span class="sxs-lookup"><span data-stu-id="bd7ae-160">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="bd7ae-161">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-161">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="bd7ae-162">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-162">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bd7ae-163">issuedDate</span><span class="sxs-lookup"><span data-stu-id="bd7ae-163">issuedDate</span></span>       |<span data-ttu-id="bd7ae-164">日期</span><span class="sxs-lookup"><span data-stu-id="bd7ae-164">Date</span></span>        |<span data-ttu-id="bd7ae-165">颁发证书的日期。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-165">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="bd7ae-166">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="bd7ae-166">issuingAuthority</span></span> |<span data-ttu-id="bd7ae-167">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-167">String</span></span>      |<span data-ttu-id="bd7ae-168">授予证书颁发机构的权限。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-168">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="bd7ae-169">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="bd7ae-169">issuingCompany</span></span>   |<span data-ttu-id="bd7ae-170">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-170">String</span></span>      |<span data-ttu-id="bd7ae-171">授予证书的公司。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-171">Company which granted the certification.</span></span>          |
|<span data-ttu-id="bd7ae-172">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bd7ae-172">lastModifiedBy</span></span>|[<span data-ttu-id="bd7ae-173">identitySet</span><span class="sxs-lookup"><span data-stu-id="bd7ae-173">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="bd7ae-174">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-174">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="bd7ae-175">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-175">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bd7ae-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7ae-176">lastModifiedDateTime</span></span>|<span data-ttu-id="bd7ae-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7ae-177">DateTimeOffset</span></span>|<span data-ttu-id="bd7ae-178">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-178">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="bd7ae-179">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-179">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bd7ae-180">source</span><span class="sxs-lookup"><span data-stu-id="bd7ae-180">source</span></span>|[<span data-ttu-id="bd7ae-181">personDataSource</span><span class="sxs-lookup"><span data-stu-id="bd7ae-181">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="bd7ae-182">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-182">Where the values originated if synced from another service.</span></span> <span data-ttu-id="bd7ae-183">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-183">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bd7ae-184">startDate</span><span class="sxs-lookup"><span data-stu-id="bd7ae-184">startDate</span></span>        |<span data-ttu-id="bd7ae-185">日期</span><span class="sxs-lookup"><span data-stu-id="bd7ae-185">Date</span></span>        |<span data-ttu-id="bd7ae-186">证书生效的日期。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-186">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="bd7ae-187">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="bd7ae-187">thumbnailUrl</span></span>     |<span data-ttu-id="bd7ae-188">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-188">String</span></span>      |<span data-ttu-id="bd7ae-189">URL 引用证书的缩略图。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-189">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="bd7ae-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="bd7ae-190">webUrl</span></span>           |<span data-ttu-id="bd7ae-191">String</span><span class="sxs-lookup"><span data-stu-id="bd7ae-191">String</span></span>      |<span data-ttu-id="bd7ae-192">引用证书的 URL。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-192">URL referencing the certification.</span></span>                  |

## <a name="relationships"></a><span data-ttu-id="bd7ae-193">关系</span><span class="sxs-lookup"><span data-stu-id="bd7ae-193">Relationships</span></span>
<span data-ttu-id="bd7ae-194">无。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-194">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd7ae-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd7ae-195">JSON representation</span></span>
<span data-ttu-id="bd7ae-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd7ae-196">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personCertification",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personCertification",
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
  "certificationId": "String",
  "description": "String",
  "displayName": "String",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "String",
  "issuingCompany": "String",
  "startDate": "Date",
  "thumbnailUrl": "String",
  "webUrl": "String"
}
```
