---
title: featureRolloutPolicy 资源类型
description: 表示与目录对象相关联的功能展示策略。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ec1f42ba951fa1bde827b2900b98e37c62d6160
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845279"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="51d03-103">featureRolloutPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="51d03-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="51d03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51d03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51d03-105">表示与目录对象相关联的功能展示策略。</span><span class="sxs-lookup"><span data-stu-id="51d03-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="51d03-106">创建功能展示策略可帮助租户管理员在为整个组织启用功能之前，使用特定组试点 Azure AD 的功能。</span><span class="sxs-lookup"><span data-stu-id="51d03-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="51d03-107">这将最大限度地减少影响并帮助管理员逐步测试和部署与身份验证相关的功能。</span><span class="sxs-lookup"><span data-stu-id="51d03-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="51d03-108">以下是功能展示的限制：</span><span class="sxs-lookup"><span data-stu-id="51d03-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="51d03-109">每个功能最多支持10个组。</span><span class="sxs-lookup"><span data-stu-id="51d03-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="51d03-110">**AppliesTo**字段仅支持组。</span><span class="sxs-lookup"><span data-stu-id="51d03-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="51d03-111">不支持动态组和嵌套组。</span><span class="sxs-lookup"><span data-stu-id="51d03-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="51d03-112">对于当前只有为使用此首展策略进行展示的每项功能，以下是必备组件。</span><span class="sxs-lookup"><span data-stu-id="51d03-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="51d03-113">传递身份验证</span><span class="sxs-lookup"><span data-stu-id="51d03-113">Passthrough Authentication</span></span>

