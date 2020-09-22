---
title: userAccountInformation 资源类型
description: userAccountInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9bcd0553c51d75724f28737321f463bcab034306
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057911"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="a6b59-103">userAccountInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6b59-103">userAccountInformation resource type</span></span>

<span data-ttu-id="a6b59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6b59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b59-105">代表特定绑定到用户帐户的信息，无论是作为 Azure AD 帐户还是 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="a6b59-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="a6b59-106">实体标识符分别设置为相应的 Azure AD guid 或 Microsoft 帐户 CID。</span><span class="sxs-lookup"><span data-stu-id="a6b59-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="a6b59-107">这些字段在 Microsoft Graph 中是只读的，并且必须通过用户配置文件或租户管理员在相应的体验上进行编辑。</span><span class="sxs-lookup"><span data-stu-id="a6b59-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="a6b59-108">继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a6b59-109">方法</span><span class="sxs-lookup"><span data-stu-id="a6b59-109">Methods</span></span>

|<span data-ttu-id="a6b59-110">方法</span><span class="sxs-lookup"><span data-stu-id="a6b59-110">Method</span></span>|<span data-ttu-id="a6b59-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6b59-111">Return type</span></span>|<span data-ttu-id="a6b59-112">说明</span><span class="sxs-lookup"><span data-stu-id="a6b59-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6b59-113">列表帐户</span><span class="sxs-lookup"><span data-stu-id="a6b59-113">List accounts</span></span>](../api/profile-list-accounts.md)|<span data-ttu-id="a6b59-114">[userAccountInformation](../resources/useraccountinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b59-114">[userAccountInformation](../resources/useraccountinformation.md) collection</span></span>|<span data-ttu-id="a6b59-115">从帐户导航属性中获取 userAccountInformation 资源。</span><span class="sxs-lookup"><span data-stu-id="a6b59-115">Get the userAccountInformation resources from the account navigation property.</span></span>|
|[<span data-ttu-id="a6b59-116">创建 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-116">Create userAccountInformation</span></span>](../api/profile-post-accounts.md)|[<span data-ttu-id="a6b59-117">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-117">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="a6b59-118">创建新的 userAccountInformation 对象。</span><span class="sxs-lookup"><span data-stu-id="a6b59-118">Create a new userAccountInformation object.</span></span>|
|[<span data-ttu-id="a6b59-119">获取 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-119">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md)|[<span data-ttu-id="a6b59-120">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-120">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="a6b59-121">读取 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6b59-121">Read the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="a6b59-122">更新 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-122">Update userAccountInformation</span></span>](../api/useraccountinformation-update.md)|[<span data-ttu-id="a6b59-123">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-123">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="a6b59-124">更新 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6b59-124">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="a6b59-125">删除 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="a6b59-125">Delete userAccountInformation</span></span>](../api/useraccountinformation-delete.md)|<span data-ttu-id="a6b59-126">无</span><span class="sxs-lookup"><span data-stu-id="a6b59-126">None</span></span>|<span data-ttu-id="a6b59-127">删除一个 [userAccountInformation](../resources/useraccountinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6b59-127">Deletes a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6b59-128">属性</span><span class="sxs-lookup"><span data-stu-id="a6b59-128">Properties</span></span>

|<span data-ttu-id="a6b59-129">属性</span><span class="sxs-lookup"><span data-stu-id="a6b59-129">Property</span></span>|<span data-ttu-id="a6b59-130">类型</span><span class="sxs-lookup"><span data-stu-id="a6b59-130">Type</span></span>|<span data-ttu-id="a6b59-131">说明</span><span class="sxs-lookup"><span data-stu-id="a6b59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b59-132">ageGroup</span><span class="sxs-lookup"><span data-stu-id="a6b59-132">ageGroup</span></span>|<span data-ttu-id="a6b59-133">String</span><span class="sxs-lookup"><span data-stu-id="a6b59-133">String</span></span>|<span data-ttu-id="a6b59-134">显示用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="a6b59-134">Shows the age group of user.</span></span> <span data-ttu-id="a6b59-135">允许的 `null` 值 `minor` 、 `notAdult` 和 `adult` 由目录生成且不能更改。</span><span class="sxs-lookup"><span data-stu-id="a6b59-135">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="a6b59-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a6b59-136">allowedAudiences</span></span>|<span data-ttu-id="a6b59-137">String</span><span class="sxs-lookup"><span data-stu-id="a6b59-137">String</span></span>|<span data-ttu-id="a6b59-138">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="a6b59-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a6b59-139">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a6b59-140">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a6b59-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a6b59-141">countryCode</span><span class="sxs-lookup"><span data-stu-id="a6b59-141">countryCode</span></span>|<span data-ttu-id="a6b59-142">String</span><span class="sxs-lookup"><span data-stu-id="a6b59-142">String</span></span>|<span data-ttu-id="a6b59-143">包含与用户帐户关联的双字符国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="a6b59-143">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="a6b59-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="a6b59-144">createdBy</span></span>|[<span data-ttu-id="a6b59-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="a6b59-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a6b59-146">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b59-146">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="a6b59-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6b59-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6b59-148">createdDateTime</span></span>|<span data-ttu-id="a6b59-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6b59-149">DateTimeOffset</span></span>|<span data-ttu-id="a6b59-150">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a6b59-150">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="a6b59-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6b59-152">id</span><span class="sxs-lookup"><span data-stu-id="a6b59-152">id</span></span>|<span data-ttu-id="a6b59-153">String</span><span class="sxs-lookup"><span data-stu-id="a6b59-153">String</span></span>|<span data-ttu-id="a6b59-154">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b59-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="a6b59-155">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="a6b59-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="a6b59-156">推导</span><span class="sxs-lookup"><span data-stu-id="a6b59-156">inference</span></span>|[<span data-ttu-id="a6b59-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a6b59-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a6b59-158">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="a6b59-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a6b59-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6b59-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a6b59-160">lastModifiedBy</span></span>|[<span data-ttu-id="a6b59-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="a6b59-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a6b59-162">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b59-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="a6b59-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6b59-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6b59-164">lastModifiedDateTime</span></span>|<span data-ttu-id="a6b59-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6b59-165">DateTimeOffset</span></span>|<span data-ttu-id="a6b59-166">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a6b59-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="a6b59-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6b59-168">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="a6b59-168">preferredLanguageTag</span></span>|[<span data-ttu-id="a6b59-169">localeInfo</span><span class="sxs-lookup"><span data-stu-id="a6b59-169">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="a6b59-170">包含用户与帐户相关的首选语言。</span><span class="sxs-lookup"><span data-stu-id="a6b59-170">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="a6b59-171">source</span><span class="sxs-lookup"><span data-stu-id="a6b59-171">source</span></span>|[<span data-ttu-id="a6b59-172">personDataSource</span><span class="sxs-lookup"><span data-stu-id="a6b59-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="a6b59-173">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="a6b59-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="a6b59-174">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6b59-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6b59-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a6b59-175">userPrincipalName</span></span>|<span data-ttu-id="a6b59-176">String</span><span class="sxs-lookup"><span data-stu-id="a6b59-176">String</span></span>|<span data-ttu-id="a6b59-177">与帐户关联的用户的用户主体名称 (UPN) 。</span><span class="sxs-lookup"><span data-stu-id="a6b59-177">The user principal name (UPN) of the user associated with the account.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="a6b59-178">关系</span><span class="sxs-lookup"><span data-stu-id="a6b59-178">Relationships</span></span>
<span data-ttu-id="a6b59-179">无。</span><span class="sxs-lookup"><span data-stu-id="a6b59-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6b59-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6b59-180">JSON representation</span></span>
<span data-ttu-id="a6b59-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b59-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
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
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```


