---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型
description: 向用户注册的 Microsoft Authenticator 无密码电话登录方法的表示形式。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8815d84a8a85491399e97f7d10aa2e6cc1aeaf9d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796547"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a><span data-ttu-id="c2f67-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="c2f67-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type (deprecated)</span></span>

<span data-ttu-id="c2f67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2f67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2f67-105">向用户注册的 Microsoft Authenticator 无密码电话登录方法的表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2f67-105">A representation of a Microsoft Authenticator Passwordless Phone Sign-in method registered to a user.</span></span>

> [!CAUTION]
> <span data-ttu-id="c2f67-106">Microsoft Authenticator 无密码电话登录方法 API 已弃用，将在 2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="c2f67-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="c2f67-107">请使用新的 [Microsoft Authenticator 身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethod.md)。</span><span class="sxs-lookup"><span data-stu-id="c2f67-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>


## <a name="methods"></a><span data-ttu-id="c2f67-108">方法</span><span class="sxs-lookup"><span data-stu-id="c2f67-108">Methods</span></span>
|<span data-ttu-id="c2f67-109">方法</span><span class="sxs-lookup"><span data-stu-id="c2f67-109">Method</span></span>|<span data-ttu-id="c2f67-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2f67-110">Return type</span></span>|<span data-ttu-id="c2f67-111">说明</span><span class="sxs-lookup"><span data-stu-id="c2f67-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f67-112">[列出](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (弃) </span><span class="sxs-lookup"><span data-stu-id="c2f67-112">[List](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (deprecated)</span></span>|<span data-ttu-id="c2f67-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2f67-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="c2f67-114">检索用户的无密码MicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c2f67-114">Retrieve a list of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod objects and their properties.</span></span>|
|<span data-ttu-id="c2f67-115">[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (弃) </span><span class="sxs-lookup"><span data-stu-id="c2f67-115">[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (deprecated)</span></span>|[<span data-ttu-id="c2f67-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2f67-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="c2f67-117">读取用户的无密码MicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c2f67-117">Read the properties and relationships of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|
|<span data-ttu-id="c2f67-118">[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (弃) </span><span class="sxs-lookup"><span data-stu-id="c2f67-118">[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (deprecated)</span></span>|<span data-ttu-id="c2f67-119">无</span><span class="sxs-lookup"><span data-stu-id="c2f67-119">None</span></span>|<span data-ttu-id="c2f67-120">删除用户的无密码MicrosoftAuthenticatorAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="c2f67-120">Deletes a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="c2f67-121">属性</span><span class="sxs-lookup"><span data-stu-id="c2f67-121">Properties</span></span>
|<span data-ttu-id="c2f67-122">属性</span><span class="sxs-lookup"><span data-stu-id="c2f67-122">Property</span></span>|<span data-ttu-id="c2f67-123">类型</span><span class="sxs-lookup"><span data-stu-id="c2f67-123">Type</span></span>|<span data-ttu-id="c2f67-124">说明</span><span class="sxs-lookup"><span data-stu-id="c2f67-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f67-125">id</span><span class="sxs-lookup"><span data-stu-id="c2f67-125">id</span></span>|<span data-ttu-id="c2f67-126">String</span><span class="sxs-lookup"><span data-stu-id="c2f67-126">String</span></span>|<span data-ttu-id="c2f67-127">身份验证方法标识符。</span><span class="sxs-lookup"><span data-stu-id="c2f67-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="c2f67-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c2f67-128">displayName</span></span>|<span data-ttu-id="c2f67-129">String</span><span class="sxs-lookup"><span data-stu-id="c2f67-129">String</span></span>|<span data-ttu-id="c2f67-130">用户显示名称移动设备的运行时间。</span><span class="sxs-lookup"><span data-stu-id="c2f67-130">The display name of the mobile device as given by the user.</span></span>|
|<span data-ttu-id="c2f67-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="c2f67-131">creationDateTime</span></span>|<span data-ttu-id="c2f67-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2f67-132">DateTimeOffset</span></span>|<span data-ttu-id="c2f67-133">向用户注册此方法的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c2f67-133">The timestamp when this method was registered to the user.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c2f67-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2f67-134">JSON representation</span></span>
<span data-ttu-id="c2f67-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2f67-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

