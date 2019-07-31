---
title: trustFrameworkPolicy
description: 在 Azure AD B2C 信任框架策略中称为 "自定义策略"。 这描述了适用于租户的 trustFrameworkPolicy 对象的操作。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f573b331b587db50019e71468ec98d0e746e3963
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964184"
---
# <a name="trustframeworkpolicy-resource-type"></a><span data-ttu-id="9f680-104">trustFrameworkPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f680-104">trustFrameworkPolicy resource type</span></span>

> <span data-ttu-id="9f680-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f680-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f680-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f680-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f680-107">表示[Azure Active DIRECTORY B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview)中的[信任框架](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)策略 (也称为[自定义策略](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom))。</span><span class="sxs-lookup"><span data-stu-id="9f680-107">Represents a [Trust Framework](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom) policy (also called [custom policy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)) in [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview).</span></span> <span data-ttu-id="9f680-108">信任框架策略提供了对用户旅程的完全控制权限。</span><span class="sxs-lookup"><span data-stu-id="9f680-108">A Trust Framework policy gives full control over the user journeys.</span></span> <span data-ttu-id="9f680-109">使用它可以执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="9f680-109">Use it to:</span></span>

* <span data-ttu-id="9f680-110">完全自定义注册和登录体验。</span><span class="sxs-lookup"><span data-stu-id="9f680-110">Customize the sign-up and sign-in experiences fully.</span></span>
* <span data-ttu-id="9f680-111">联合任何 SAML、Open ID Connect 或 OAuth2 identity provider。</span><span class="sxs-lookup"><span data-stu-id="9f680-111">Federate to any SAML, Open ID Connect, or OAuth2 identity provider.</span></span>
* <span data-ttu-id="9f680-112">通过调用 REST 终结点与其他系统或用户数据存储集成。</span><span class="sxs-lookup"><span data-stu-id="9f680-112">Integrate with other systems or user data stores by calling REST endpoints.</span></span>
* <span data-ttu-id="9f680-113">转换声明并自定义颁发给信赖方应用程序的令牌。</span><span class="sxs-lookup"><span data-stu-id="9f680-113">Transform claims and customize tokens issued to the relying party application.</span></span>

<span data-ttu-id="9f680-114">有关详细信息, 请参阅[Azure Active DIRECTORY B2C 中的自定义策略](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)。</span><span class="sxs-lookup"><span data-stu-id="9f680-114">For more information, see [Custom policies in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom).</span></span>

## <a name="methods"></a><span data-ttu-id="9f680-115">方法</span><span class="sxs-lookup"><span data-stu-id="9f680-115">Methods</span></span>

| <span data-ttu-id="9f680-116">方法</span><span class="sxs-lookup"><span data-stu-id="9f680-116">Method</span></span>       | <span data-ttu-id="9f680-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f680-117">Return Type</span></span>  |<span data-ttu-id="9f680-118">说明</span><span class="sxs-lookup"><span data-stu-id="9f680-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f680-119">创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-119">Create trustFrameworkPolicy</span></span>](../api/trustframework-post-trustframeworkpolicy.md)|<span data-ttu-id="9f680-120">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-120">trustFrameworkPolicy</span></span>|<span data-ttu-id="9f680-121">创建新的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="9f680-121">Create a new trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="9f680-122">获取 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-122">Get trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-get.md) |<span data-ttu-id="9f680-123">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-123">trustFrameworkPolicy</span></span>|<span data-ttu-id="9f680-124">读取现有 trustFrameworkPolicy 的属性。</span><span class="sxs-lookup"><span data-stu-id="9f680-124">Read properties of an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="9f680-125">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="9f680-125">List trustFrameworkPolicies</span></span>](../api/trustframework-list-trustframeworkpolicies.md)|<span data-ttu-id="9f680-126">trustFrameworkPolicy 集合</span><span class="sxs-lookup"><span data-stu-id="9f680-126">trustFrameworkPolicy collection</span></span>|<span data-ttu-id="9f680-127">列出租户中配置的所有 trustFrameworkPolicies。</span><span class="sxs-lookup"><span data-stu-id="9f680-127">List all trustFrameworkPolicies configured in a tenant.</span></span>|
|[<span data-ttu-id="9f680-128">更新或创建 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-128">Update or create trustFrameworkPolicy</span></span>](../api/trustframework-put-trustframeworkpolicy.md)|<span data-ttu-id="9f680-129">无</span><span class="sxs-lookup"><span data-stu-id="9f680-129">None</span></span>|<span data-ttu-id="9f680-130">更新现有的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="9f680-130">Update an existing trustFrameworkPolicy.</span></span>|
|[<span data-ttu-id="9f680-131">删除 trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-131">Delete trustFrameworkPolicy</span></span>](../api/trustframeworkpolicy-delete.md)|<span data-ttu-id="9f680-132">无</span><span class="sxs-lookup"><span data-stu-id="9f680-132">None</span></span>|<span data-ttu-id="9f680-133">删除现有的 trustFrameworkPolicy。</span><span class="sxs-lookup"><span data-stu-id="9f680-133">Delete an existing trustFrameworkPolicy.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f680-134">属性</span><span class="sxs-lookup"><span data-stu-id="9f680-134">Properties</span></span>

|<span data-ttu-id="9f680-135">属性</span><span class="sxs-lookup"><span data-stu-id="9f680-135">Property</span></span>|<span data-ttu-id="9f680-136">类型</span><span class="sxs-lookup"><span data-stu-id="9f680-136">Type</span></span>|<span data-ttu-id="9f680-137">说明</span><span class="sxs-lookup"><span data-stu-id="9f680-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f680-138">id</span><span class="sxs-lookup"><span data-stu-id="9f680-138">id</span></span>|<span data-ttu-id="9f680-139">String</span><span class="sxs-lookup"><span data-stu-id="9f680-139">String</span></span>|<span data-ttu-id="9f680-140">策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="9f680-140">The ID of the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f680-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f680-141">JSON representation</span></span>

<span data-ttu-id="9f680-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f680-142">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9f680-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9f680-143">See also</span></span>

- <span data-ttu-id="9f680-144">[trustFrameworkPolicy 架构](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy), 以了解有关架构元素的信息。</span><span class="sxs-lookup"><span data-stu-id="9f680-144">[trustFrameworkPolicy schema](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy) for information about the schema elements.</span></span>  
- [<span data-ttu-id="9f680-145">trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="9f680-145">trustFrameworkPolicy.xsd</span></span>](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
