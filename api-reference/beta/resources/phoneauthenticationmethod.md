---
title: phoneAuthenticationMethod 资源类型
description: 向用户注册的电话的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 93bf64756d0da1e4199fdede55990e695f434480
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997835"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="66176-103">phoneAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="66176-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="66176-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66176-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66176-105">向用户注册的电话的表示形式。</span><span class="sxs-lookup"><span data-stu-id="66176-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="66176-106">此资源包括电话号码、电话类型以及电话是否配置为用户通过 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="66176-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="66176-107">电话具有以下三种类型之一：移动、备用移动或办公室。</span><span class="sxs-lookup"><span data-stu-id="66176-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="66176-108">用户可以为每种类型注册一个号码，并且在添加备用移动电话之前，必须有一个移动电话。</span><span class="sxs-lookup"><span data-stu-id="66176-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="66176-109">将电话用于多重身份验证 (MFA) 或自助服务密码重置 (SSPR) 中，移动电话是默认设置，备用移动电话是备份。</span><span class="sxs-lookup"><span data-stu-id="66176-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="66176-110">移动电话可用于短信和语音呼叫，具体取决于租户设置。</span><span class="sxs-lookup"><span data-stu-id="66176-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="66176-111">办公室电话只能接收语音呼叫，不能接收短信消息。</span><span class="sxs-lookup"><span data-stu-id="66176-111">An office phone can only receive voice calls, not SMS messages.</span></span>

<span data-ttu-id="66176-112">SMS 登录状态属性提供有关电话号码是否已准备好通过短信登录的信息。</span><span class="sxs-lookup"><span data-stu-id="66176-112">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="66176-113">以下是可能的值。</span><span class="sxs-lookup"><span data-stu-id="66176-113">The following are the possible values.</span></span>

|<span data-ttu-id="66176-114">值</span><span class="sxs-lookup"><span data-stu-id="66176-114">Value</span></span>|<span data-ttu-id="66176-115">说明</span><span class="sxs-lookup"><span data-stu-id="66176-115">Description</span></span>|
|--------|-----------|
|`notSupported`|<span data-ttu-id="66176-116">此身份验证方法上不支持主登录-例如，只能在用户的主移动电话号码（而不是备用号码）上启用登录。</span><span class="sxs-lookup"><span data-stu-id="66176-116">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|`notAllowedByPolicy`|<span data-ttu-id="66176-117">此用户未通过策略启用以将此方法用作主要登录。</span><span class="sxs-lookup"><span data-stu-id="66176-117">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|`notConfigured`|<span data-ttu-id="66176-118">此用户由策略启用，以将此方法用作主要登录，但需要执行其他操作以进行配置。</span><span class="sxs-lookup"><span data-stu-id="66176-118">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|`phoneNumberNotUnique`|<span data-ttu-id="66176-119">此用户尝试将电话号码设置为主登录名，但该号码不是唯一的，并且不能用作登录名。</span><span class="sxs-lookup"><span data-stu-id="66176-119">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|`ready`|<span data-ttu-id="66176-120">此身份验证方法已准备就绪，可在主登录中使用。</span><span class="sxs-lookup"><span data-stu-id="66176-120">This authentication method is ready for use in primary sign-in.</span></span>|

## <a name="methods"></a><span data-ttu-id="66176-121">方法</span><span class="sxs-lookup"><span data-stu-id="66176-121">Methods</span></span>

