---
title: appleManagedIdentityProvider 资源类型
description: 在 Azure AD B2C 租户中表示 Apple 标识提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ee02900b6d41695d49d7c5ee38d834c676f69603
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491097"
---
# <a name="applemanagedidentityprovider-resource-type"></a><span data-ttu-id="7da32-103">appleManagedIdentityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="7da32-103">appleManagedIdentityProvider resource type</span></span>
<span data-ttu-id="7da32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7da32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7da32-105">可以将 Apple 配置为 Azure AD B2C 租户的社交标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="7da32-105">You can configure Apple as a social identity provider for an Azure AD B2C tenant.</span></span> <span data-ttu-id="7da32-106">根据 Apple 提供的信息，API 将生成客户端密码。</span><span class="sxs-lookup"><span data-stu-id="7da32-106">Based on the information Apple provides, the API will generate a client secret.</span></span> <span data-ttu-id="7da32-107">Apple 需要每六个月更新一次秘诀。</span><span class="sxs-lookup"><span data-stu-id="7da32-107">Apple needs the secret to be renewed every six months.</span></span> <span data-ttu-id="7da32-108">必须囘圼旋转編密編。</span><span class="sxs-lookup"><span data-stu-id="7da32-108">You will have to maunally rotate the secret.</span></span>

<span data-ttu-id="7da32-109">此类型将从 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="7da32-109">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7da32-110">方法</span><span class="sxs-lookup"><span data-stu-id="7da32-110">Methods</span></span>

| <span data-ttu-id="7da32-111">方法</span><span class="sxs-lookup"><span data-stu-id="7da32-111">Method</span></span>       | <span data-ttu-id="7da32-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="7da32-112">Return Type</span></span>  |<span data-ttu-id="7da32-113">Description</span><span class="sxs-lookup"><span data-stu-id="7da32-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7da32-114">List</span><span class="sxs-lookup"><span data-stu-id="7da32-114">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="7da32-115">identityProviderBase 集合</span><span class="sxs-lookup"><span data-stu-id="7da32-115">identityProviderBase collection</span></span>|<span data-ttu-id="7da32-116">检索租户中配置的所有标识提供程序，包括 Apple 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="7da32-116">Retrieve all identity providers configured in a tenant including the Apple identity providers.</span></span>|
|[<span data-ttu-id="7da32-117">Create</span><span class="sxs-lookup"><span data-stu-id="7da32-117">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="7da32-118">appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="7da32-118">appleManagedIdentityProvider</span></span> |<span data-ttu-id="7da32-119">创建新的 Apple 标识提供程序配置。</span><span class="sxs-lookup"><span data-stu-id="7da32-119">Create a new Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="7da32-120">Get</span><span class="sxs-lookup"><span data-stu-id="7da32-120">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="7da32-121">appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="7da32-121">appleManagedIdentityProvider</span></span> |<span data-ttu-id="7da32-122">检索 Apple 标识提供程序配置的属性。</span><span class="sxs-lookup"><span data-stu-id="7da32-122">Retrieve properties of the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="7da32-123">更新</span><span class="sxs-lookup"><span data-stu-id="7da32-123">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="7da32-124">无</span><span class="sxs-lookup"><span data-stu-id="7da32-124">None</span></span>|<span data-ttu-id="7da32-125">更新 Apple 标识提供程序配置。</span><span class="sxs-lookup"><span data-stu-id="7da32-125">Update the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="7da32-126">删除</span><span class="sxs-lookup"><span data-stu-id="7da32-126">Delete</span></span>](../api/identityproviderbase-delete.md)|<span data-ttu-id="7da32-127">无</span><span class="sxs-lookup"><span data-stu-id="7da32-127">None</span></span>|<span data-ttu-id="7da32-128">删除 Apple 标识提供程序配置。</span><span class="sxs-lookup"><span data-stu-id="7da32-128">Delete the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="7da32-129">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="7da32-129">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="7da32-130">String 集合</span><span class="sxs-lookup"><span data-stu-id="7da32-130">String collection</span></span>|<span data-ttu-id="7da32-131">检索租户中所有可用的标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="7da32-131">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="7da32-132">属性</span><span class="sxs-lookup"><span data-stu-id="7da32-132">Properties</span></span>

