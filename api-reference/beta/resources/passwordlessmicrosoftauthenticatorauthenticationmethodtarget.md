---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用了用户或组的集合，以使用 Microsoft 身份验证器 Passwordless Phone 登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a26a8fe76da954d3dc44a238665954539df0fa72
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418268"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="7fc5b-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fc5b-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type</span></span>

<span data-ttu-id="7fc5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fc5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fc5b-105">启用使用 Microsoft authentication Passwordless Phone 登录身份验证方法策略] ( 的用户或组的集合。。/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) 在 Azure AD 中。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!NOTE]
> <span data-ttu-id="7fc5b-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="7fc5b-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="7fc5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7fc5b-108">Properties</span></span>
|<span data-ttu-id="7fc5b-109">属性</span><span class="sxs-lookup"><span data-stu-id="7fc5b-109">Property</span></span>|<span data-ttu-id="7fc5b-110">类型</span><span class="sxs-lookup"><span data-stu-id="7fc5b-110">Type</span></span>|<span data-ttu-id="7fc5b-111">说明</span><span class="sxs-lookup"><span data-stu-id="7fc5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc5b-112">id</span><span class="sxs-lookup"><span data-stu-id="7fc5b-112">id</span></span>|<span data-ttu-id="7fc5b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7fc5b-113">String</span></span>|<span data-ttu-id="7fc5b-114">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="7fc5b-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="7fc5b-115">isRegistrationRequired</span></span>|<span data-ttu-id="7fc5b-116">布尔</span><span class="sxs-lookup"><span data-stu-id="7fc5b-116">Boolean</span></span>|<span data-ttu-id="7fc5b-117">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="7fc5b-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="7fc5b-118">shownContext</span></span>|<span data-ttu-id="7fc5b-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="7fc5b-119">authenticatorAppContextType</span></span>|<span data-ttu-id="7fc5b-120">可取值为：`location`、`app`。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="7fc5b-121">targetType</span><span class="sxs-lookup"><span data-stu-id="7fc5b-121">targetType</span></span>|<span data-ttu-id="7fc5b-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="7fc5b-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="7fc5b-123">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="7fc5b-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="7fc5b-124">useForSignIn</span></span>|<span data-ttu-id="7fc5b-125">布尔</span><span class="sxs-lookup"><span data-stu-id="7fc5b-125">Boolean</span></span>|<span data-ttu-id="7fc5b-126">确定身份验证方法是否可用于登录 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fc5b-127">关系</span><span class="sxs-lookup"><span data-stu-id="7fc5b-127">Relationships</span></span>
<span data-ttu-id="7fc5b-128">无。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fc5b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fc5b-129">JSON representation</span></span>
<span data-ttu-id="7fc5b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fc5b-130">The following is a JSON representation of the resource.</span></span>
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
