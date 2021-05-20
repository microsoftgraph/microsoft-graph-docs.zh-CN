---
title: temporaryAccessPassAuthenticationMethod 资源类型
description: 表示注册到用户的临时访问通道。
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1d4b084bdb66215bb60990c62dbfa6682bafe0b1
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546943"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a><span data-ttu-id="d7147-103">temporaryAccessPassAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7147-103">temporaryAccessPassAuthenticationMethod resource type</span></span>

<span data-ttu-id="d7147-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7147-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7147-105">表示注册到用户的临时访问通道。</span><span class="sxs-lookup"><span data-stu-id="d7147-105">Represents a Temporary Access Pass registered to a user.</span></span> <span data-ttu-id="d7147-106">临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。</span><span class="sxs-lookup"><span data-stu-id="d7147-106">A Temporary Access Pass is a time-limited passcode that serves as a strong credential and allows onboarding of passwordless credentials.</span></span>

## <a name="methods"></a><span data-ttu-id="d7147-107">方法</span><span class="sxs-lookup"><span data-stu-id="d7147-107">Methods</span></span>

|<span data-ttu-id="d7147-108">方法</span><span class="sxs-lookup"><span data-stu-id="d7147-108">Method</span></span>|<span data-ttu-id="d7147-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7147-109">Return type</span></span>|<span data-ttu-id="d7147-110">Description</span><span class="sxs-lookup"><span data-stu-id="d7147-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d7147-111">List</span><span class="sxs-lookup"><span data-stu-id="d7147-111">List</span></span>](../api/temporaryaccesspassauthenticationmethod-list.md)|<span data-ttu-id="d7147-112">[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7147-112">[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) collection</span></span>|<span data-ttu-id="d7147-113">检索用户的临时 **AccessPassAuthenticationMethod** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d7147-113">Retrieve a list of a user's **temporaryAccessPassAuthenticationMethod** objects and their properties.</span></span> <span data-ttu-id="d7147-114">用户只能有一个临时访问传递身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d7147-114">Users can only have one Temporary Access Pass authentication method.</span></span>|
|[<span data-ttu-id="d7147-115">创建</span><span class="sxs-lookup"><span data-stu-id="d7147-115">Create</span></span>](../api/temporaryaccesspassauthenticationmethod-post.md)|[<span data-ttu-id="d7147-116">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d7147-116">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="d7147-117">创建用户 **的临时AccessPassAuthenticationMethod** 对象。</span><span class="sxs-lookup"><span data-stu-id="d7147-117">Create a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|
|[<span data-ttu-id="d7147-118">获取</span><span class="sxs-lookup"><span data-stu-id="d7147-118">Get</span></span>](../api/temporaryaccesspassauthenticationmethod-get.md)|[<span data-ttu-id="d7147-119">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d7147-119">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="d7147-120">检索用户 **temporaryAccessPassAuthenticationMethod 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="d7147-120">Retrieve the properties of the user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|
|[<span data-ttu-id="d7147-121">删除</span><span class="sxs-lookup"><span data-stu-id="d7147-121">Delete</span></span>](../api/temporaryaccesspassauthenticationmethod-delete.md)|<span data-ttu-id="d7147-122">无</span><span class="sxs-lookup"><span data-stu-id="d7147-122">None</span></span>|<span data-ttu-id="d7147-123">删除用户 **的临时AccessPassAuthenticationMethod** 对象。</span><span class="sxs-lookup"><span data-stu-id="d7147-123">Delete a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7147-124">属性</span><span class="sxs-lookup"><span data-stu-id="d7147-124">Properties</span></span>
|<span data-ttu-id="d7147-125">属性</span><span class="sxs-lookup"><span data-stu-id="d7147-125">Property</span></span>|<span data-ttu-id="d7147-126">类型</span><span class="sxs-lookup"><span data-stu-id="d7147-126">Type</span></span>|<span data-ttu-id="d7147-127">说明</span><span class="sxs-lookup"><span data-stu-id="d7147-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7147-128">id</span><span class="sxs-lookup"><span data-stu-id="d7147-128">id</span></span>|<span data-ttu-id="d7147-129">String</span><span class="sxs-lookup"><span data-stu-id="d7147-129">String</span></span>|<span data-ttu-id="d7147-130">注册到此用户的临时访问传递的标识符。</span><span class="sxs-lookup"><span data-stu-id="d7147-130">The identifier of the Temporary Access Pass registered to this user.</span></span>|
|<span data-ttu-id="d7147-131">temporaryAccessPass</span><span class="sxs-lookup"><span data-stu-id="d7147-131">temporaryAccessPass</span></span>|<span data-ttu-id="d7147-132">String</span><span class="sxs-lookup"><span data-stu-id="d7147-132">String</span></span>|<span data-ttu-id="d7147-133">用于进行身份验证的 temporaryAccessPass。</span><span class="sxs-lookup"><span data-stu-id="d7147-133">The temporaryAccessPass used to authenticate.</span></span> <span data-ttu-id="d7147-134">仅在新建 temporaryAccessPass 时返回;与 GET 一起返回为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d7147-134">Returned only on creation of a new temporaryAccessPass; returned as NULL with GET.</span></span>|
|<span data-ttu-id="d7147-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7147-135">createdDateTime</span></span>|<span data-ttu-id="d7147-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7147-136">DateTimeOffset</span></span>|<span data-ttu-id="d7147-137">创建 temporaryAccessPass 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d7147-137">The date and time when the temporaryAccessPass was created.</span></span>|
|<span data-ttu-id="d7147-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d7147-138">startDateTime</span></span>|<span data-ttu-id="d7147-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7147-139">DateTimeOffset</span></span>|<span data-ttu-id="d7147-140">temporaryAccessPass 可供使用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d7147-140">The date and time when the temporaryAccessPass becomes available to use.</span></span>|
|<span data-ttu-id="d7147-141">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d7147-141">lifetimeInMinutes</span></span>|<span data-ttu-id="d7147-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d7147-142">Int32</span></span>|<span data-ttu-id="d7147-143">temporaryAccessPass 的生存期，以分钟计，从 startDateTime 开始。</span><span class="sxs-lookup"><span data-stu-id="d7147-143">The lifetime of the temporaryAccessPass in minutes starting at startDateTime.</span></span> <span data-ttu-id="d7147-144">最少 10 天，最多 43200 (相当于 30 天) 。</span><span class="sxs-lookup"><span data-stu-id="d7147-144">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>|
|<span data-ttu-id="d7147-145">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="d7147-145">isUsableOnce</span></span>|<span data-ttu-id="d7147-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7147-146">Boolean</span></span>|<span data-ttu-id="d7147-147">确定是否将传递限制为一次使用。</span><span class="sxs-lookup"><span data-stu-id="d7147-147">Determines whether the pass is limited to a one time use.</span></span> <span data-ttu-id="d7147-148">如果 `true` 为 ，则传递可以使用一次;如果 为 ，则 pass 可以在 `false` temporaryAccessPass 生存期内多次使用。</span><span class="sxs-lookup"><span data-stu-id="d7147-148">If `true`, the pass can be used once; if `false`, the pass can be used multiple times within the temporaryAccessPass lifetime.</span></span>|
|<span data-ttu-id="d7147-149">isUsable</span><span class="sxs-lookup"><span data-stu-id="d7147-149">isUsable</span></span>|<span data-ttu-id="d7147-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7147-150">Boolean</span></span>|<span data-ttu-id="d7147-151">身份验证方法的状态，指示它当前是否由用户使用。</span><span class="sxs-lookup"><span data-stu-id="d7147-151">The state of the authentication method that indicates whether it's currently usable by the user.</span></span>|
|<span data-ttu-id="d7147-152">methodUsabilityReason</span><span class="sxs-lookup"><span data-stu-id="d7147-152">methodUsabilityReason</span></span>|<span data-ttu-id="d7147-153">String</span><span class="sxs-lookup"><span data-stu-id="d7147-153">String</span></span>|<span data-ttu-id="d7147-154">有关可用性状态的详细信息 (isUsable) 。</span><span class="sxs-lookup"><span data-stu-id="d7147-154">Details about usability state (isUsable).</span></span> <span data-ttu-id="d7147-155">原因可能包括 `enabledByPolicy` `disabledByPolicy` `expired` ：、、、、。 `notYetValid` `oneTimeUsed`</span><span class="sxs-lookup"><span data-stu-id="d7147-155">Reasons can include: `enabledByPolicy`, `disabledByPolicy`, `expired`, `notYetValid`, `oneTimeUsed`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d7147-156">关系</span><span class="sxs-lookup"><span data-stu-id="d7147-156">Relationships</span></span>
<span data-ttu-id="d7147-157">无。</span><span class="sxs-lookup"><span data-stu-id="d7147-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7147-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7147-158">JSON representation</span></span>
<span data-ttu-id="d7147-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7147-159">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "String (identifier)",
  "temporaryAccessPass": "String",
  "createdDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "isUsable": "Boolean",
  "methodUsabilityReason": "String"
}
```
