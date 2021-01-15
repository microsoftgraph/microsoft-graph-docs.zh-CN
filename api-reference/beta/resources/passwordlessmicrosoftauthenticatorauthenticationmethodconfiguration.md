---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 代表 Microsoft Authenticator 无密码电话登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e27424264293d87775937c7893546ec321728b4a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872280"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a><span data-ttu-id="12cc3-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="12cc3-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type (deprecated)</span></span>

<span data-ttu-id="12cc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12cc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12cc3-105">代表 Microsoft Authenticator 无密码电话登录身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="12cc3-105">Represents a Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy.</span></span> <span data-ttu-id="12cc3-106">身份验证方法策略定义配置设置以及已启用使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="12cc3-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

> [!CAUTION]
> <span data-ttu-id="12cc3-107">Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="12cc3-107">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="12cc3-108">请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="12cc3-108">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>


## <a name="methods"></a><span data-ttu-id="12cc3-109">方法</span><span class="sxs-lookup"><span data-stu-id="12cc3-109">Methods</span></span>
|<span data-ttu-id="12cc3-110">方法</span><span class="sxs-lookup"><span data-stu-id="12cc3-110">Method</span></span>|<span data-ttu-id="12cc3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="12cc3-111">Return type</span></span>|<span data-ttu-id="12cc3-112">Description</span><span class="sxs-lookup"><span data-stu-id="12cc3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cc3-113">[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (弃) </span><span class="sxs-lookup"><span data-stu-id="12cc3-113">[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (deprecated)</span></span>|[<span data-ttu-id="12cc3-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="12cc3-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="12cc3-115">读取无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12cc3-115">Read the properties and relationships of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="12cc3-116">[更新](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (弃用) </span><span class="sxs-lookup"><span data-stu-id="12cc3-116">[Update](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (deprecated)</span></span> |[<span data-ttu-id="12cc3-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="12cc3-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="12cc3-118">更新无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12cc3-118">Update the properties of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="12cc3-119">[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (已弃) </span><span class="sxs-lookup"><span data-stu-id="12cc3-119">[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (deprecated)</span></span>|<span data-ttu-id="12cc3-120">无</span><span class="sxs-lookup"><span data-stu-id="12cc3-120">None</span></span>|<span data-ttu-id="12cc3-121">将无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="12cc3-121">Reverts the passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="12cc3-122">属性</span><span class="sxs-lookup"><span data-stu-id="12cc3-122">Properties</span></span>
|<span data-ttu-id="12cc3-123">属性</span><span class="sxs-lookup"><span data-stu-id="12cc3-123">Property</span></span>|<span data-ttu-id="12cc3-124">类型</span><span class="sxs-lookup"><span data-stu-id="12cc3-124">Type</span></span>|<span data-ttu-id="12cc3-125">说明</span><span class="sxs-lookup"><span data-stu-id="12cc3-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cc3-126">id</span><span class="sxs-lookup"><span data-stu-id="12cc3-126">id</span></span>|<span data-ttu-id="12cc3-127">String</span><span class="sxs-lookup"><span data-stu-id="12cc3-127">String</span></span>|<span data-ttu-id="12cc3-128">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="12cc3-128">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="12cc3-129">state</span><span class="sxs-lookup"><span data-stu-id="12cc3-129">state</span></span>|<span data-ttu-id="12cc3-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="12cc3-130">authenticationMethodState</span></span>|<span data-ttu-id="12cc3-131">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="12cc3-131">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12cc3-132">关系</span><span class="sxs-lookup"><span data-stu-id="12cc3-132">Relationships</span></span>
|<span data-ttu-id="12cc3-133">关系</span><span class="sxs-lookup"><span data-stu-id="12cc3-133">Relationship</span></span>|<span data-ttu-id="12cc3-134">类型</span><span class="sxs-lookup"><span data-stu-id="12cc3-134">Type</span></span>|<span data-ttu-id="12cc3-135">Description</span><span class="sxs-lookup"><span data-stu-id="12cc3-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cc3-136">includeTargets</span><span class="sxs-lookup"><span data-stu-id="12cc3-136">includeTargets</span></span>|<span data-ttu-id="12cc3-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12cc3-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="12cc3-138">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="12cc3-138">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12cc3-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12cc3-139">JSON representation</span></span>
<span data-ttu-id="12cc3-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12cc3-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
