---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用使用 Microsoft Authenticator 无密码电话登录身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef62b251d6c943bd6290a07fa2b018bddca81ab5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872266"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a><span data-ttu-id="a3a67-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="a3a67-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type (deprecated)</span></span>

<span data-ttu-id="a3a67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a67-105">已启用使用 Microsoft Authenticator 无密码电话登录身份验证方法策略的用户或组的集合] (。/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) Azure AD 中。</span><span class="sxs-lookup"><span data-stu-id="a3a67-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!CAUTION]
> <span data-ttu-id="a3a67-106">Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="a3a67-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="a3a67-107">请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a3a67-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a3a67-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3a67-108">Properties</span></span>
|<span data-ttu-id="a3a67-109">属性</span><span class="sxs-lookup"><span data-stu-id="a3a67-109">Property</span></span>|<span data-ttu-id="a3a67-110">类型</span><span class="sxs-lookup"><span data-stu-id="a3a67-110">Type</span></span>|<span data-ttu-id="a3a67-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3a67-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3a67-112">id</span><span class="sxs-lookup"><span data-stu-id="a3a67-112">id</span></span>|<span data-ttu-id="a3a67-113">String</span><span class="sxs-lookup"><span data-stu-id="a3a67-113">String</span></span>|<span data-ttu-id="a3a67-114">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="a3a67-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="a3a67-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="a3a67-115">isRegistrationRequired</span></span>|<span data-ttu-id="a3a67-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3a67-116">Boolean</span></span>|<span data-ttu-id="a3a67-117">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a3a67-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="a3a67-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="a3a67-118">shownContext</span></span>|<span data-ttu-id="a3a67-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="a3a67-119">authenticatorAppContextType</span></span>|<span data-ttu-id="a3a67-120">可取值为：`location`、`app`。</span><span class="sxs-lookup"><span data-stu-id="a3a67-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="a3a67-121">targetType</span><span class="sxs-lookup"><span data-stu-id="a3a67-121">targetType</span></span>|<span data-ttu-id="a3a67-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="a3a67-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="a3a67-123">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="a3a67-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="a3a67-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="a3a67-124">useForSignIn</span></span>|<span data-ttu-id="a3a67-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3a67-125">Boolean</span></span>|<span data-ttu-id="a3a67-126">确定是否可以使用身份验证方法登录到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="a3a67-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3a67-127">关系</span><span class="sxs-lookup"><span data-stu-id="a3a67-127">Relationships</span></span>
<span data-ttu-id="a3a67-128">无。</span><span class="sxs-lookup"><span data-stu-id="a3a67-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3a67-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3a67-129">JSON representation</span></span>
<span data-ttu-id="a3a67-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3a67-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
