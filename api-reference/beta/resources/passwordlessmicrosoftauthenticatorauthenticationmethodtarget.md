---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用使用 Microsoft Authenticator 无密码电话登录身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d3dd874b96a54dc7e764200800e85b445abd50ee
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137653"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a><span data-ttu-id="2c842-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget (已弃) </span><span class="sxs-lookup"><span data-stu-id="2c842-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type (deprecated)</span></span>

<span data-ttu-id="2c842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c842-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c842-105">已启用使用 Microsoft Authenticator 无密码电话登录身份验证方法策略的用户或组的集合] (。/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) Azure AD 中。</span><span class="sxs-lookup"><span data-stu-id="2c842-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!CAUTION]
> <span data-ttu-id="2c842-106">Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="2c842-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="2c842-107">请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2c842-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c842-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c842-108">Properties</span></span>
|<span data-ttu-id="2c842-109">属性</span><span class="sxs-lookup"><span data-stu-id="2c842-109">Property</span></span>|<span data-ttu-id="2c842-110">类型</span><span class="sxs-lookup"><span data-stu-id="2c842-110">Type</span></span>|<span data-ttu-id="2c842-111">说明</span><span class="sxs-lookup"><span data-stu-id="2c842-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c842-112">id</span><span class="sxs-lookup"><span data-stu-id="2c842-112">id</span></span>|<span data-ttu-id="2c842-113">字符串</span><span class="sxs-lookup"><span data-stu-id="2c842-113">String</span></span>|<span data-ttu-id="2c842-114">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="2c842-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="2c842-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="2c842-115">isRegistrationRequired</span></span>|<span data-ttu-id="2c842-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c842-116">Boolean</span></span>|<span data-ttu-id="2c842-117">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="2c842-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="2c842-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="2c842-118">shownContext</span></span>|<span data-ttu-id="2c842-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="2c842-119">authenticatorAppContextType</span></span>|<span data-ttu-id="2c842-120">可取值为：`location`、`app`。</span><span class="sxs-lookup"><span data-stu-id="2c842-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="2c842-121">targetType</span><span class="sxs-lookup"><span data-stu-id="2c842-121">targetType</span></span>|<span data-ttu-id="2c842-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="2c842-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="2c842-123">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="2c842-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="2c842-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="2c842-124">useForSignIn</span></span>|<span data-ttu-id="2c842-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c842-125">Boolean</span></span>|<span data-ttu-id="2c842-126">确定是否可以使用身份验证方法登录到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="2c842-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c842-127">关系</span><span class="sxs-lookup"><span data-stu-id="2c842-127">Relationships</span></span>
<span data-ttu-id="2c842-128">无。</span><span class="sxs-lookup"><span data-stu-id="2c842-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c842-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c842-129">JSON representation</span></span>
<span data-ttu-id="2c842-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c842-130">The following is a JSON representation of the resource.</span></span>
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
