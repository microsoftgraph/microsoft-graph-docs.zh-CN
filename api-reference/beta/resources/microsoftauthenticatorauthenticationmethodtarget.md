---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 已启用使用 Microsoft Authenticator 身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8eb9959faaf5f4a6bcaecceb165384be737623d
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292271"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="fcbf6-103">microsoftAuthenticatorAuthenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcbf6-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="fcbf6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcbf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcbf6-105">在 Azure AD 中启用了 [使用 Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) 的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="fcbf6-106">属性</span><span class="sxs-lookup"><span data-stu-id="fcbf6-106">Properties</span></span>
|<span data-ttu-id="fcbf6-107">属性</span><span class="sxs-lookup"><span data-stu-id="fcbf6-107">Property</span></span>|<span data-ttu-id="fcbf6-108">类型</span><span class="sxs-lookup"><span data-stu-id="fcbf6-108">Type</span></span>|<span data-ttu-id="fcbf6-109">说明</span><span class="sxs-lookup"><span data-stu-id="fcbf6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcbf6-110">id</span><span class="sxs-lookup"><span data-stu-id="fcbf6-110">id</span></span>|<span data-ttu-id="fcbf6-111">String</span><span class="sxs-lookup"><span data-stu-id="fcbf6-111">String</span></span>|<span data-ttu-id="fcbf6-112">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="fcbf6-113">isNumberMatchingRequired (Private Preview) </span><span class="sxs-lookup"><span data-stu-id="fcbf6-113">isNumberMatchingRequired (Private Preview)</span></span>|<span data-ttu-id="fcbf6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcbf6-114">Boolean</span></span>|<span data-ttu-id="fcbf6-115">要求用户匹配登录页上显示的数量以批准 MFA 通知。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-115">Require the user to match the number displayed on the sign-in page to approve the MFA notification.</span></span>|
|<span data-ttu-id="fcbf6-116">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="fcbf6-116">isRegistrationRequired</span></span>|<span data-ttu-id="fcbf6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcbf6-117">Boolean</span></span>|<span data-ttu-id="fcbf6-118">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-118">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="fcbf6-119">*不支持*。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-119">*Not supported*.</span></span> |
|<span data-ttu-id="fcbf6-120">shownContext (Private Preview) </span><span class="sxs-lookup"><span data-stu-id="fcbf6-120">shownContext (Private Preview)</span></span>|<span data-ttu-id="fcbf6-121">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="fcbf6-121">authenticatorAppContextType</span></span>|<span data-ttu-id="fcbf6-122">确定应在通知正文中向用户显示有关登录的上下文类型。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-122">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="fcbf6-123">可取值为：`location`、`app`。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-123">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="fcbf6-124">targetType</span><span class="sxs-lookup"><span data-stu-id="fcbf6-124">targetType</span></span>|<span data-ttu-id="fcbf6-125">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="fcbf6-125">authenticationMethodTargetType</span></span>| <span data-ttu-id="fcbf6-126">可取值为：`null`、`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-126">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcbf6-127">关系</span><span class="sxs-lookup"><span data-stu-id="fcbf6-127">Relationships</span></span>
<span data-ttu-id="fcbf6-128">无。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcbf6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcbf6-129">JSON representation</span></span>
<span data-ttu-id="fcbf6-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcbf6-130">The following is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String",
  "isNumberMatchingRequired": "Boolean"
}
```

