---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 表示 Microsoft 验证 Passwordless 电话登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf6a66abbf745a769a44cf323ebb245c31ecf60
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418269"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="7e511-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e511-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="7e511-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e511-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e511-105">表示 Microsoft 验证 Passwordless 电话登录身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="7e511-105">Represents a Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy.</span></span> <span data-ttu-id="7e511-106">身份验证方法策略定义启用使用身份验证方法的配置设置和用户或组。</span><span class="sxs-lookup"><span data-stu-id="7e511-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

> [!NOTE]
> <span data-ttu-id="7e511-107">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="7e511-107">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="7e511-108">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="7e511-108">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="methods"></a><span data-ttu-id="7e511-109">方法</span><span class="sxs-lookup"><span data-stu-id="7e511-109">Methods</span></span>
|<span data-ttu-id="7e511-110">方法</span><span class="sxs-lookup"><span data-stu-id="7e511-110">Method</span></span>|<span data-ttu-id="7e511-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e511-111">Return type</span></span>|<span data-ttu-id="7e511-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e511-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e511-113">获取</span><span class="sxs-lookup"><span data-stu-id="7e511-113">Get</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="7e511-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e511-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="7e511-115">读取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e511-115">Read the properties and relationships of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="7e511-116">更新</span><span class="sxs-lookup"><span data-stu-id="7e511-116">Update</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="7e511-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e511-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="7e511-118">更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e511-118">Update the properties of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="7e511-119">删除</span><span class="sxs-lookup"><span data-stu-id="7e511-119">Delete</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="7e511-120">无</span><span class="sxs-lookup"><span data-stu-id="7e511-120">None</span></span>|<span data-ttu-id="7e511-121">将 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象还原为其默认配置。</span><span class="sxs-lookup"><span data-stu-id="7e511-121">Reverts the passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="7e511-122">属性</span><span class="sxs-lookup"><span data-stu-id="7e511-122">Properties</span></span>
|<span data-ttu-id="7e511-123">属性</span><span class="sxs-lookup"><span data-stu-id="7e511-123">Property</span></span>|<span data-ttu-id="7e511-124">类型</span><span class="sxs-lookup"><span data-stu-id="7e511-124">Type</span></span>|<span data-ttu-id="7e511-125">说明</span><span class="sxs-lookup"><span data-stu-id="7e511-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e511-126">id</span><span class="sxs-lookup"><span data-stu-id="7e511-126">id</span></span>|<span data-ttu-id="7e511-127">字符串</span><span class="sxs-lookup"><span data-stu-id="7e511-127">String</span></span>|<span data-ttu-id="7e511-128">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="7e511-128">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="7e511-129">state</span><span class="sxs-lookup"><span data-stu-id="7e511-129">state</span></span>|<span data-ttu-id="7e511-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="7e511-130">authenticationMethodState</span></span>|<span data-ttu-id="7e511-131">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="7e511-131">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e511-132">关系</span><span class="sxs-lookup"><span data-stu-id="7e511-132">Relationships</span></span>
|<span data-ttu-id="7e511-133">关系</span><span class="sxs-lookup"><span data-stu-id="7e511-133">Relationship</span></span>|<span data-ttu-id="7e511-134">类型</span><span class="sxs-lookup"><span data-stu-id="7e511-134">Type</span></span>|<span data-ttu-id="7e511-135">说明</span><span class="sxs-lookup"><span data-stu-id="7e511-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e511-136">includeTargets</span><span class="sxs-lookup"><span data-stu-id="7e511-136">includeTargets</span></span>|<span data-ttu-id="7e511-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e511-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="7e511-138">启用使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="7e511-138">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e511-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e511-139">JSON representation</span></span>
<span data-ttu-id="7e511-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e511-140">The following is a JSON representation of the resource.</span></span>
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
