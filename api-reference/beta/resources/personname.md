---
title: Contact.personname 资源类型
description: Contact.personname 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f1817e3d9868e47158453113f4781ebfc155f86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997940"
---
# <a name="personname-resource-type"></a><span data-ttu-id="f2620-103">Contact.personname 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2620-103">personName resource type</span></span>

<span data-ttu-id="f2620-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2620-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2620-105">代表用户提供的、与其在 [配置文件](../resources/profile.md)中关联的扩展名称信息。</span><span class="sxs-lookup"><span data-stu-id="f2620-105">Represents extended name information provided by the user or which they have associated within their [profile](../resources/profile.md).</span></span>

<span data-ttu-id="f2620-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f2620-107">方法</span><span class="sxs-lookup"><span data-stu-id="f2620-107">Methods</span></span>
|<span data-ttu-id="f2620-108">方法</span><span class="sxs-lookup"><span data-stu-id="f2620-108">Method</span></span>|<span data-ttu-id="f2620-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2620-109">Return type</span></span>|<span data-ttu-id="f2620-110">说明</span><span class="sxs-lookup"><span data-stu-id="f2620-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2620-111">列出名称</span><span class="sxs-lookup"><span data-stu-id="f2620-111">List names</span></span>](../api/profile-list-names.md)|<span data-ttu-id="f2620-112">[contact.personname](../resources/personname.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2620-112">[personName](../resources/personname.md) collection</span></span>|<span data-ttu-id="f2620-113">从 "名称" 导航属性中获取 Contact.personname 资源。</span><span class="sxs-lookup"><span data-stu-id="f2620-113">Get the personName resources from the names navigation property.</span></span>|
|[<span data-ttu-id="f2620-114">创建 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-114">Create personName</span></span>](../api/profile-post-names.md)|[<span data-ttu-id="f2620-115">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-115">personName</span></span>](../resources/personname.md)|<span data-ttu-id="f2620-116">从 "名称" 导航属性中创建一个新的 [contact.personname](../resources/personname.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2620-116">Create a new [personName](../resources/personname.md) object from the names navigation property.</span></span>|
|[<span data-ttu-id="f2620-117">获取 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-117">Get personName</span></span>](../api/personname-get.md)|[<span data-ttu-id="f2620-118">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-118">personName</span></span>](../resources/personname.md)|<span data-ttu-id="f2620-119">读取 [contact.personname](../resources/personname.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2620-119">Read the properties and relationships of a [personName](../resources/personname.md) object.</span></span>|
|[<span data-ttu-id="f2620-120">更新 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-120">Update personName</span></span>](../api/personname-update.md)|[<span data-ttu-id="f2620-121">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-121">personName</span></span>](../resources/personname.md)|<span data-ttu-id="f2620-122">更新 [contact.personname](../resources/personname.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2620-122">Update the properties of a [personName](../resources/personname.md) object.</span></span>|
|[<span data-ttu-id="f2620-123">删除 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="f2620-123">Delete personName</span></span>](../api/personname-delete.md)|<span data-ttu-id="f2620-124">无</span><span class="sxs-lookup"><span data-stu-id="f2620-124">None</span></span>|<span data-ttu-id="f2620-125">删除一个 [contact.personname](../resources/personname.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2620-125">Deletes a [personName](../resources/personname.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2620-126">属性</span><span class="sxs-lookup"><span data-stu-id="f2620-126">Properties</span></span>
|<span data-ttu-id="f2620-127">属性</span><span class="sxs-lookup"><span data-stu-id="f2620-127">Property</span></span>|<span data-ttu-id="f2620-128">类型</span><span class="sxs-lookup"><span data-stu-id="f2620-128">Type</span></span>|<span data-ttu-id="f2620-129">说明</span><span class="sxs-lookup"><span data-stu-id="f2620-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2620-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="f2620-130">allowedAudiences</span></span>|<span data-ttu-id="f2620-131">String</span><span class="sxs-lookup"><span data-stu-id="f2620-131">String</span></span>|<span data-ttu-id="f2620-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="f2620-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f2620-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f2620-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f2620-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f2620-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="f2620-135">createdBy</span></span>|[<span data-ttu-id="f2620-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="f2620-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="f2620-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="f2620-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="f2620-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f2620-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2620-139">createdDateTime</span></span>|<span data-ttu-id="f2620-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2620-140">DateTimeOffset</span></span>|<span data-ttu-id="f2620-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="f2620-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="f2620-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f2620-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f2620-143">displayName</span></span>|<span data-ttu-id="f2620-144">String</span><span class="sxs-lookup"><span data-stu-id="f2620-144">String</span></span>|<span data-ttu-id="f2620-145">根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="f2620-145">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="f2620-146">前</span><span class="sxs-lookup"><span data-stu-id="f2620-146">first</span></span>|<span data-ttu-id="f2620-147">String</span><span class="sxs-lookup"><span data-stu-id="f2620-147">String</span></span>|<span data-ttu-id="f2620-148">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="f2620-148">First name of the user.</span></span>|
|<span data-ttu-id="f2620-149">id</span><span class="sxs-lookup"><span data-stu-id="f2620-149">id</span></span>|<span data-ttu-id="f2620-150">String</span><span class="sxs-lookup"><span data-stu-id="f2620-150">String</span></span>|<span data-ttu-id="f2620-151">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="f2620-151">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="f2620-152">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="f2620-152">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="f2620-153">推导</span><span class="sxs-lookup"><span data-stu-id="f2620-153">inference</span></span>|[<span data-ttu-id="f2620-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="f2620-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f2620-155">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="f2620-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f2620-156">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f2620-157">initials</span><span class="sxs-lookup"><span data-stu-id="f2620-157">initials</span></span>|<span data-ttu-id="f2620-158">String</span><span class="sxs-lookup"><span data-stu-id="f2620-158">String</span></span>|<span data-ttu-id="f2620-159">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="f2620-159">Initials of the user.</span></span>|
|<span data-ttu-id="f2620-160">languageTag</span><span class="sxs-lookup"><span data-stu-id="f2620-160">languageTag</span></span>|<span data-ttu-id="f2620-161">String</span><span class="sxs-lookup"><span data-stu-id="f2620-161">String</span></span>|<span data-ttu-id="f2620-162">包含以下语言的名称： (en-us、无 NB、en-us) 以下 IETF BCP47 格式。</span><span class="sxs-lookup"><span data-stu-id="f2620-162">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="f2620-163">末</span><span class="sxs-lookup"><span data-stu-id="f2620-163">last</span></span>|<span data-ttu-id="f2620-164">String</span><span class="sxs-lookup"><span data-stu-id="f2620-164">String</span></span>|<span data-ttu-id="f2620-165">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="f2620-165">Last name of the user.</span></span>|
|<span data-ttu-id="f2620-166">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f2620-166">lastModifiedBy</span></span>|[<span data-ttu-id="f2620-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="f2620-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="f2620-168">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="f2620-168">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="f2620-169">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-169">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f2620-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2620-170">lastModifiedDateTime</span></span>|<span data-ttu-id="f2620-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2620-171">DateTimeOffset</span></span>|<span data-ttu-id="f2620-172">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="f2620-172">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="f2620-173">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-173">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f2620-174">maiden</span><span class="sxs-lookup"><span data-stu-id="f2620-174">maiden</span></span>|<span data-ttu-id="f2620-175">String</span><span class="sxs-lookup"><span data-stu-id="f2620-175">String</span></span>|<span data-ttu-id="f2620-176">Maiden 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="f2620-176">Maiden name of the user.</span></span> |
|<span data-ttu-id="f2620-177">中间</span><span class="sxs-lookup"><span data-stu-id="f2620-177">middle</span></span>|<span data-ttu-id="f2620-178">String</span><span class="sxs-lookup"><span data-stu-id="f2620-178">String</span></span>|<span data-ttu-id="f2620-179">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="f2620-179">Middle name of the user.</span></span>|
|<span data-ttu-id="f2620-180">昵称</span><span class="sxs-lookup"><span data-stu-id="f2620-180">nickname</span></span>|<span data-ttu-id="f2620-181">String</span><span class="sxs-lookup"><span data-stu-id="f2620-181">String</span></span>|<span data-ttu-id="f2620-182">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="f2620-182">Nickname of the user.</span></span>|
|<span data-ttu-id="f2620-183">拼音</span><span class="sxs-lookup"><span data-stu-id="f2620-183">pronunciation</span></span>|[<span data-ttu-id="f2620-184">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="f2620-184">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="f2620-185">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="f2620-185">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="f2620-186">source</span><span class="sxs-lookup"><span data-stu-id="f2620-186">source</span></span>|[<span data-ttu-id="f2620-187">personDataSource</span><span class="sxs-lookup"><span data-stu-id="f2620-187">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="f2620-188">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="f2620-188">Where the values originated if synced from another service.</span></span> <span data-ttu-id="f2620-189">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f2620-189">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f2620-190">后缀</span><span class="sxs-lookup"><span data-stu-id="f2620-190">suffix</span></span>|<span data-ttu-id="f2620-191">String</span><span class="sxs-lookup"><span data-stu-id="f2620-191">String</span></span>|<span data-ttu-id="f2620-192">用户名称之后使用的指示符 (例如：博士. ) </span><span class="sxs-lookup"><span data-stu-id="f2620-192">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="f2620-193">title</span><span class="sxs-lookup"><span data-stu-id="f2620-193">title</span></span>|<span data-ttu-id="f2620-194">String</span><span class="sxs-lookup"><span data-stu-id="f2620-194">String</span></span>|<span data-ttu-id="f2620-195">Honorifics 用于为用户名称加上前缀 (例如： Dr.、罗德、Madam、Mrs ) </span><span class="sxs-lookup"><span data-stu-id="f2620-195">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2620-196">关系</span><span class="sxs-lookup"><span data-stu-id="f2620-196">Relationships</span></span>
<span data-ttu-id="f2620-197">无。</span><span class="sxs-lookup"><span data-stu-id="f2620-197">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2620-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2620-198">JSON representation</span></span>
<span data-ttu-id="f2620-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2620-199">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personName",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personName",
  "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
  "allowedAudiences": "organization",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

