---
title: featureRolloutPolicy 资源类型
description: 表示与目录对象相关联的功能展示策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50d54ae046ef5a0283f5eb2e474fd0faab781687
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062116"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="f16c4-103">featureRolloutPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="f16c4-103">featureRolloutPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f16c4-104">表示与目录对象相关联的功能展示策略。</span><span class="sxs-lookup"><span data-stu-id="f16c4-104">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="f16c4-105">创建功能展示策略可帮助租户管理员在为整个组织启用功能之前, 使用特定组试点 Azure AD 的功能。</span><span class="sxs-lookup"><span data-stu-id="f16c4-105">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="f16c4-106">这将最大限度地减少影响并帮助管理员逐步测试和部署与身份验证相关的功能。</span><span class="sxs-lookup"><span data-stu-id="f16c4-106">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="f16c4-107">以下是功能展示的限制:</span><span class="sxs-lookup"><span data-stu-id="f16c4-107">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="f16c4-108">每个功能最多支持10个组。</span><span class="sxs-lookup"><span data-stu-id="f16c4-108">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="f16c4-109">**AppliesTo**字段仅支持组。</span><span class="sxs-lookup"><span data-stu-id="f16c4-109">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="f16c4-110">不支持动态组和嵌套组。</span><span class="sxs-lookup"><span data-stu-id="f16c4-110">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="f16c4-111">对于当前只有为使用此首展策略进行展示的每项功能, 以下是必备组件。</span><span class="sxs-lookup"><span data-stu-id="f16c4-111">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="f16c4-112">传递身份验证</span><span class="sxs-lookup"><span data-stu-id="f16c4-112">Passthrough Authentication</span></span>

