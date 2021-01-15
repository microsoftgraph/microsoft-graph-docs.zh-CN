---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用使用 Microsoft Authenticator 身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 395a1a10d9d99ce8ea5475e09a2e082b3bc5ddf3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874464"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="ec816-103">microsoftAuthenticatorAuthenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec816-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="ec816-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec816-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec816-105">在 Azure AD 中启用使用 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) 的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="ec816-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="ec816-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec816-106">Properties</span></span>
|<span data-ttu-id="ec816-107">属性</span><span class="sxs-lookup"><span data-stu-id="ec816-107">Property</span></span>|<span data-ttu-id="ec816-108">类型</span><span class="sxs-lookup"><span data-stu-id="ec816-108">Type</span></span>|<span data-ttu-id="ec816-109">说明</span><span class="sxs-lookup"><span data-stu-id="ec816-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec816-110">id</span><span class="sxs-lookup"><span data-stu-id="ec816-110">id</span></span>|<span data-ttu-id="ec816-111">String</span><span class="sxs-lookup"><span data-stu-id="ec816-111">String</span></span>|<span data-ttu-id="ec816-112">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="ec816-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="ec816-113">isNumberMatchingRequired (Preview) </span><span class="sxs-lookup"><span data-stu-id="ec816-113">isNumberMatchingRequired (Private Preview)</span></span>|<span data-ttu-id="ec816-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec816-114">Boolean</span></span>|<span data-ttu-id="ec816-115">要求用户匹配登录页上显示的数量以批准 MFA 通知。</span><span class="sxs-lookup"><span data-stu-id="ec816-115">Require the user to match the number displayed on the sign-in page to approve the MFA notification.</span></span>|
|<span data-ttu-id="ec816-116">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="ec816-116">isRegistrationRequired</span></span>|<span data-ttu-id="ec816-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec816-117">Boolean</span></span>|<span data-ttu-id="ec816-118">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ec816-118">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="ec816-119">*不支持*。</span><span class="sxs-lookup"><span data-stu-id="ec816-119">*Not supported*.</span></span> |
|<span data-ttu-id="ec816-120">shownContext (Private Preview) </span><span class="sxs-lookup"><span data-stu-id="ec816-120">shownContext (Private Preview)</span></span>|<span data-ttu-id="ec816-121">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="ec816-121">authenticatorAppContextType</span></span>|<span data-ttu-id="ec816-122">确定应在通知正文中向用户显示有关登录的上下文类型。</span><span class="sxs-lookup"><span data-stu-id="ec816-122">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="ec816-123">可取值为：`location`、`app`。</span><span class="sxs-lookup"><span data-stu-id="ec816-123">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="ec816-124">targetType</span><span class="sxs-lookup"><span data-stu-id="ec816-124">targetType</span></span>|<span data-ttu-id="ec816-125">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="ec816-125">authenticationMethodTargetType</span></span>| <span data-ttu-id="ec816-126">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="ec816-126">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec816-127">关系</span><span class="sxs-lookup"><span data-stu-id="ec816-127">Relationships</span></span>
<span data-ttu-id="ec816-128">无。</span><span class="sxs-lookup"><span data-stu-id="ec816-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec816-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec816-129">JSON representation</span></span>
<span data-ttu-id="ec816-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec816-130">The following is a JSON representation of the resource.</span></span>
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

