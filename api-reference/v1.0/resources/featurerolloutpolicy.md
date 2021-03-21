---
title: featureRolloutPolicy 资源类型
description: 表示与目录对象关联的功能推出策略。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 889ff6c7a36be5580a6a419b6bd99e7e85240632
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964686"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="33c11-103">featureRolloutPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="33c11-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="33c11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33c11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33c11-105">表示与目录对象关联的功能推出策略。</span><span class="sxs-lookup"><span data-stu-id="33c11-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="33c11-106">创建功能推出策略可帮助租户管理员在为整个组织启用功能之前，通过特定组试用 Azure AD 的功能。</span><span class="sxs-lookup"><span data-stu-id="33c11-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="33c11-107">这将最大限度地减少影响，并帮助管理员逐步测试和推出与身份验证相关的功能。</span><span class="sxs-lookup"><span data-stu-id="33c11-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="33c11-108">以下是功能推出的限制：</span><span class="sxs-lookup"><span data-stu-id="33c11-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="33c11-109">每个功能最多支持 10 个组。</span><span class="sxs-lookup"><span data-stu-id="33c11-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="33c11-110">**appliesTo** 字段仅支持组。</span><span class="sxs-lookup"><span data-stu-id="33c11-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="33c11-111">不支持动态组和嵌套组。</span><span class="sxs-lookup"><span data-stu-id="33c11-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="33c11-112">以下是当前支持使用此推出策略进行部署的每个功能的先决条件。</span><span class="sxs-lookup"><span data-stu-id="33c11-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="33c11-113">Passthrough 身份验证</span><span class="sxs-lookup"><span data-stu-id="33c11-113">Passthrough Authentication</span></span>