|<span data-ttu-id="7da32-133">属性</span><span class="sxs-lookup"><span data-stu-id="7da32-133">Property</span></span>|<span data-ttu-id="7da32-134">类型</span><span class="sxs-lookup"><span data-stu-id="7da32-134">Type</span></span>|<span data-ttu-id="7da32-135">说明</span><span class="sxs-lookup"><span data-stu-id="7da32-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7da32-136">developerId</span><span class="sxs-lookup"><span data-stu-id="7da32-136">developerId</span></span>|<span data-ttu-id="7da32-137">String</span><span class="sxs-lookup"><span data-stu-id="7da32-137">String</span></span>|<span data-ttu-id="7da32-138">Apple 开发人员标识符。</span><span class="sxs-lookup"><span data-stu-id="7da32-138">The Apple developer identifier.</span></span> <span data-ttu-id="7da32-139">必填。</span><span class="sxs-lookup"><span data-stu-id="7da32-139">Required.</span></span>|
|<span data-ttu-id="7da32-140">服务 Id</span><span class="sxs-lookup"><span data-stu-id="7da32-140">serviceId</span></span>|<span data-ttu-id="7da32-141">String</span><span class="sxs-lookup"><span data-stu-id="7da32-141">String</span></span>|<span data-ttu-id="7da32-142">Apple 服务标识符。</span><span class="sxs-lookup"><span data-stu-id="7da32-142">The Apple service identifier.</span></span> <span data-ttu-id="7da32-143">必填。</span><span class="sxs-lookup"><span data-stu-id="7da32-143">Required.</span></span>|
|<span data-ttu-id="7da32-144">keyId</span><span class="sxs-lookup"><span data-stu-id="7da32-144">keyId</span></span>|<span data-ttu-id="7da32-145">String</span><span class="sxs-lookup"><span data-stu-id="7da32-145">String</span></span>|<span data-ttu-id="7da32-146">Apple 密钥标识符。</span><span class="sxs-lookup"><span data-stu-id="7da32-146">The Apple key identifier.</span></span> <span data-ttu-id="7da32-147">必填。</span><span class="sxs-lookup"><span data-stu-id="7da32-147">Required.</span></span>|
|<span data-ttu-id="7da32-148">certificateData</span><span class="sxs-lookup"><span data-stu-id="7da32-148">certificateData</span></span>|<span data-ttu-id="7da32-149">String</span><span class="sxs-lookup"><span data-stu-id="7da32-149">String</span></span>|<span data-ttu-id="7da32-150">证书中长文本字符串的证书数据可能是 null。</span><span class="sxs-lookup"><span data-stu-id="7da32-150">The certificate data which is a long string of text from the certificate, can be null.</span></span>|
|<span data-ttu-id="7da32-151">id</span><span class="sxs-lookup"><span data-stu-id="7da32-151">id</span></span>|<span data-ttu-id="7da32-152">String</span><span class="sxs-lookup"><span data-stu-id="7da32-152">String</span></span>|<span data-ttu-id="7da32-153">标识提供程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="7da32-153">The identifier of the identity provider.</span></span> <span data-ttu-id="7da32-154">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="7da32-154">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="7da32-155">只读。</span><span class="sxs-lookup"><span data-stu-id="7da32-155">Read-only.</span></span>|
|<span data-ttu-id="7da32-156">displayName</span><span class="sxs-lookup"><span data-stu-id="7da32-156">displayName</span></span>|<span data-ttu-id="7da32-157">字符串</span><span class="sxs-lookup"><span data-stu-id="7da32-157">String</span></span>|<span data-ttu-id="7da32-158">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7da32-158">The display name of the identity provider.</span></span> <span data-ttu-id="7da32-159">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="7da32-159">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|

<span data-ttu-id="7da32-160">你可以从 Apple 开发人员门户找到 developerId、serviceId、keyId 和 certificateData。</span><span class="sxs-lookup"><span data-stu-id="7da32-160">You can find the developerId, serviceId, keyId and the certificateData from the Apple developer portal.</span></span> <span data-ttu-id="7da32-161">有关更多详细信息，你可以按照指南创建 [Apple ID 应用程序](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)</span><span class="sxs-lookup"><span data-stu-id="7da32-161">For nore details you can follow the guide to [create an Apple ID application](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)</span></span>

## <a name="json-representation"></a><span data-ttu-id="7da32-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7da32-162">JSON representation</span></span>

<span data-ttu-id="7da32-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7da32-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```json
{
    "id": "String",
    "displayName": "String",
    "developerId": "String",
    "serviceId": "String",
    "keyId": "String",
    "certificateData": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "appleIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
