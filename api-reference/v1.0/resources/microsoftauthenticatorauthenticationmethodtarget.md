---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 已启用使用 Microsoft Authenticator 身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 43c8e5a4ba92e838a64ec5f345ae82c744b53dee
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469246"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="6b014-103">microsoftAuthenticatorAuthenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b014-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="6b014-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b014-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b014-105">在 Azure AD 中启用了使用 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) 的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="6b014-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="6b014-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b014-106">Properties</span></span>
|<span data-ttu-id="6b014-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b014-107">Property</span></span>|<span data-ttu-id="6b014-108">类型</span><span class="sxs-lookup"><span data-stu-id="6b014-108">Type</span></span>|<span data-ttu-id="6b014-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b014-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b014-110">id</span><span class="sxs-lookup"><span data-stu-id="6b014-110">id</span></span>|<span data-ttu-id="6b014-111">String</span><span class="sxs-lookup"><span data-stu-id="6b014-111">String</span></span>|<span data-ttu-id="6b014-112">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="6b014-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="6b014-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="6b014-113">authenticationMode</span></span>|<span data-ttu-id="6b014-114">microsoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="6b014-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="6b014-115">确定可用于登录的通知类型。</span><span class="sxs-lookup"><span data-stu-id="6b014-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="6b014-116">可能的值是 `any` `deviceBasedPush` ：、 (无密码) 、 `push` 。</span><span class="sxs-lookup"><span data-stu-id="6b014-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="6b014-117">featureSettings</span><span class="sxs-lookup"><span data-stu-id="6b014-117">featureSettings</span></span>|<span data-ttu-id="6b014-118">authenticatorAppFeatureSettings</span><span class="sxs-lookup"><span data-stu-id="6b014-118">authenticatorAppFeatureSettings</span></span>|<span data-ttu-id="6b014-119">确定应用于 Microsoft Authenticator 的其他设置。</span><span class="sxs-lookup"><span data-stu-id="6b014-119">Determines what additional settings should be applied to Microsoft Authenticator.</span></span> <span data-ttu-id="6b014-120">可能的值是 `null` `requireNumberMatching` ：、 (需要匹配 MFA 通知的号码。</span><span class="sxs-lookup"><span data-stu-id="6b014-120">Possible values are: `null`, `requireNumberMatching` (Requires number matching for MFA notifications.</span></span> <span data-ttu-id="6b014-121">对于手机登录通知，此值将被忽略) 。</span><span class="sxs-lookup"><span data-stu-id="6b014-121">Value is ignored for phone sign-in notifications).</span></span>|
|<span data-ttu-id="6b014-122">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="6b014-122">isRegistrationRequired</span></span>|<span data-ttu-id="6b014-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b014-123">Boolean</span></span>|<span data-ttu-id="6b014-124">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6b014-124">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="6b014-125">*不支持*。</span><span class="sxs-lookup"><span data-stu-id="6b014-125">*Not supported*.</span></span> |
|<span data-ttu-id="6b014-126">shownContext</span><span class="sxs-lookup"><span data-stu-id="6b014-126">shownContext</span></span>|<span data-ttu-id="6b014-127">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="6b014-127">authenticatorAppContextType</span></span>|<span data-ttu-id="6b014-128"> (个人预览) 确定应在通知正文中向用户显示有关登录的上下文类型。</span><span class="sxs-lookup"><span data-stu-id="6b014-128">(Private Preview) Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="6b014-129">可取值为：`location`、`app`。</span><span class="sxs-lookup"><span data-stu-id="6b014-129">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="6b014-130">targetType</span><span class="sxs-lookup"><span data-stu-id="6b014-130">targetType</span></span>|<span data-ttu-id="6b014-131">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="6b014-131">authenticationMethodTargetType</span></span>| <span data-ttu-id="6b014-132">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="6b014-132">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b014-133">关系</span><span class="sxs-lookup"><span data-stu-id="6b014-133">Relationships</span></span>
<span data-ttu-id="6b014-134">无。</span><span class="sxs-lookup"><span data-stu-id="6b014-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b014-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b014-135">JSON representation</span></span>
<span data-ttu-id="6b014-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b014-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "shownContext": "String",
  "featureSettings": "String"
}
```