* <span data-ttu-id="33c11-114">确定在 R2 Windows Server 2012运行 [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) 代理的服务器。</span><span class="sxs-lookup"><span data-stu-id="33c11-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="33c11-115">确保服务器已加入域，可以使用 Active Directory 对所选用户进行身份验证，并且可以在出站端口/URL 上与 Azure AD 通信。</span><span class="sxs-lookup"><span data-stu-id="33c11-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="33c11-116">[下载](https://aka.ms/getauthagent) &在服务器上安装 Microsoft Azure AD Connect 身份验证代理。</span><span class="sxs-lookup"><span data-stu-id="33c11-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="33c11-117">若要启用高可用性，请在其他服务器上安装其他身份验证代理，如下 [所述](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)。</span><span class="sxs-lookup"><span data-stu-id="33c11-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="33c11-118">确保正确配置了 [智能锁定](/azure/active-directory/authentication/howto-password-smart-lockout) 设置。</span><span class="sxs-lookup"><span data-stu-id="33c11-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="33c11-119">这是为了确保你的用户本地 Active Directory 帐户不会被坏角色锁定。</span><span class="sxs-lookup"><span data-stu-id="33c11-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="33c11-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="33c11-120">SeamlessSso</span></span>

* <span data-ttu-id="33c11-121">根据这些说明为 AD[林启用](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)[SeamlessSso。](/azure/active-directory/hybrid/how-to-connect-sso)</span><span class="sxs-lookup"><span data-stu-id="33c11-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="33c11-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="33c11-122">PasswordHashSync</span></span>

* <span data-ttu-id="33c11-123">从 [Azure](/azure/active-directory/hybrid/whatis-phs)   AD Connect 中的"可选功能"页面启用 PasswordHashSync。</span><span class="sxs-lookup"><span data-stu-id="33c11-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

### <a name="emailasalternateid"></a><span data-ttu-id="33c11-124">EmailAsAlternateId</span><span class="sxs-lookup"><span data-stu-id="33c11-124">EmailAsAlternateId</span></span>

* <span data-ttu-id="33c11-125">将备用电子邮件与用户帐户关联。</span><span class="sxs-lookup"><span data-stu-id="33c11-125">Associate alternate email  with user accounts.</span></span>

## <a name="methods"></a><span data-ttu-id="33c11-126">Methods</span><span class="sxs-lookup"><span data-stu-id="33c11-126">Methods</span></span>

| <span data-ttu-id="33c11-127">方法</span><span class="sxs-lookup"><span data-stu-id="33c11-127">Method</span></span>                                                                         | <span data-ttu-id="33c11-128">返回类型</span><span class="sxs-lookup"><span data-stu-id="33c11-128">Return Type</span></span>                                     | <span data-ttu-id="33c11-129">说明</span><span class="sxs-lookup"><span data-stu-id="33c11-129">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="33c11-130">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="33c11-130">List featureRolloutPolicies</span></span>](../api/featurerolloutpolicies-list.md) | [<span data-ttu-id="33c11-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="33c11-132">检索 featureRolloutPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="33c11-132">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="33c11-133">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-133">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="33c11-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="33c11-135">检索 featurerolloutpolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33c11-135">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="33c11-136">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-136">Create featureRolloutPolicy</span></span>](../api/featurerolloutpolicies-post.md) | [<span data-ttu-id="33c11-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="33c11-138">创建新的 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="33c11-138">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="33c11-139">更新 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="33c11-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="33c11-141">更新 featurerolloutpolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="33c11-141">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="33c11-142">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="33c11-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="33c11-143">无</span><span class="sxs-lookup"><span data-stu-id="33c11-143">None</span></span>                                            | <span data-ttu-id="33c11-144">删除 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="33c11-144">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="33c11-145">Assign appliesTo</span><span class="sxs-lookup"><span data-stu-id="33c11-145">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="33c11-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="33c11-146">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="33c11-147">将 directoryObject 分配给功能推出。</span><span class="sxs-lookup"><span data-stu-id="33c11-147">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="33c11-148">Remove appliesTo</span><span class="sxs-lookup"><span data-stu-id="33c11-148">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="33c11-149">无</span><span class="sxs-lookup"><span data-stu-id="33c11-149">None</span></span>                                            | <span data-ttu-id="33c11-150">从功能推出中删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="33c11-150">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="33c11-151">属性</span><span class="sxs-lookup"><span data-stu-id="33c11-151">Properties</span></span>

| <span data-ttu-id="33c11-152">属性</span><span class="sxs-lookup"><span data-stu-id="33c11-152">Property</span></span>     | <span data-ttu-id="33c11-153">类型</span><span class="sxs-lookup"><span data-stu-id="33c11-153">Type</span></span>        | <span data-ttu-id="33c11-154">说明</span><span class="sxs-lookup"><span data-stu-id="33c11-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33c11-155">说明</span><span class="sxs-lookup"><span data-stu-id="33c11-155">description</span></span>|<span data-ttu-id="33c11-156">String</span><span class="sxs-lookup"><span data-stu-id="33c11-156">String</span></span>|<span data-ttu-id="33c11-157">此功能推出策略的说明。</span><span class="sxs-lookup"><span data-stu-id="33c11-157">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="33c11-158">displayName</span><span class="sxs-lookup"><span data-stu-id="33c11-158">displayName</span></span>|<span data-ttu-id="33c11-159">String</span><span class="sxs-lookup"><span data-stu-id="33c11-159">String</span></span>|<span data-ttu-id="33c11-160">此功能显示名称策略的部署策略。</span><span class="sxs-lookup"><span data-stu-id="33c11-160">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="33c11-161">功能</span><span class="sxs-lookup"><span data-stu-id="33c11-161">feature</span></span>|<span data-ttu-id="33c11-162">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="33c11-162">stagedFeatureName</span></span>| <span data-ttu-id="33c11-163">可取值为：`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`emailAsAlternateId`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="33c11-163">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="33c11-164">id</span><span class="sxs-lookup"><span data-stu-id="33c11-164">id</span></span>|<span data-ttu-id="33c11-165">String</span><span class="sxs-lookup"><span data-stu-id="33c11-165">String</span></span>| <span data-ttu-id="33c11-166">只读。</span><span class="sxs-lookup"><span data-stu-id="33c11-166">Read-only.</span></span>|
|<span data-ttu-id="33c11-167">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="33c11-167">isAppliedToOrganization</span></span>|<span data-ttu-id="33c11-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="33c11-168">Boolean</span></span>|<span data-ttu-id="33c11-169">指示是否应当将此功能推出策略应用于整个组织。</span><span class="sxs-lookup"><span data-stu-id="33c11-169">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="33c11-170">isEnabled</span><span class="sxs-lookup"><span data-stu-id="33c11-170">isEnabled</span></span>|<span data-ttu-id="33c11-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="33c11-171">Boolean</span></span>|<span data-ttu-id="33c11-172">指示是否启用功能推出。</span><span class="sxs-lookup"><span data-stu-id="33c11-172">Indicates whether the feature rollout is enabled.</span></span>|

### <a name="stagedfeaturename-values"></a><span data-ttu-id="33c11-173">stagedFeatureName 值</span><span class="sxs-lookup"><span data-stu-id="33c11-173">stagedFeatureName values</span></span> 

|<span data-ttu-id="33c11-174">成员</span><span class="sxs-lookup"><span data-stu-id="33c11-174">Member</span></span>|
|:---|
|<span data-ttu-id="33c11-175">passthroughAuthentication</span><span class="sxs-lookup"><span data-stu-id="33c11-175">passthroughAuthentication</span></span>|
|<span data-ttu-id="33c11-176">seamlessSso</span><span class="sxs-lookup"><span data-stu-id="33c11-176">seamlessSso</span></span>|
|<span data-ttu-id="33c11-177">passwordHashSync</span><span class="sxs-lookup"><span data-stu-id="33c11-177">passwordHashSync</span></span>|
|<span data-ttu-id="33c11-178">emailAsAlternateId</span><span class="sxs-lookup"><span data-stu-id="33c11-178">emailAsAlternateId</span></span>|
|<span data-ttu-id="33c11-179">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="33c11-179">unknownFutureValue</span></span>|

## <a name="relationships"></a><span data-ttu-id="33c11-180">关系</span><span class="sxs-lookup"><span data-stu-id="33c11-180">Relationships</span></span>

| <span data-ttu-id="33c11-181">关系</span><span class="sxs-lookup"><span data-stu-id="33c11-181">Relationship</span></span> | <span data-ttu-id="33c11-182">类型</span><span class="sxs-lookup"><span data-stu-id="33c11-182">Type</span></span>        | <span data-ttu-id="33c11-183">说明</span><span class="sxs-lookup"><span data-stu-id="33c11-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33c11-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="33c11-184">appliesTo</span></span>|<span data-ttu-id="33c11-185">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="33c11-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="33c11-186">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="33c11-186">Nullable.</span></span> <span data-ttu-id="33c11-187">指定启用该功能的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="33c11-187">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33c11-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33c11-188">JSON representation</span></span>

<span data-ttu-id="33c11-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33c11-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


