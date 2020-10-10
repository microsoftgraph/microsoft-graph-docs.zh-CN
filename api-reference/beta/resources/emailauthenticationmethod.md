---
title: emailAuthenticationMethod 资源类型
description: 向用户注册的电子邮件地址的表示形式。 电子邮件是一种身份验证方法，仅提供 (SSPR) 的自助密码重置功能
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6dde3c9a859f2527241b66c0172d6b5dd877aac4
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418265"
---
# <a name="emailauthenticationmethod-resource-type"></a><span data-ttu-id="b08fe-104">emailAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="b08fe-104">emailAuthenticationMethod resource type</span></span>

<span data-ttu-id="b08fe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b08fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b08fe-106">向用户注册的电子邮件地址的表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08fe-106">A representation of an email address registered to a user.</span></span> <span data-ttu-id="b08fe-107">电子邮件是一种身份验证方法，仅可用于 (SSPR) 的自助密码重置。</span><span class="sxs-lookup"><span data-stu-id="b08fe-107">Email is an authentication method available only to self-service password reset (SSPR).</span></span> <span data-ttu-id="b08fe-108">用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b08fe-108">Users may only have one email authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="b08fe-109">方法</span><span class="sxs-lookup"><span data-stu-id="b08fe-109">Methods</span></span>
|<span data-ttu-id="b08fe-110">方法</span><span class="sxs-lookup"><span data-stu-id="b08fe-110">Method</span></span>|<span data-ttu-id="b08fe-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b08fe-111">Return type</span></span>|<span data-ttu-id="b08fe-112">说明</span><span class="sxs-lookup"><span data-stu-id="b08fe-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b08fe-113">List</span><span class="sxs-lookup"><span data-stu-id="b08fe-113">List</span></span>](../api/emailauthenticationmethod-list.md)|<span data-ttu-id="b08fe-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b08fe-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span></span>|<span data-ttu-id="b08fe-115">检索用户的 emailAuthenticationMethods 的列表。</span><span class="sxs-lookup"><span data-stu-id="b08fe-115">Retrieve a list of a user's emailAuthenticationMethods.</span></span> <span data-ttu-id="b08fe-116">用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b08fe-116">Users may only have one email authentication method.</span></span>|
|[<span data-ttu-id="b08fe-117">创建</span><span class="sxs-lookup"><span data-stu-id="b08fe-117">Create</span></span>](../api/emailauthenticationmethod-post.md)|[<span data-ttu-id="b08fe-118">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b08fe-118">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="b08fe-119">创建用户的 emailMethods 对象。</span><span class="sxs-lookup"><span data-stu-id="b08fe-119">Create a user's emailMethods object.</span></span>|
|[<span data-ttu-id="b08fe-120">获取</span><span class="sxs-lookup"><span data-stu-id="b08fe-120">Get</span></span>](../api/emailauthenticationmethod-get.md)|[<span data-ttu-id="b08fe-121">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b08fe-121">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="b08fe-122">检索用户的 emailAuthenticationMethod 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b08fe-122">Retrieve the properties  of the user's emailAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="b08fe-123">更新</span><span class="sxs-lookup"><span data-stu-id="b08fe-123">Update</span></span>](../api/emailauthenticationmethod-update.md)|[<span data-ttu-id="b08fe-124">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b08fe-124">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="b08fe-125">更新用户的 emailMethods 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b08fe-125">Update the properties of a user's emailMethods object.</span></span>|
|[<span data-ttu-id="b08fe-126">删除</span><span class="sxs-lookup"><span data-stu-id="b08fe-126">Delete</span></span>](../api/emailauthenticationmethod-delete.md)|<span data-ttu-id="b08fe-127">无</span><span class="sxs-lookup"><span data-stu-id="b08fe-127">None</span></span>|<span data-ttu-id="b08fe-128">删除用户的 emailAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="b08fe-128">Delete a user's emailAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="b08fe-129">属性</span><span class="sxs-lookup"><span data-stu-id="b08fe-129">Properties</span></span>
|<span data-ttu-id="b08fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="b08fe-130">Property</span></span>|<span data-ttu-id="b08fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="b08fe-131">Type</span></span>|<span data-ttu-id="b08fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="b08fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b08fe-133">id</span><span class="sxs-lookup"><span data-stu-id="b08fe-133">id</span></span>|<span data-ttu-id="b08fe-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b08fe-134">String</span></span>|<span data-ttu-id="b08fe-135">向此用户注册的电子邮件地址的标识符。</span><span class="sxs-lookup"><span data-stu-id="b08fe-135">The identifier of the email address registered to this user.</span></span>|
|<span data-ttu-id="b08fe-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b08fe-136">emailAddress</span></span>|<span data-ttu-id="b08fe-137">String</span><span class="sxs-lookup"><span data-stu-id="b08fe-137">String</span></span>|<span data-ttu-id="b08fe-138">向此用户注册的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b08fe-138">The email address registered to this user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b08fe-139">关系</span><span class="sxs-lookup"><span data-stu-id="b08fe-139">Relationships</span></span>
<span data-ttu-id="b08fe-140">无。</span><span class="sxs-lookup"><span data-stu-id="b08fe-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b08fe-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b08fe-141">JSON representation</span></span>
<span data-ttu-id="b08fe-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08fe-142">The following is a JSON representation of the resource.</span></span>
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