* <span data-ttu-id="f16c4-113">确定运行 Windows Server 2012 R2 或更高版本的服务器 (要在其中运行[PassthroughAuthentication](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta)代理) 的服务器。</span><span class="sxs-lookup"><span data-stu-id="f16c4-113">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="f16c4-114">确保服务器已加入域, 可以使用 Active Directory 对所选用户进行身份验证, 并且可以在出站端口/Url 上与 Azure AD 进行通信。</span><span class="sxs-lookup"><span data-stu-id="f16c4-114"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="f16c4-115">[下载](https://aka.ms/getauthagent)& 在服务器上安装 MICROSOFT Azure AD Connect 身份验证代理。</span><span class="sxs-lookup"><span data-stu-id="f16c4-115">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="f16c4-116">若要启用高可用性, 请在其他服务器上安装其他身份[](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)验证代理, 如下所述。</span><span class="sxs-lookup"><span data-stu-id="f16c4-116">To enable high availability, install additional Authentication Agents on other servers as described [here](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="f16c4-117">确保您已正确配置了[智能锁定](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-password-smart-lockout)设置。</span><span class="sxs-lookup"><span data-stu-id="f16c4-117">Ensure that you have configured your [Smart Lockout](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="f16c4-118">这是为了确保用户的本地 Active Directory 帐户不会被不良参与者锁定。</span><span class="sxs-lookup"><span data-stu-id="f16c4-118">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="f16c4-119">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="f16c4-119">SeamlessSso</span></span>

* <span data-ttu-id="f16c4-120">根据[这些](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)说明为 AD 林启用[SeamlessSso](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso) 。</span><span class="sxs-lookup"><span data-stu-id="f16c4-120">Enable [SeamlessSso](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="f16c4-121">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="f16c4-121">PasswordHashSync</span></span>

* <span data-ttu-id="f16c4-122">从 Azure AD Connect 中的 "可选功能" 页启用 [PasswordHashSync](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs) 。</span><span class="sxs-lookup"><span data-stu-id="f16c4-122">Enable [PasswordHashSync](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="f16c4-123">方法</span><span class="sxs-lookup"><span data-stu-id="f16c4-123">Methods</span></span>

| <span data-ttu-id="f16c4-124">方法</span><span class="sxs-lookup"><span data-stu-id="f16c4-124">Method</span></span>       | <span data-ttu-id="f16c4-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="f16c4-125">Return Type</span></span> | <span data-ttu-id="f16c4-126">说明</span><span class="sxs-lookup"><span data-stu-id="f16c4-126">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f16c4-127">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="f16c4-127">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="f16c4-128">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-128">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="f16c4-129">检索 featureRolloutPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f16c4-129">Retrieve a list of featureRolloutPolicy objects.</span></span> |
| [<span data-ttu-id="f16c4-130">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-130">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="f16c4-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="f16c4-132">检索 featurerolloutpolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f16c4-132">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> ||
| [<span data-ttu-id="f16c4-133">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="f16c4-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="f16c4-135">创建新的 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="f16c4-135">Create a new featureRolloutPolicy object.</span></span>
| [<span data-ttu-id="f16c4-136">更新 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-136">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="f16c4-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="f16c4-138">更新 featurerolloutpolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f16c4-138">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="f16c4-139">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f16c4-139">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="f16c4-140">无</span><span class="sxs-lookup"><span data-stu-id="f16c4-140">None</span></span> | <span data-ttu-id="f16c4-141">删除 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="f16c4-141">Delete a featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="f16c4-142">分配 appliesTo</span><span class="sxs-lookup"><span data-stu-id="f16c4-142">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md) | [<span data-ttu-id="f16c4-143">directoryObject</span><span class="sxs-lookup"><span data-stu-id="f16c4-143">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="f16c4-144">将 directoryObject 分配给功能推出。</span><span class="sxs-lookup"><span data-stu-id="f16c4-144">Assign a directoryObject to feature rollout.</span></span> |
| [<span data-ttu-id="f16c4-145">删除 appliesTo</span><span class="sxs-lookup"><span data-stu-id="f16c4-145">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md) | <span data-ttu-id="f16c4-146">无</span><span class="sxs-lookup"><span data-stu-id="f16c4-146">None</span></span> | <span data-ttu-id="f16c4-147">从功能推出中删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="f16c4-147">Remove a directoryObject from feature rollout.</span></span> |

## <a name="properties"></a><span data-ttu-id="f16c4-148">属性</span><span class="sxs-lookup"><span data-stu-id="f16c4-148">Properties</span></span>

| <span data-ttu-id="f16c4-149">属性</span><span class="sxs-lookup"><span data-stu-id="f16c4-149">Property</span></span>     | <span data-ttu-id="f16c4-150">类型</span><span class="sxs-lookup"><span data-stu-id="f16c4-150">Type</span></span>        | <span data-ttu-id="f16c4-151">说明</span><span class="sxs-lookup"><span data-stu-id="f16c4-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f16c4-152">说明</span><span class="sxs-lookup"><span data-stu-id="f16c4-152">description</span></span>|<span data-ttu-id="f16c4-153">String</span><span class="sxs-lookup"><span data-stu-id="f16c4-153">String</span></span>|<span data-ttu-id="f16c4-154">此功能展示策略的说明。</span><span class="sxs-lookup"><span data-stu-id="f16c4-154">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="f16c4-155">displayName</span><span class="sxs-lookup"><span data-stu-id="f16c4-155">displayName</span></span>|<span data-ttu-id="f16c4-156">String</span><span class="sxs-lookup"><span data-stu-id="f16c4-156">String</span></span>|<span data-ttu-id="f16c4-157">此功能展示策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f16c4-157">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="f16c4-158">功能</span><span class="sxs-lookup"><span data-stu-id="f16c4-158">feature</span></span>|<span data-ttu-id="f16c4-159">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="f16c4-159">stagedFeatureName</span></span>| <span data-ttu-id="f16c4-160">可取值为：`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f16c4-160">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f16c4-161">id</span><span class="sxs-lookup"><span data-stu-id="f16c4-161">id</span></span>|<span data-ttu-id="f16c4-162">String</span><span class="sxs-lookup"><span data-stu-id="f16c4-162">String</span></span>| <span data-ttu-id="f16c4-163">只读。</span><span class="sxs-lookup"><span data-stu-id="f16c4-163">Read-only.</span></span>|
|<span data-ttu-id="f16c4-164">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="f16c4-164">isAppliedToOrganization</span></span>|<span data-ttu-id="f16c4-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f16c4-165">Boolean</span></span>|<span data-ttu-id="f16c4-166">指示是否应将此功能展示策略应用于整个组织。</span><span class="sxs-lookup"><span data-stu-id="f16c4-166">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="f16c4-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f16c4-167">isEnabled</span></span>|<span data-ttu-id="f16c4-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f16c4-168">Boolean</span></span>|<span data-ttu-id="f16c4-169">指示是否启用功能展示。</span><span class="sxs-lookup"><span data-stu-id="f16c4-169">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f16c4-170">关系</span><span class="sxs-lookup"><span data-stu-id="f16c4-170">Relationships</span></span>

| <span data-ttu-id="f16c4-171">关系</span><span class="sxs-lookup"><span data-stu-id="f16c4-171">Relationship</span></span> | <span data-ttu-id="f16c4-172">类型</span><span class="sxs-lookup"><span data-stu-id="f16c4-172">Type</span></span>        | <span data-ttu-id="f16c4-173">说明</span><span class="sxs-lookup"><span data-stu-id="f16c4-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f16c4-174">appliesTo</span><span class="sxs-lookup"><span data-stu-id="f16c4-174">appliesTo</span></span>|<span data-ttu-id="f16c4-175">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="f16c4-175">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="f16c4-176">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f16c4-176">Nullable.</span></span> <span data-ttu-id="f16c4-177">指定为其启用功能的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="f16c4-177">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f16c4-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f16c4-178">JSON representation</span></span>

<span data-ttu-id="f16c4-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f16c4-179">The following is a JSON representation of the resource.</span></span>

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
