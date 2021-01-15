---
title: microsoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 表示 Microsoft Authenticator 身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2d5dbc64fe81b629f89cf0b98bd3f2d32c1411
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874465"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="6c305-103">microsoftAuthenticatorAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c305-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="6c305-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c305-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c305-105">表示 Microsoft Authenticator 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="6c305-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="6c305-106">身份验证方法策略定义配置设置以及已启用使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="6c305-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="6c305-107">方法</span><span class="sxs-lookup"><span data-stu-id="6c305-107">Methods</span></span>
|<span data-ttu-id="6c305-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c305-108">Method</span></span>|<span data-ttu-id="6c305-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c305-109">Return type</span></span>|<span data-ttu-id="6c305-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c305-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c305-111">获取</span><span class="sxs-lookup"><span data-stu-id="6c305-111">Get</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="6c305-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c305-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="6c305-113">读取 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c305-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="6c305-114">更新</span><span class="sxs-lookup"><span data-stu-id="6c305-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="6c305-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c305-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="6c305-116">更新 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c305-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="6c305-117">删除</span><span class="sxs-lookup"><span data-stu-id="6c305-117">Delete</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="6c305-118">无</span><span class="sxs-lookup"><span data-stu-id="6c305-118">None</span></span>|<span data-ttu-id="6c305-119">将 microsoftAuthenticatorAuthenticationMethodConfiguration 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="6c305-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c305-120">属性</span><span class="sxs-lookup"><span data-stu-id="6c305-120">Properties</span></span>
|<span data-ttu-id="6c305-121">属性</span><span class="sxs-lookup"><span data-stu-id="6c305-121">Property</span></span>|<span data-ttu-id="6c305-122">类型</span><span class="sxs-lookup"><span data-stu-id="6c305-122">Type</span></span>|<span data-ttu-id="6c305-123">说明</span><span class="sxs-lookup"><span data-stu-id="6c305-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c305-124">id</span><span class="sxs-lookup"><span data-stu-id="6c305-124">id</span></span>|<span data-ttu-id="6c305-125">String</span><span class="sxs-lookup"><span data-stu-id="6c305-125">String</span></span>|<span data-ttu-id="6c305-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="6c305-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="6c305-127">state</span><span class="sxs-lookup"><span data-stu-id="6c305-127">state</span></span>|<span data-ttu-id="6c305-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="6c305-128">authenticationMethodState</span></span>|<span data-ttu-id="6c305-129">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6c305-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c305-130">关系</span><span class="sxs-lookup"><span data-stu-id="6c305-130">Relationships</span></span>
|<span data-ttu-id="6c305-131">关系</span><span class="sxs-lookup"><span data-stu-id="6c305-131">Relationship</span></span>|<span data-ttu-id="6c305-132">类型</span><span class="sxs-lookup"><span data-stu-id="6c305-132">Type</span></span>|<span data-ttu-id="6c305-133">Description</span><span class="sxs-lookup"><span data-stu-id="6c305-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c305-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="6c305-134">includeTargets</span></span>|<span data-ttu-id="6c305-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c305-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="6c305-136">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="6c305-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c305-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c305-137">JSON representation</span></span>
<span data-ttu-id="6c305-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c305-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

