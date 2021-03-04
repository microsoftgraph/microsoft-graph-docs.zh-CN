---
title: phoneAuthenticationMethod 资源类型
description: 向用户注册的电话的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2d0ec89e21ff6ab7aa39b05acabd81c2b22bd54f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442899"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="a92bf-103">phoneAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="a92bf-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="a92bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a92bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a92bf-105">向用户注册的电话的表示形式。</span><span class="sxs-lookup"><span data-stu-id="a92bf-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="a92bf-106">此资源包括电话号码、电话类型，以及是否将电话配置为用户通过短信登录。</span><span class="sxs-lookup"><span data-stu-id="a92bf-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="a92bf-107">电话有三种类型之一：移动、备用移动或办公室。</span><span class="sxs-lookup"><span data-stu-id="a92bf-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="a92bf-108">用户可以为每种类型注册一个号码，并且必须拥有移动电话，然后才能添加备用移动电话。</span><span class="sxs-lookup"><span data-stu-id="a92bf-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="a92bf-109">使用电话进行多重身份验证 (MFA) 或自助服务密码重置 (SSPR) 时，移动电话为默认值，备用移动电话为备份。</span><span class="sxs-lookup"><span data-stu-id="a92bf-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="a92bf-110">移动电话可用于短信和语音呼叫，具体取决于租户设置。</span><span class="sxs-lookup"><span data-stu-id="a92bf-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="a92bf-111">Office 电话只能接收语音呼叫，不能接收短信。</span><span class="sxs-lookup"><span data-stu-id="a92bf-111">An office phone can only receive voice calls, not SMS messages.</span></span>

<span data-ttu-id="a92bf-112">SMS 登录状态属性提供有关电话号码是否已准备好通过短信登录的信息。</span><span class="sxs-lookup"><span data-stu-id="a92bf-112">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="a92bf-113">以下是可能的值。</span><span class="sxs-lookup"><span data-stu-id="a92bf-113">The following are the possible values.</span></span>

|<span data-ttu-id="a92bf-114">值</span><span class="sxs-lookup"><span data-stu-id="a92bf-114">Value</span></span>|<span data-ttu-id="a92bf-115">说明</span><span class="sxs-lookup"><span data-stu-id="a92bf-115">Description</span></span>|
|--------|-----------|
|`notSupported`|<span data-ttu-id="a92bf-116">此身份验证方法不支持主登录 -例如，只能对用户的主移动号码（而非备用号码）启用登录。</span><span class="sxs-lookup"><span data-stu-id="a92bf-116">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|`notAllowedByPolicy`|<span data-ttu-id="a92bf-117">策略不启用此用户以将此方法用作主登录。</span><span class="sxs-lookup"><span data-stu-id="a92bf-117">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|`notConfigured`|<span data-ttu-id="a92bf-118">策略使此用户能够使用此方法作为主登录，但需要执行其他操作来配置它。</span><span class="sxs-lookup"><span data-stu-id="a92bf-118">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|`phoneNumberNotUnique`|<span data-ttu-id="a92bf-119">此用户尝试将电话号码设置为主登录，但该号码不是唯一的，不能用作登录名。</span><span class="sxs-lookup"><span data-stu-id="a92bf-119">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|`ready`|<span data-ttu-id="a92bf-120">此身份验证方法可供主登录使用。</span><span class="sxs-lookup"><span data-stu-id="a92bf-120">This authentication method is ready for use in primary sign-in.</span></span>|

## <a name="methods"></a><span data-ttu-id="a92bf-121">Methods</span><span class="sxs-lookup"><span data-stu-id="a92bf-121">Methods</span></span>

