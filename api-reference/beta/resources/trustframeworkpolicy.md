---
title: trustFrameworkPolicy
description: 在 Azure AD B2C 信任框架策略中称为 "自定义策略"。 这描述了适用于租户的 trustFrameworkPolicy 对象的操作。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bad5d8cfa6d9b53c4023bb89eabd74436ab7dacd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057946"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="b2799-104">trustFrameworkPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2799-104">trustFrameworkPolicy resource type</span></span>

<span data-ttu-id="b2799-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2799-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2799-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b2799-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2799-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b2799-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2799-108">表示[信任框架](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)策略 (也称为[AZURE Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview)中) [自定义策略](/azure/active-directory-b2c/active-directory-b2c-overview-custom)。</span><span class="sxs-lookup"><span data-stu-id="b2799-108">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="b2799-109">信任框架策略提供了对用户旅程的完全控制权限。</span><span class="sxs-lookup"><span data-stu-id="b2799-109">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="b2799-110">使用它可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b2799-110">Use it to:</span></span>

* <span data-ttu-id="b2799-111">完全自定义注册和登录体验。</span><span class="sxs-lookup"><span data-stu-id="b2799-111">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="b2799-112">联合任何 SAML、Open ID Connect 或 OAuth2 identity provider。</span><span class="sxs-lookup"><span data-stu-id="b2799-112">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="b2799-113">通过调用 REST 终结点与其他系统或用户数据存储集成。</span><span class="sxs-lookup"><span data-stu-id="b2799-113">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="b2799-114">转换声明并自定义颁发给信赖方应用程序的令牌。</span><span class="sxs-lookup"><span data-stu-id="b2799-114">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="b2799-115">有关详细信息，请参阅 [Azure Active DIRECTORY B2C 中的自定义策略](/azure/active-directory-b2c/active-directory-b2c-overview-custom)。</span><span class="sxs-lookup"><span data-stu-id="b2799-115">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="b2799-116">方法</span><span class="sxs-lookup"><span data-stu-id="b2799-116">Methods</span></span>

| <span data-ttu-id="b2799-117">方法</span><span class="sxs-lookup"><span data-stu-id="b2799-117">Method</span></span>       | <span data-ttu-id="b2799-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="b2799-118">Return Type</span></span>  |<span data-ttu-id="b2799-119">说明</span><span class="sxs-lookup"><span data-stu-id="b2799-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2799-120">创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-120">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="b2799-121">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-121">trustFrameworkPolicy</span></span>|<span data-ttu-id="b2799-122">创建新的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="b2799-122">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="b2799-123">获取 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-123">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="b2799-124">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-124">trustFrameworkPolicy</span></span>|<span data-ttu-id="b2799-125">读取现有 trustFrameworkPolicy 的属性。</span><span class="sxs-lookup"><span data-stu-id="b2799-125">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="b2799-126">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="b2799-126">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="b2799-127">trustFrameworkPolicy 集合</span><span class="sxs-lookup"><span data-stu-id="b2799-127">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="b2799-128">列出租户中配置的所有 trustFrameworkPolicies。</span><span class="sxs-lookup"><span data-stu-id="b2799-128">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="b2799-129">更新或创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-129">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="b2799-130">无</span><span class="sxs-lookup"><span data-stu-id="b2799-130">None</span></span>|<span data-ttu-id="b2799-131">更新现有的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="b2799-131">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="b2799-132">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-132">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="b2799-133">无</span><span class="sxs-lookup"><span data-stu-id="b2799-133">None</span></span>|<span data-ttu-id="b2799-134">删除现有的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="b2799-134">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2799-135">属性</span><span class="sxs-lookup"><span data-stu-id="b2799-135">Properties</span></span>

|<span data-ttu-id="b2799-136">属性</span><span class="sxs-lookup"><span data-stu-id="b2799-136">Property</span></span>|<span data-ttu-id="b2799-137">类型</span><span class="sxs-lookup"><span data-stu-id="b2799-137">Type</span></span>|<span data-ttu-id="b2799-138">说明</span><span class="sxs-lookup"><span data-stu-id="b2799-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2799-139">id</span><span class="sxs-lookup"><span data-stu-id="b2799-139">id</span></span>|<span data-ttu-id="b2799-140">String</span><span class="sxs-lookup"><span data-stu-id="b2799-140">String</span></span>|<span data-ttu-id="b2799-141">策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2799-141">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2799-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2799-142">JSON representation</span></span>

<span data-ttu-id="b2799-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2799-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a><span data-ttu-id="b2799-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b2799-144">See also</span></span>

- <span data-ttu-id="b2799-145">[trustFrameworkPolicy 架构](/azure/active-directory-b2c/trustframeworkpolicy) ，以了解有关架构元素的信息。</span><span class="sxs-lookup"><span data-stu-id="b2799-145">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="b2799-146">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="b2799-146">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)