* <span data-ttu-id="51d03-114">确定运行 Windows Server 2012 R2 或更高版本的服务器（要在其中运行[PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta)代理）的服务器。</span><span class="sxs-lookup"><span data-stu-id="51d03-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="51d03-115">确保服务器已加入域，可以使用 Active Directory 对所选用户进行身份验证，并且可以在出站端口/Url 上与 Azure AD 进行通信。</span><span class="sxs-lookup"><span data-stu-id="51d03-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="51d03-116">[下载](https://aka.ms/getauthagent)& 在服务器上安装 MICROSOFT Azure AD Connect 身份验证代理。</span><span class="sxs-lookup"><span data-stu-id="51d03-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="51d03-117">若要启用高可用性，请在其他服务器上安装其他身份验证代理[，如下所述。](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)</span><span class="sxs-lookup"><span data-stu-id="51d03-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="51d03-118">确保您已正确配置了[智能锁定](/azure/active-directory/authentication/howto-password-smart-lockout)设置。</span><span class="sxs-lookup"><span data-stu-id="51d03-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="51d03-119">这是为了确保用户的本地 Active Directory 帐户不会被不良参与者锁定。</span><span class="sxs-lookup"><span data-stu-id="51d03-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="51d03-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="51d03-120">SeamlessSso</span></span>

* <span data-ttu-id="51d03-121">根据[这些](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)说明为 AD 林启用[SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) 。</span><span class="sxs-lookup"><span data-stu-id="51d03-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="51d03-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="51d03-122">PasswordHashSync</span></span>

* <span data-ttu-id="51d03-123"> [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)   从 Azure AD Connect 中的 "可选功能" 页启用 PasswordHashSync。</span><span class="sxs-lookup"><span data-stu-id="51d03-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="51d03-124">Methods</span><span class="sxs-lookup"><span data-stu-id="51d03-124">Methods</span></span>

| <span data-ttu-id="51d03-125">方法</span><span class="sxs-lookup"><span data-stu-id="51d03-125">Method</span></span>                                                                         | <span data-ttu-id="51d03-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="51d03-126">Return Type</span></span>                                     | <span data-ttu-id="51d03-127">说明</span><span class="sxs-lookup"><span data-stu-id="51d03-127">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="51d03-128">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="51d03-128">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="51d03-129">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-129">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="51d03-130">检索 featureRolloutPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="51d03-130">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="51d03-131">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-131">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="51d03-132">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-132">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="51d03-133">检索 featurerolloutpolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51d03-133">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="51d03-134">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="51d03-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="51d03-136">创建新的 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="51d03-136">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="51d03-137">更新 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-137">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="51d03-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="51d03-139">更新 featurerolloutpolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51d03-139">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="51d03-140">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="51d03-140">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="51d03-141">无</span><span class="sxs-lookup"><span data-stu-id="51d03-141">None</span></span>                                            | <span data-ttu-id="51d03-142">删除 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="51d03-142">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="51d03-143">分配 appliesTo</span><span class="sxs-lookup"><span data-stu-id="51d03-143">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="51d03-144">directoryObject</span><span class="sxs-lookup"><span data-stu-id="51d03-144">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="51d03-145">将 directoryObject 分配给功能推出。</span><span class="sxs-lookup"><span data-stu-id="51d03-145">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="51d03-146">删除 appliesTo</span><span class="sxs-lookup"><span data-stu-id="51d03-146">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="51d03-147">无</span><span class="sxs-lookup"><span data-stu-id="51d03-147">None</span></span>                                            | <span data-ttu-id="51d03-148">从功能推出中删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="51d03-148">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="51d03-149">属性</span><span class="sxs-lookup"><span data-stu-id="51d03-149">Properties</span></span>

| <span data-ttu-id="51d03-150">属性</span><span class="sxs-lookup"><span data-stu-id="51d03-150">Property</span></span>     | <span data-ttu-id="51d03-151">类型</span><span class="sxs-lookup"><span data-stu-id="51d03-151">Type</span></span>        | <span data-ttu-id="51d03-152">说明</span><span class="sxs-lookup"><span data-stu-id="51d03-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51d03-153">说明</span><span class="sxs-lookup"><span data-stu-id="51d03-153">description</span></span>|<span data-ttu-id="51d03-154">String</span><span class="sxs-lookup"><span data-stu-id="51d03-154">String</span></span>|<span data-ttu-id="51d03-155">此功能展示策略的说明。</span><span class="sxs-lookup"><span data-stu-id="51d03-155">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="51d03-156">displayName</span><span class="sxs-lookup"><span data-stu-id="51d03-156">displayName</span></span>|<span data-ttu-id="51d03-157">String</span><span class="sxs-lookup"><span data-stu-id="51d03-157">String</span></span>|<span data-ttu-id="51d03-158">此功能展示策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="51d03-158">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="51d03-159">功能</span><span class="sxs-lookup"><span data-stu-id="51d03-159">feature</span></span>|<span data-ttu-id="51d03-160">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="51d03-160">stagedFeatureName</span></span>| <span data-ttu-id="51d03-161">可取值为：`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="51d03-161">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="51d03-162">id</span><span class="sxs-lookup"><span data-stu-id="51d03-162">id</span></span>|<span data-ttu-id="51d03-163">字符串</span><span class="sxs-lookup"><span data-stu-id="51d03-163">String</span></span>| <span data-ttu-id="51d03-164">只读。</span><span class="sxs-lookup"><span data-stu-id="51d03-164">Read-only.</span></span>|
|<span data-ttu-id="51d03-165">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="51d03-165">isAppliedToOrganization</span></span>|<span data-ttu-id="51d03-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d03-166">Boolean</span></span>|<span data-ttu-id="51d03-167">指示是否应将此功能展示策略应用于整个组织。</span><span class="sxs-lookup"><span data-stu-id="51d03-167">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="51d03-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="51d03-168">isEnabled</span></span>|<span data-ttu-id="51d03-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d03-169">Boolean</span></span>|<span data-ttu-id="51d03-170">指示是否启用功能展示。</span><span class="sxs-lookup"><span data-stu-id="51d03-170">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51d03-171">关系</span><span class="sxs-lookup"><span data-stu-id="51d03-171">Relationships</span></span>

| <span data-ttu-id="51d03-172">关系</span><span class="sxs-lookup"><span data-stu-id="51d03-172">Relationship</span></span> | <span data-ttu-id="51d03-173">类型</span><span class="sxs-lookup"><span data-stu-id="51d03-173">Type</span></span>        | <span data-ttu-id="51d03-174">Description</span><span class="sxs-lookup"><span data-stu-id="51d03-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51d03-175">appliesTo</span><span class="sxs-lookup"><span data-stu-id="51d03-175">appliesTo</span></span>|<span data-ttu-id="51d03-176">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="51d03-176">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="51d03-177">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="51d03-177">Nullable.</span></span> <span data-ttu-id="51d03-178">指定为其启用功能的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="51d03-178">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51d03-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51d03-179">JSON representation</span></span>

<span data-ttu-id="51d03-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51d03-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
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
