---
title: userAccountInformation 资源类型
description: userAccountInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a633b6de9269b67fcf26dea035438a3494c4515c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812742"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="b4cf4-103">userAccountInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4cf4-103">userAccountInformation resource type</span></span>

<span data-ttu-id="b4cf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4cf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4cf4-105">代表特定绑定到用户帐户的信息，无论是作为 Azure AD 帐户还是 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="b4cf4-106">实体标识符分别设置为相应的 Azure AD guid 或 Microsoft 帐户 CID。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="b4cf4-107">这些字段在 Microsoft Graph 中是只读的，并且必须通过用户配置文件或租户管理员在相应的体验上进行编辑。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="b4cf4-108">继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b4cf4-109">方法</span><span class="sxs-lookup"><span data-stu-id="b4cf4-109">Methods</span></span>

|<span data-ttu-id="b4cf4-110">方法</span><span class="sxs-lookup"><span data-stu-id="b4cf4-110">Method</span></span>|<span data-ttu-id="b4cf4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b4cf4-111">Return type</span></span>|<span data-ttu-id="b4cf4-112">说明</span><span class="sxs-lookup"><span data-stu-id="b4cf4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b4cf4-113">列表帐户</span><span class="sxs-lookup"><span data-stu-id="b4cf4-113">List accounts</span></span>](../api/profile-list-accounts.md)|<span data-ttu-id="b4cf4-114">[userAccountInformation](../resources/useraccountinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4cf4-114">[userAccountInformation](../resources/useraccountinformation.md) collection</span></span>|<span data-ttu-id="b4cf4-115">从帐户导航属性中获取 userAccountInformation 资源。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-115">Get the userAccountInformation resources from the account navigation property.</span></span>|
|[<span data-ttu-id="b4cf4-116">创建 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-116">Create userAccountInformation</span></span>](../api/profile-post-accounts.md)|[<span data-ttu-id="b4cf4-117">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-117">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="b4cf4-118">创建新的 userAccountInformation 对象。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-118">Create a new userAccountInformation object.</span></span>|
|[<span data-ttu-id="b4cf4-119">获取 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-119">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md)|[<span data-ttu-id="b4cf4-120">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-120">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="b4cf4-121">读取 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-121">Read the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="b4cf4-122">更新 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-122">Update userAccountInformation</span></span>](../api/useraccountinformation-update.md)|[<span data-ttu-id="b4cf4-123">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-123">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="b4cf4-124">更新 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-124">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="b4cf4-125">删除 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="b4cf4-125">Delete userAccountInformation</span></span>](../api/useraccountinformation-delete.md)|<span data-ttu-id="b4cf4-126">无</span><span class="sxs-lookup"><span data-stu-id="b4cf4-126">None</span></span>|<span data-ttu-id="b4cf4-127">删除一个 [userAccountInformation](../resources/useraccountinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-127">Deletes a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b4cf4-128">属性</span><span class="sxs-lookup"><span data-stu-id="b4cf4-128">Properties</span></span>

|<span data-ttu-id="b4cf4-129">属性</span><span class="sxs-lookup"><span data-stu-id="b4cf4-129">Property</span></span>|<span data-ttu-id="b4cf4-130">类型</span><span class="sxs-lookup"><span data-stu-id="b4cf4-130">Type</span></span>|<span data-ttu-id="b4cf4-131">说明</span><span class="sxs-lookup"><span data-stu-id="b4cf4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4cf4-132">ageGroup</span><span class="sxs-lookup"><span data-stu-id="b4cf4-132">ageGroup</span></span>|<span data-ttu-id="b4cf4-133">String</span><span class="sxs-lookup"><span data-stu-id="b4cf4-133">String</span></span>|<span data-ttu-id="b4cf4-134">显示用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-134">Shows the age group of user.</span></span> <span data-ttu-id="b4cf4-135">允许的 `null` 值 `minor` 、 `notAdult` 和 `adult` 由目录生成且不能更改。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-135">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="b4cf4-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="b4cf4-136">allowedAudiences</span></span>|<span data-ttu-id="b4cf4-137">String</span><span class="sxs-lookup"><span data-stu-id="b4cf4-137">String</span></span>|<span data-ttu-id="b4cf4-138">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b4cf4-139">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b4cf4-140">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b4cf4-141">countryCode</span><span class="sxs-lookup"><span data-stu-id="b4cf4-141">countryCode</span></span>|<span data-ttu-id="b4cf4-142">String</span><span class="sxs-lookup"><span data-stu-id="b4cf4-142">String</span></span>|<span data-ttu-id="b4cf4-143">包含与用户帐户关联的双字符国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-143">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="b4cf4-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="b4cf4-144">createdBy</span></span>|[<span data-ttu-id="b4cf4-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="b4cf4-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="b4cf4-146">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-146">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="b4cf4-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b4cf4-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4cf4-148">createdDateTime</span></span>|<span data-ttu-id="b4cf4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4cf4-149">DateTimeOffset</span></span>|<span data-ttu-id="b4cf4-150">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-150">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="b4cf4-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b4cf4-152">id</span><span class="sxs-lookup"><span data-stu-id="b4cf4-152">id</span></span>|<span data-ttu-id="b4cf4-153">String</span><span class="sxs-lookup"><span data-stu-id="b4cf4-153">String</span></span>|<span data-ttu-id="b4cf4-154">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="b4cf4-155">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="b4cf4-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="b4cf4-156">推导</span><span class="sxs-lookup"><span data-stu-id="b4cf4-156">inference</span></span>|[<span data-ttu-id="b4cf4-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="b4cf4-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b4cf4-158">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b4cf4-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b4cf4-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b4cf4-160">lastModifiedBy</span></span>|[<span data-ttu-id="b4cf4-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="b4cf4-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="b4cf4-162">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="b4cf4-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b4cf4-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4cf4-164">lastModifiedDateTime</span></span>|<span data-ttu-id="b4cf4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4cf4-165">DateTimeOffset</span></span>|<span data-ttu-id="b4cf4-166">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="b4cf4-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b4cf4-168">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="b4cf4-168">preferredLanguageTag</span></span>|[<span data-ttu-id="b4cf4-169">localeInfo</span><span class="sxs-lookup"><span data-stu-id="b4cf4-169">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="b4cf4-170">包含用户与帐户相关的首选语言。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-170">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="b4cf4-171">source</span><span class="sxs-lookup"><span data-stu-id="b4cf4-171">source</span></span>|[<span data-ttu-id="b4cf4-172">personDataSource</span><span class="sxs-lookup"><span data-stu-id="b4cf4-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="b4cf4-173">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="b4cf4-174">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b4cf4-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b4cf4-175">userPrincipalName</span></span>|<span data-ttu-id="b4cf4-176">String</span><span class="sxs-lookup"><span data-stu-id="b4cf4-176">String</span></span>|<span data-ttu-id="b4cf4-177">与帐户关联的用户的用户主体名称 (UPN) 。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-177">The user principal name (UPN) of the user associated with the account.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="b4cf4-178">关系</span><span class="sxs-lookup"><span data-stu-id="b4cf4-178">Relationships</span></span>
<span data-ttu-id="b4cf4-179">无。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4cf4-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4cf4-180">JSON representation</span></span>
<span data-ttu-id="b4cf4-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4cf4-181">The following is a JSON representation of the resource.</span></span>
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