| <span data-ttu-id="a92bf-122">方法</span><span class="sxs-lookup"><span data-stu-id="a92bf-122">Method</span></span>       | <span data-ttu-id="a92bf-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="a92bf-123">Return Type</span></span> | <span data-ttu-id="a92bf-124">Description</span><span class="sxs-lookup"><span data-stu-id="a92bf-124">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a92bf-125">List</span><span class="sxs-lookup"><span data-stu-id="a92bf-125">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="a92bf-126">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a92bf-126">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="a92bf-127">读取该用户的所有 phoneAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a92bf-127">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| [<span data-ttu-id="a92bf-128">获取</span><span class="sxs-lookup"><span data-stu-id="a92bf-128">Get</span></span>](../api/phoneauthenticationmethod-get.md) | [<span data-ttu-id="a92bf-129">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a92bf-129">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="a92bf-130">读取 phoneAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a92bf-130">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="a92bf-131">更新</span><span class="sxs-lookup"><span data-stu-id="a92bf-131">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="a92bf-132">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a92bf-132">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="a92bf-133">更新 phoneAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="a92bf-133">Update phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="a92bf-134">删除</span><span class="sxs-lookup"><span data-stu-id="a92bf-134">Delete</span></span>](../api/phoneauthenticationmethod-delete.md) | <span data-ttu-id="a92bf-135">无</span><span class="sxs-lookup"><span data-stu-id="a92bf-135">None</span></span> | <span data-ttu-id="a92bf-136">删除 phoneAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="a92bf-136">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="a92bf-137">禁用短信登录</span><span class="sxs-lookup"><span data-stu-id="a92bf-137">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="a92bf-138">无</span><span class="sxs-lookup"><span data-stu-id="a92bf-138">None</span></span>|<span data-ttu-id="a92bf-139">关闭用户的短信登录。</span><span class="sxs-lookup"><span data-stu-id="a92bf-139">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="a92bf-140">启用短信登录</span><span class="sxs-lookup"><span data-stu-id="a92bf-140">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="a92bf-141">无</span><span class="sxs-lookup"><span data-stu-id="a92bf-141">None</span></span>|<span data-ttu-id="a92bf-142">为用户启用短信登录。</span><span class="sxs-lookup"><span data-stu-id="a92bf-142">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="a92bf-143">属性</span><span class="sxs-lookup"><span data-stu-id="a92bf-143">Properties</span></span>

| <span data-ttu-id="a92bf-144">属性</span><span class="sxs-lookup"><span data-stu-id="a92bf-144">Property</span></span>     | <span data-ttu-id="a92bf-145">类型</span><span class="sxs-lookup"><span data-stu-id="a92bf-145">Type</span></span>        | <span data-ttu-id="a92bf-146">说明</span><span class="sxs-lookup"><span data-stu-id="a92bf-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a92bf-147">id</span><span class="sxs-lookup"><span data-stu-id="a92bf-147">id</span></span>|<span data-ttu-id="a92bf-148">String</span><span class="sxs-lookup"><span data-stu-id="a92bf-148">String</span></span>| <span data-ttu-id="a92bf-149">注册到此用户的此电话的标识符。</span><span class="sxs-lookup"><span data-stu-id="a92bf-149">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="a92bf-150">只读。</span><span class="sxs-lookup"><span data-stu-id="a92bf-150">Read-only.</span></span>|
|<span data-ttu-id="a92bf-151">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a92bf-151">phoneNumber</span></span>|<span data-ttu-id="a92bf-152">String</span><span class="sxs-lookup"><span data-stu-id="a92bf-152">String</span></span>|<span data-ttu-id="a92bf-153">发短信或呼叫进行身份验证的电话号码。</span><span class="sxs-lookup"><span data-stu-id="a92bf-153">The phone number to text or call for authentication.</span></span> <span data-ttu-id="a92bf-154">电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机是可选的。</span><span class="sxs-lookup"><span data-stu-id="a92bf-154">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="a92bf-155">例如，+1 5555551234 或 +1 5555551234x123 有效。</span><span class="sxs-lookup"><span data-stu-id="a92bf-155">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="a92bf-156">如果数字与所需格式不匹配，则创建/更新时将拒绝这些号码。</span><span class="sxs-lookup"><span data-stu-id="a92bf-156">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="a92bf-157">phoneType</span><span class="sxs-lookup"><span data-stu-id="a92bf-157">phoneType</span></span>|<span data-ttu-id="a92bf-158">string</span><span class="sxs-lookup"><span data-stu-id="a92bf-158">string</span></span>|<span data-ttu-id="a92bf-159">此电话的类型。</span><span class="sxs-lookup"><span data-stu-id="a92bf-159">The type of this phone.</span></span> <span data-ttu-id="a92bf-160">可能的值为： `mobile`、 `alternateMobile`或 `office`。</span><span class="sxs-lookup"><span data-stu-id="a92bf-160">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="a92bf-161">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="a92bf-161">smsSignInState</span></span>|<span data-ttu-id="a92bf-162">string</span><span class="sxs-lookup"><span data-stu-id="a92bf-162">string</span></span>|<span data-ttu-id="a92bf-163">电话是否已准备好用于短信登录。</span><span class="sxs-lookup"><span data-stu-id="a92bf-163">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="a92bf-164">可能的值是： `notSupported` `notAllowedByPolicy` 、 、 、 `notEnabled` 或 `phoneNumberNotUnique` `ready` `notConfigured` 。</span><span class="sxs-lookup"><span data-stu-id="a92bf-164">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a92bf-165">关系</span><span class="sxs-lookup"><span data-stu-id="a92bf-165">Relationships</span></span>

<span data-ttu-id="a92bf-166">无。</span><span class="sxs-lookup"><span data-stu-id="a92bf-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a92bf-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a92bf-167">JSON representation</span></span>

<span data-ttu-id="a92bf-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a92bf-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
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


