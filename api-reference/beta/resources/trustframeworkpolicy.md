---
title: trustFrameworkPolicy
description: 在 Azure AD B2C 信任框架策略中称为 "自定义策略"。 这描述了适用于租户的 trustFrameworkPolicy 对象的操作。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2cda564b353675d54305db5c0e6eaaa64682a7ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519636"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="ff245-104">trustFrameworkPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff245-104">trustFrameworkPolicy resource type</span></span>

<span data-ttu-id="ff245-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff245-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff245-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff245-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff245-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff245-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff245-108">表示[Azure Active DIRECTORY B2C](/azure/active-directory-b2c/active-directory-b2c-overview)中的[信任框架](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)策略（也称为[自定义策略](/azure/active-directory-b2c/active-directory-b2c-overview-custom)）。</span><span class="sxs-lookup"><span data-stu-id="ff245-108">Represents a [Trust Framework](/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="ff245-109">信任框架策略提供了对用户旅程的完全控制权限。</span><span class="sxs-lookup"><span data-stu-id="ff245-109">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="ff245-110">使用它可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ff245-110">Use it to:</span></span>

* <span data-ttu-id="ff245-111">完全自定义注册和登录体验。</span><span class="sxs-lookup"><span data-stu-id="ff245-111">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="ff245-112">联合任何 SAML、Open ID Connect 或 OAuth2 identity provider。</span><span class="sxs-lookup"><span data-stu-id="ff245-112">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="ff245-113">通过调用 REST 终结点与其他系统或用户数据存储集成。</span><span class="sxs-lookup"><span data-stu-id="ff245-113">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="ff245-114">转换声明并自定义颁发给信赖方应用程序的令牌。</span><span class="sxs-lookup"><span data-stu-id="ff245-114">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="ff245-115">有关详细信息，请参阅[Azure Active DIRECTORY B2C 中的自定义策略](/azure/active-directory-b2c/active-directory-b2c-overview-custom)。</span><span class="sxs-lookup"><span data-stu-id="ff245-115">For more information, see [Custom policies in Azure Active Directory B2C](/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="ff245-116">方法</span><span class="sxs-lookup"><span data-stu-id="ff245-116">Methods</span></span>

| <span data-ttu-id="ff245-117">方法</span><span class="sxs-lookup"><span data-stu-id="ff245-117">Method</span></span>       | <span data-ttu-id="ff245-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff245-118">Return Type</span></span>  |<span data-ttu-id="ff245-119">说明</span><span class="sxs-lookup"><span data-stu-id="ff245-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff245-120">创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-120">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="ff245-121">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-121">trustFrameworkPolicy</span></span>|<span data-ttu-id="ff245-122">创建新的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="ff245-122">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="ff245-123">获取 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-123">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="ff245-124">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-124">trustFrameworkPolicy</span></span>|<span data-ttu-id="ff245-125">读取现有 trustFrameworkPolicy 的属性。</span><span class="sxs-lookup"><span data-stu-id="ff245-125">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="ff245-126">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="ff245-126">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="ff245-127">trustFrameworkPolicy 集合</span><span class="sxs-lookup"><span data-stu-id="ff245-127">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="ff245-128">列出租户中配置的所有 trustFrameworkPolicies。</span><span class="sxs-lookup"><span data-stu-id="ff245-128">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="ff245-129">更新或创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-129">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="ff245-130">无</span><span class="sxs-lookup"><span data-stu-id="ff245-130">None</span></span>|<span data-ttu-id="ff245-131">更新现有的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="ff245-131">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="ff245-132">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-132">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="ff245-133">无</span><span class="sxs-lookup"><span data-stu-id="ff245-133">None</span></span>|<span data-ttu-id="ff245-134">删除现有的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="ff245-134">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff245-135">属性</span><span class="sxs-lookup"><span data-stu-id="ff245-135">Properties</span></span>

|<span data-ttu-id="ff245-136">属性</span><span class="sxs-lookup"><span data-stu-id="ff245-136">Property</span></span>|<span data-ttu-id="ff245-137">类型</span><span class="sxs-lookup"><span data-stu-id="ff245-137">Type</span></span>|<span data-ttu-id="ff245-138">说明</span><span class="sxs-lookup"><span data-stu-id="ff245-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff245-139">id</span><span class="sxs-lookup"><span data-stu-id="ff245-139">id</span></span>|<span data-ttu-id="ff245-140">String</span><span class="sxs-lookup"><span data-stu-id="ff245-140">String</span></span>|<span data-ttu-id="ff245-141">策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="ff245-141">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff245-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff245-142">JSON representation</span></span>

<span data-ttu-id="ff245-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff245-143">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ff245-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ff245-144">See also</span></span>

- <span data-ttu-id="ff245-145">[trustFrameworkPolicy 架构](/azure/active-directory-b2c/trustframeworkpolicy)，以了解有关架构元素的信息。</span><span class="sxs-lookup"><span data-stu-id="ff245-145">[trustFrameworkPolicy schema](/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>
- [<span data-ttu-id="ff245-146">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="ff245-146">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
