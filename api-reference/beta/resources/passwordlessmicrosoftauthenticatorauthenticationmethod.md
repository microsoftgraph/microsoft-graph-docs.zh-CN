---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型
description: 向用户注册的 Microsoft 身份验证 Passwordless 电话登录方法的表示形式。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b34b807106591390198c58d26d7804dc6ada5460
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418270"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="50353-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="50353-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="50353-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50353-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50353-105">向用户注册的 Microsoft 身份验证 Passwordless 电话登录方法的表示形式。</span><span class="sxs-lookup"><span data-stu-id="50353-105">A representation of a Microsoft Authenticator Passwordless Phone Sign-in method registered to a user.</span></span>

> [!NOTE]
> <span data-ttu-id="50353-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="50353-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="50353-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="50353-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="methods"></a><span data-ttu-id="50353-108">方法</span><span class="sxs-lookup"><span data-stu-id="50353-108">Methods</span></span>
|<span data-ttu-id="50353-109">方法</span><span class="sxs-lookup"><span data-stu-id="50353-109">Method</span></span>|<span data-ttu-id="50353-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="50353-110">Return type</span></span>|<span data-ttu-id="50353-111">说明</span><span class="sxs-lookup"><span data-stu-id="50353-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50353-112">List</span><span class="sxs-lookup"><span data-stu-id="50353-112">List</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="50353-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50353-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="50353-114">检索用户的 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="50353-114">Retrieve a list of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="50353-115">获取</span><span class="sxs-lookup"><span data-stu-id="50353-115">Get</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="50353-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="50353-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="50353-117">读取用户的 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50353-117">Read the properties and relationships of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="50353-118">删除</span><span class="sxs-lookup"><span data-stu-id="50353-118">Delete</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="50353-119">无</span><span class="sxs-lookup"><span data-stu-id="50353-119">None</span></span>|<span data-ttu-id="50353-120">删除用户的 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="50353-120">Deletes a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="50353-121">属性</span><span class="sxs-lookup"><span data-stu-id="50353-121">Properties</span></span>
|<span data-ttu-id="50353-122">属性</span><span class="sxs-lookup"><span data-stu-id="50353-122">Property</span></span>|<span data-ttu-id="50353-123">类型</span><span class="sxs-lookup"><span data-stu-id="50353-123">Type</span></span>|<span data-ttu-id="50353-124">说明</span><span class="sxs-lookup"><span data-stu-id="50353-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50353-125">id</span><span class="sxs-lookup"><span data-stu-id="50353-125">id</span></span>|<span data-ttu-id="50353-126">字符串</span><span class="sxs-lookup"><span data-stu-id="50353-126">String</span></span>|<span data-ttu-id="50353-127">身份验证方法标识符。</span><span class="sxs-lookup"><span data-stu-id="50353-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="50353-128">displayName</span><span class="sxs-lookup"><span data-stu-id="50353-128">displayName</span></span>|<span data-ttu-id="50353-129">字符串</span><span class="sxs-lookup"><span data-stu-id="50353-129">String</span></span>|<span data-ttu-id="50353-130">由用户指定的移动设备的显示名称。</span><span class="sxs-lookup"><span data-stu-id="50353-130">The display name of the mobile device as given by the user.</span></span>|
|<span data-ttu-id="50353-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="50353-131">creationDateTime</span></span>|<span data-ttu-id="50353-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50353-132">DateTimeOffset</span></span>|<span data-ttu-id="50353-133">向用户注册此方法时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="50353-133">The timestamp when this method was registered to the user.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="50353-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50353-134">JSON representation</span></span>
<span data-ttu-id="50353-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50353-135">The following is a JSON representation of the resource.</span></span>
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

