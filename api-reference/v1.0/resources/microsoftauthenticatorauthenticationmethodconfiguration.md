---
title: microsoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 表示 Microsoft Authenticator 身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0700a6811b35123709628abc66d8e4eb6b319a03
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469260"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="ffe6b-103">microsoftAuthenticatorAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffe6b-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="ffe6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffe6b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffe6b-105">表示 Microsoft Authenticator 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="ffe6b-106">身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="ffe6b-107">方法</span><span class="sxs-lookup"><span data-stu-id="ffe6b-107">Methods</span></span>
|<span data-ttu-id="ffe6b-108">方法</span><span class="sxs-lookup"><span data-stu-id="ffe6b-108">Method</span></span>|<span data-ttu-id="ffe6b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffe6b-109">Return type</span></span>|<span data-ttu-id="ffe6b-110">说明</span><span class="sxs-lookup"><span data-stu-id="ffe6b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ffe6b-111">获取</span><span class="sxs-lookup"><span data-stu-id="ffe6b-111">Get</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="ffe6b-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffe6b-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="ffe6b-113">读取 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ffe6b-114">更新</span><span class="sxs-lookup"><span data-stu-id="ffe6b-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="ffe6b-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffe6b-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="ffe6b-116">更新 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ffe6b-117">删除</span><span class="sxs-lookup"><span data-stu-id="ffe6b-117">Delete</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="ffe6b-118">无</span><span class="sxs-lookup"><span data-stu-id="ffe6b-118">None</span></span>|<span data-ttu-id="ffe6b-119">将 microsoftAuthenticatorAuthenticationMethodConfiguration 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="ffe6b-120">属性</span><span class="sxs-lookup"><span data-stu-id="ffe6b-120">Properties</span></span>
|<span data-ttu-id="ffe6b-121">属性</span><span class="sxs-lookup"><span data-stu-id="ffe6b-121">Property</span></span>|<span data-ttu-id="ffe6b-122">类型</span><span class="sxs-lookup"><span data-stu-id="ffe6b-122">Type</span></span>|<span data-ttu-id="ffe6b-123">说明</span><span class="sxs-lookup"><span data-stu-id="ffe6b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe6b-124">id</span><span class="sxs-lookup"><span data-stu-id="ffe6b-124">id</span></span>|<span data-ttu-id="ffe6b-125">String</span><span class="sxs-lookup"><span data-stu-id="ffe6b-125">String</span></span>|<span data-ttu-id="ffe6b-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="ffe6b-127">state</span><span class="sxs-lookup"><span data-stu-id="ffe6b-127">state</span></span>|<span data-ttu-id="ffe6b-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="ffe6b-128">authenticationMethodState</span></span>|<span data-ttu-id="ffe6b-129">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffe6b-130">关系</span><span class="sxs-lookup"><span data-stu-id="ffe6b-130">Relationships</span></span>
|<span data-ttu-id="ffe6b-131">关系</span><span class="sxs-lookup"><span data-stu-id="ffe6b-131">Relationship</span></span>|<span data-ttu-id="ffe6b-132">类型</span><span class="sxs-lookup"><span data-stu-id="ffe6b-132">Type</span></span>|<span data-ttu-id="ffe6b-133">说明</span><span class="sxs-lookup"><span data-stu-id="ffe6b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe6b-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="ffe6b-134">includeTargets</span></span>|<span data-ttu-id="ffe6b-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ffe6b-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="ffe6b-136">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffe6b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffe6b-137">JSON representation</span></span>
<span data-ttu-id="ffe6b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffe6b-138">The following is a JSON representation of the resource.</span></span>
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