| <span data-ttu-id="66176-122">方法</span><span class="sxs-lookup"><span data-stu-id="66176-122">Method</span></span>       | <span data-ttu-id="66176-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="66176-123">Return Type</span></span> | <span data-ttu-id="66176-124">Description</span><span class="sxs-lookup"><span data-stu-id="66176-124">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66176-125">List</span><span class="sxs-lookup"><span data-stu-id="66176-125">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="66176-126">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="66176-126">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="66176-127">读取此用户的所有 phoneAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66176-127">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| [<span data-ttu-id="66176-128">获取</span><span class="sxs-lookup"><span data-stu-id="66176-128">Get</span></span>](../api/phoneauthenticationmethod-get.md) | [<span data-ttu-id="66176-129">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="66176-129">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="66176-130">读取 phoneAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66176-130">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="66176-131">更新</span><span class="sxs-lookup"><span data-stu-id="66176-131">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="66176-132">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="66176-132">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="66176-133">更新 phoneAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="66176-133">Update phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="66176-134">删除</span><span class="sxs-lookup"><span data-stu-id="66176-134">Delete</span></span>](../api/phoneauthenticationmethod-delete.md) | <span data-ttu-id="66176-135">无</span><span class="sxs-lookup"><span data-stu-id="66176-135">None</span></span> | <span data-ttu-id="66176-136">删除 phoneAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="66176-136">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="66176-137">禁用短信登录</span><span class="sxs-lookup"><span data-stu-id="66176-137">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="66176-138">无</span><span class="sxs-lookup"><span data-stu-id="66176-138">None</span></span>|<span data-ttu-id="66176-139">为用户关闭 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="66176-139">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="66176-140">启用 SMS 登录</span><span class="sxs-lookup"><span data-stu-id="66176-140">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="66176-141">无</span><span class="sxs-lookup"><span data-stu-id="66176-141">None</span></span>|<span data-ttu-id="66176-142">为用户启用 SMS 登录。</span><span class="sxs-lookup"><span data-stu-id="66176-142">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="66176-143">属性</span><span class="sxs-lookup"><span data-stu-id="66176-143">Properties</span></span>

| <span data-ttu-id="66176-144">属性</span><span class="sxs-lookup"><span data-stu-id="66176-144">Property</span></span>     | <span data-ttu-id="66176-145">类型</span><span class="sxs-lookup"><span data-stu-id="66176-145">Type</span></span>        | <span data-ttu-id="66176-146">说明</span><span class="sxs-lookup"><span data-stu-id="66176-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66176-147">id</span><span class="sxs-lookup"><span data-stu-id="66176-147">id</span></span>|<span data-ttu-id="66176-148">String</span><span class="sxs-lookup"><span data-stu-id="66176-148">String</span></span>| <span data-ttu-id="66176-149">注册到此用户的此电话的标识符。</span><span class="sxs-lookup"><span data-stu-id="66176-149">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="66176-150">只读。</span><span class="sxs-lookup"><span data-stu-id="66176-150">Read-only.</span></span>|
|<span data-ttu-id="66176-151">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="66176-151">phoneNumber</span></span>|<span data-ttu-id="66176-152">String</span><span class="sxs-lookup"><span data-stu-id="66176-152">String</span></span>|<span data-ttu-id="66176-153">将电话号码设为文本或呼叫以进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="66176-153">The phone number to text or call for authentication.</span></span> <span data-ttu-id="66176-154">电话号码使用格式 "+ \<country code\> \<number\> x \<extension\> "，扩展名为可选。</span><span class="sxs-lookup"><span data-stu-id="66176-154">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="66176-155">例如，+ 1 5555551234 或 + 1 5555551234x123 是有效的。</span><span class="sxs-lookup"><span data-stu-id="66176-155">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="66176-156">如果创建/更新时编号不符合要求的格式，则会拒绝编号。</span><span class="sxs-lookup"><span data-stu-id="66176-156">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="66176-157">phoneType</span><span class="sxs-lookup"><span data-stu-id="66176-157">phoneType</span></span>|<span data-ttu-id="66176-158">字符串</span><span class="sxs-lookup"><span data-stu-id="66176-158">string</span></span>|<span data-ttu-id="66176-159">此电话的类型。</span><span class="sxs-lookup"><span data-stu-id="66176-159">The type of this phone.</span></span> <span data-ttu-id="66176-160">可能的值包括： `mobile` 、 `alternateMobile` 或 `office` 。</span><span class="sxs-lookup"><span data-stu-id="66176-160">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="66176-161">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="66176-161">smsSignInState</span></span>|<span data-ttu-id="66176-162">字符串</span><span class="sxs-lookup"><span data-stu-id="66176-162">string</span></span>|<span data-ttu-id="66176-163">电话是否已准备好用于短信登录。</span><span class="sxs-lookup"><span data-stu-id="66176-163">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="66176-164">可能的值包括： `notSupported` 、、、、 `notAllowedByPolicy` `notEnabled` `phoneNumberNotUnique` `ready` 或 `notConfigured` 。</span><span class="sxs-lookup"><span data-stu-id="66176-164">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66176-165">关系</span><span class="sxs-lookup"><span data-stu-id="66176-165">Relationships</span></span>

<span data-ttu-id="66176-166">无。</span><span class="sxs-lookup"><span data-stu-id="66176-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66176-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66176-167">JSON representation</span></span>

<span data-ttu-id="66176-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66176-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


