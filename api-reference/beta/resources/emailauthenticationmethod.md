---
title: emailAuthenticationMethod 资源类型
description: '注册到用户的电子邮件地址的表示形式。 电子邮件是一种身份验证方法，仅适用于 SSPR (的自助服务密码) '
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a24a67fdb4bcc054036de26ba235bf4bac0f2da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440365"
---
# <a name="emailauthenticationmethod-resource-type"></a><span data-ttu-id="ea63d-104">emailAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea63d-104">emailAuthenticationMethod resource type</span></span>

<span data-ttu-id="ea63d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea63d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea63d-106">注册到用户的电子邮件地址的表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea63d-106">A representation of an email address registered to a user.</span></span> <span data-ttu-id="ea63d-107">电子邮件是一种身份验证方法，仅适用于 SSPR (的自助服务密码) 。</span><span class="sxs-lookup"><span data-stu-id="ea63d-107">Email is an authentication method available only to self-service password reset (SSPR).</span></span> <span data-ttu-id="ea63d-108">用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ea63d-108">Users may only have one email authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="ea63d-109">Methods</span><span class="sxs-lookup"><span data-stu-id="ea63d-109">Methods</span></span>
|<span data-ttu-id="ea63d-110">方法</span><span class="sxs-lookup"><span data-stu-id="ea63d-110">Method</span></span>|<span data-ttu-id="ea63d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea63d-111">Return type</span></span>|<span data-ttu-id="ea63d-112">Description</span><span class="sxs-lookup"><span data-stu-id="ea63d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea63d-113">List</span><span class="sxs-lookup"><span data-stu-id="ea63d-113">List</span></span>](../api/emailauthenticationmethod-list.md)|<span data-ttu-id="ea63d-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea63d-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span></span>|<span data-ttu-id="ea63d-115">检索用户的电子邮件AuthenticationMethods 的列表。</span><span class="sxs-lookup"><span data-stu-id="ea63d-115">Retrieve a list of a user's emailAuthenticationMethods.</span></span> <span data-ttu-id="ea63d-116">用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ea63d-116">Users may only have one email authentication method.</span></span>|
|[<span data-ttu-id="ea63d-117">创建</span><span class="sxs-lookup"><span data-stu-id="ea63d-117">Create</span></span>](../api/emailauthenticationmethod-post.md)|[<span data-ttu-id="ea63d-118">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea63d-118">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="ea63d-119">创建用户的电子邮件Methods 对象。</span><span class="sxs-lookup"><span data-stu-id="ea63d-119">Create a user's emailMethods object.</span></span>|
|[<span data-ttu-id="ea63d-120">获取</span><span class="sxs-lookup"><span data-stu-id="ea63d-120">Get</span></span>](../api/emailauthenticationmethod-get.md)|[<span data-ttu-id="ea63d-121">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea63d-121">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="ea63d-122">检索用户 emailAuthenticationMethod 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea63d-122">Retrieve the properties  of the user's emailAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="ea63d-123">更新</span><span class="sxs-lookup"><span data-stu-id="ea63d-123">Update</span></span>](../api/emailauthenticationmethod-update.md)|[<span data-ttu-id="ea63d-124">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea63d-124">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="ea63d-125">更新用户 emailMethods 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea63d-125">Update the properties of a user's emailMethods object.</span></span>|
|[<span data-ttu-id="ea63d-126">删除</span><span class="sxs-lookup"><span data-stu-id="ea63d-126">Delete</span></span>](../api/emailauthenticationmethod-delete.md)|<span data-ttu-id="ea63d-127">无</span><span class="sxs-lookup"><span data-stu-id="ea63d-127">None</span></span>|<span data-ttu-id="ea63d-128">删除用户的电子邮件AuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="ea63d-128">Delete a user's emailAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="ea63d-129">属性</span><span class="sxs-lookup"><span data-stu-id="ea63d-129">Properties</span></span>
|<span data-ttu-id="ea63d-130">属性</span><span class="sxs-lookup"><span data-stu-id="ea63d-130">Property</span></span>|<span data-ttu-id="ea63d-131">类型</span><span class="sxs-lookup"><span data-stu-id="ea63d-131">Type</span></span>|<span data-ttu-id="ea63d-132">说明</span><span class="sxs-lookup"><span data-stu-id="ea63d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea63d-133">id</span><span class="sxs-lookup"><span data-stu-id="ea63d-133">id</span></span>|<span data-ttu-id="ea63d-134">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-134">String</span></span>|<span data-ttu-id="ea63d-135">注册到此用户的电子邮件地址的标识符。</span><span class="sxs-lookup"><span data-stu-id="ea63d-135">The identifier of the email address registered to this user.</span></span>|
|<span data-ttu-id="ea63d-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ea63d-136">emailAddress</span></span>|<span data-ttu-id="ea63d-137">String</span><span class="sxs-lookup"><span data-stu-id="ea63d-137">String</span></span>|<span data-ttu-id="ea63d-138">注册到此用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ea63d-138">The email address registered to this user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea63d-139">关系</span><span class="sxs-lookup"><span data-stu-id="ea63d-139">Relationships</span></span>
<span data-ttu-id="ea63d-140">无。</span><span class="sxs-lookup"><span data-stu-id="ea63d-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea63d-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea63d-141">JSON representation</span></span>
<span data-ttu-id="ea63d-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea63d-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

