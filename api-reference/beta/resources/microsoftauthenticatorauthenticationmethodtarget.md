---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用以使用身份验证方法策略Microsoft Authenticator组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db534dfb13e288b82b49005b2b1a923b8bfd5112
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896639"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="efa9c-103">microsoftAuthenticatorAuthenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="efa9c-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="efa9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efa9c-105">在 Azure AD 中启用以使用Microsoft Authenticator[方法策略的用户](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)或组的集合。</span><span class="sxs-lookup"><span data-stu-id="efa9c-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="efa9c-106">属性</span><span class="sxs-lookup"><span data-stu-id="efa9c-106">Properties</span></span>
|<span data-ttu-id="efa9c-107">属性</span><span class="sxs-lookup"><span data-stu-id="efa9c-107">Property</span></span>|<span data-ttu-id="efa9c-108">类型</span><span class="sxs-lookup"><span data-stu-id="efa9c-108">Type</span></span>|<span data-ttu-id="efa9c-109">说明</span><span class="sxs-lookup"><span data-stu-id="efa9c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa9c-110">id</span><span class="sxs-lookup"><span data-stu-id="efa9c-110">id</span></span>|<span data-ttu-id="efa9c-111">String</span><span class="sxs-lookup"><span data-stu-id="efa9c-111">String</span></span>|<span data-ttu-id="efa9c-112">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="efa9c-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="efa9c-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="efa9c-113">authenticationMode</span></span>|<span data-ttu-id="efa9c-114">microsoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="efa9c-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="efa9c-115">确定可用于登录的通知类型。</span><span class="sxs-lookup"><span data-stu-id="efa9c-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="efa9c-116">可能的值是 `any` `deviceBasedPush` ：、 (无密码) 、 `push` 。</span><span class="sxs-lookup"><span data-stu-id="efa9c-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="efa9c-117">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="efa9c-117">isRegistrationRequired</span></span>|<span data-ttu-id="efa9c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa9c-118">Boolean</span></span>|<span data-ttu-id="efa9c-119">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="efa9c-119">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="efa9c-120">*不支持*。</span><span class="sxs-lookup"><span data-stu-id="efa9c-120">*Not supported*.</span></span> |
|<span data-ttu-id="efa9c-121">numberMatchingRequiredState</span><span class="sxs-lookup"><span data-stu-id="efa9c-121">numberMatchingRequiredState</span></span>|<span data-ttu-id="efa9c-122">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="efa9c-122">advancedConfigState</span></span>|<span data-ttu-id="efa9c-123">需要匹配 MFA 通知的号码。</span><span class="sxs-lookup"><span data-stu-id="efa9c-123">Requires number matching for MFA notifications.</span></span> <span data-ttu-id="efa9c-124">手机登录通知的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="efa9c-124">Value is ignored for phone sign-in notifications.</span></span> <span data-ttu-id="efa9c-125">可取值为：`enabled`、`disabled`、`default`。</span><span class="sxs-lookup"><span data-stu-id="efa9c-125">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="efa9c-126">displayLocationInformationRequiredState</span><span class="sxs-lookup"><span data-stu-id="efa9c-126">displayLocationInformationRequiredState</span></span>|<span data-ttu-id="efa9c-127">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="efa9c-127">advancedConfigState</span></span>|<span data-ttu-id="efa9c-128">确定是否应在通知正文中向用户显示登录的位置。</span><span class="sxs-lookup"><span data-stu-id="efa9c-128">Determines whether the location of the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="efa9c-129">可取值为：`enabled`、`disabled`、`default`。</span><span class="sxs-lookup"><span data-stu-id="efa9c-129">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="efa9c-130">displayAppInformationRequiredState</span><span class="sxs-lookup"><span data-stu-id="efa9c-130">displayAppInformationRequiredState</span></span>|<span data-ttu-id="efa9c-131">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="efa9c-131">advancedConfigState</span></span>|<span data-ttu-id="efa9c-132">确定是否应在通知正文中向用户显示用户登录的应用。</span><span class="sxs-lookup"><span data-stu-id="efa9c-132">Determines whether the app the user is signing into should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="efa9c-133">可取值为：`enabled`、`disabled`、`default`。</span><span class="sxs-lookup"><span data-stu-id="efa9c-133">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="efa9c-134">targetType</span><span class="sxs-lookup"><span data-stu-id="efa9c-134">targetType</span></span>|<span data-ttu-id="efa9c-135">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="efa9c-135">authenticationMethodTargetType</span></span>| <span data-ttu-id="efa9c-136">可取值为：`null`、`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="efa9c-136">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efa9c-137">关系</span><span class="sxs-lookup"><span data-stu-id="efa9c-137">Relationships</span></span>
<span data-ttu-id="efa9c-138">无。</span><span class="sxs-lookup"><span data-stu-id="efa9c-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efa9c-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efa9c-139">JSON representation</span></span>
<span data-ttu-id="efa9c-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efa9c-140">The following is a JSON representation of the resource.</span></span>
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
  "numberMatchingRequiredState": "String",
  "displayLocationInformationRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
