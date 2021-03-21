---
title: phoneAuthenticationMethod 资源类型
description: 注册到用户的电话的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0cab7a96923f49c77e6d160d68e8746530f8dcf2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964546"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="c1503-103">phoneAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1503-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="c1503-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1503-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1503-105">注册到用户的电话的表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1503-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="c1503-106">此资源包括电话号码、电话类型，以及是否将电话配置为允许用户通过短信登录。</span><span class="sxs-lookup"><span data-stu-id="c1503-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="c1503-107">电话有三种类型之一：移动、备用移动或办公室。</span><span class="sxs-lookup"><span data-stu-id="c1503-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="c1503-108">用户可以为每种类型注册一个号码，并且必须拥有移动电话才能添加备用移动电话。</span><span class="sxs-lookup"><span data-stu-id="c1503-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="c1503-109">当使用手机进行多重身份验证 (MFA) 或自助服务密码重置 (SSPR) 时，移动电话为默认值，备用移动电话为备份。</span><span class="sxs-lookup"><span data-stu-id="c1503-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="c1503-110">移动电话可用于短信和语音呼叫，具体取决于租户设置。</span><span class="sxs-lookup"><span data-stu-id="c1503-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="c1503-111">Office 电话只能接收语音呼叫，不能接收短信。</span><span class="sxs-lookup"><span data-stu-id="c1503-111">An office phone can only receive voice calls, not SMS messages.</span></span>

## <a name="methods"></a><span data-ttu-id="c1503-112">Methods</span><span class="sxs-lookup"><span data-stu-id="c1503-112">Methods</span></span>

| <span data-ttu-id="c1503-113">方法</span><span class="sxs-lookup"><span data-stu-id="c1503-113">Method</span></span>       | <span data-ttu-id="c1503-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1503-114">Return Type</span></span> | <span data-ttu-id="c1503-115">Description</span><span class="sxs-lookup"><span data-stu-id="c1503-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c1503-116">List</span><span class="sxs-lookup"><span data-stu-id="c1503-116">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="c1503-117">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1503-117">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="c1503-118">读取此用户的所有 phoneAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1503-118">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| [<span data-ttu-id="c1503-119">获取</span><span class="sxs-lookup"><span data-stu-id="c1503-119">Get</span></span>](../api/phoneauthenticationmethod-get.md) | [<span data-ttu-id="c1503-120">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1503-120">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="c1503-121">读取 phoneAuthenticationMethod 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1503-121">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="c1503-122">更新</span><span class="sxs-lookup"><span data-stu-id="c1503-122">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="c1503-123">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1503-123">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="c1503-124">更新 phoneAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="c1503-124">Update phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="c1503-125">删除</span><span class="sxs-lookup"><span data-stu-id="c1503-125">Delete</span></span>](../api/phoneauthenticationmethod-delete.md) | <span data-ttu-id="c1503-126">无</span><span class="sxs-lookup"><span data-stu-id="c1503-126">None</span></span> | <span data-ttu-id="c1503-127">删除 phoneAuthenticationMethod 对象。</span><span class="sxs-lookup"><span data-stu-id="c1503-127">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="c1503-128">禁用短信登录</span><span class="sxs-lookup"><span data-stu-id="c1503-128">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="c1503-129">无</span><span class="sxs-lookup"><span data-stu-id="c1503-129">None</span></span>|<span data-ttu-id="c1503-130">关闭用户的短信登录。</span><span class="sxs-lookup"><span data-stu-id="c1503-130">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="c1503-131">启用短信登录</span><span class="sxs-lookup"><span data-stu-id="c1503-131">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="c1503-132">无</span><span class="sxs-lookup"><span data-stu-id="c1503-132">None</span></span>|<span data-ttu-id="c1503-133">为用户启用短信登录。</span><span class="sxs-lookup"><span data-stu-id="c1503-133">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1503-134">属性</span><span class="sxs-lookup"><span data-stu-id="c1503-134">Properties</span></span>

| <span data-ttu-id="c1503-135">属性</span><span class="sxs-lookup"><span data-stu-id="c1503-135">Property</span></span>     | <span data-ttu-id="c1503-136">类型</span><span class="sxs-lookup"><span data-stu-id="c1503-136">Type</span></span>        | <span data-ttu-id="c1503-137">说明</span><span class="sxs-lookup"><span data-stu-id="c1503-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1503-138">id</span><span class="sxs-lookup"><span data-stu-id="c1503-138">id</span></span>|<span data-ttu-id="c1503-139">String</span><span class="sxs-lookup"><span data-stu-id="c1503-139">String</span></span>| <span data-ttu-id="c1503-140">注册到此用户的此电话的标识符。</span><span class="sxs-lookup"><span data-stu-id="c1503-140">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="c1503-141">只读。</span><span class="sxs-lookup"><span data-stu-id="c1503-141">Read-only.</span></span> <br/><br/><span data-ttu-id="c1503-142">id 的值是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="c1503-142">The value of id is one of the following:</span></span><ul><li><span data-ttu-id="c1503-143">`b6332ec1-7057-4abe-9331-3d72feddfe41` - 其中 **phoneType** 为 `alternateMobile` 。</span><span class="sxs-lookup"><span data-stu-id="c1503-143">`b6332ec1-7057-4abe-9331-3d72feddfe41` - where **phoneType** is `alternateMobile`.</span></span></li><li><span data-ttu-id="c1503-144">`e37fc753-ff3b-4958-9484-eaa9425c82bc` - 其中 **phoneType** 为 `office` 。</span><span class="sxs-lookup"><span data-stu-id="c1503-144">`e37fc753-ff3b-4958-9484-eaa9425c82bc` - where **phoneType** is `office`.</span></span></li><li><span data-ttu-id="c1503-145">`3179e48a-750b-4051-897c-87b9720928f7` - 其中 **phoneType** 为 `mobile` 。</span><span class="sxs-lookup"><span data-stu-id="c1503-145">`3179e48a-750b-4051-897c-87b9720928f7` - where **phoneType** is `mobile`.</span></span></li>|
|<span data-ttu-id="c1503-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c1503-146">phoneNumber</span></span>|<span data-ttu-id="c1503-147">String</span><span class="sxs-lookup"><span data-stu-id="c1503-147">String</span></span>|<span data-ttu-id="c1503-148">要发送文本或呼叫进行身份验证的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c1503-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="c1503-149">电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机号可选。</span><span class="sxs-lookup"><span data-stu-id="c1503-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="c1503-150">例如，+1 5555551234 或 +1 5555551234x123 有效。</span><span class="sxs-lookup"><span data-stu-id="c1503-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="c1503-151">如果数字与所需格式不匹配，则创建/更新时将拒绝数字。</span><span class="sxs-lookup"><span data-stu-id="c1503-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="c1503-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="c1503-152">phoneType</span></span>|<span data-ttu-id="c1503-153">authenticationPhoneType</span><span class="sxs-lookup"><span data-stu-id="c1503-153">authenticationPhoneType</span></span>|<span data-ttu-id="c1503-154">此电话的类型。</span><span class="sxs-lookup"><span data-stu-id="c1503-154">The type of this phone.</span></span> <span data-ttu-id="c1503-155">可能的值为： `mobile`、 `alternateMobile`或 `office`。</span><span class="sxs-lookup"><span data-stu-id="c1503-155">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="c1503-156">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="c1503-156">smsSignInState</span></span>|<span data-ttu-id="c1503-157">authenticationMethodSignInState</span><span class="sxs-lookup"><span data-stu-id="c1503-157">authenticationMethodSignInState</span></span>|<span data-ttu-id="c1503-158">电话是否可用于短信登录。</span><span class="sxs-lookup"><span data-stu-id="c1503-158">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="c1503-159">可能的值是 `notSupported` `notAllowedByPolicy` `notEnabled` ：、、、、 `phoneNumberNotUnique` `ready` 或 `notConfigured` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="c1503-159">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`, `unknownFutureValue`.</span></span>|

### <a name="smssigninstate-values"></a><span data-ttu-id="c1503-160">smsSignInState 值</span><span class="sxs-lookup"><span data-stu-id="c1503-160">smsSignInState values</span></span>

<span data-ttu-id="c1503-161">SMS 登录状态属性提供有关电话号码是否已准备好通过短信登录的信息。</span><span class="sxs-lookup"><span data-stu-id="c1503-161">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="c1503-162">以下是可能的值。</span><span class="sxs-lookup"><span data-stu-id="c1503-162">The following are the possible values.</span></span>

|<span data-ttu-id="c1503-163">值</span><span class="sxs-lookup"><span data-stu-id="c1503-163">Value</span></span>|<span data-ttu-id="c1503-164">说明</span><span class="sxs-lookup"><span data-stu-id="c1503-164">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="c1503-165">notSupported</span><span class="sxs-lookup"><span data-stu-id="c1503-165">notSupported</span></span>|<span data-ttu-id="c1503-166">此身份验证方法不支持主登录 - 例如，只能对用户的主移动电话号码（而非备用号码）启用登录。</span><span class="sxs-lookup"><span data-stu-id="c1503-166">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|<span data-ttu-id="c1503-167">notAllowedByPolicy</span><span class="sxs-lookup"><span data-stu-id="c1503-167">notAllowedByPolicy</span></span>|<span data-ttu-id="c1503-168">策略不启用此用户以将此方法用作主登录。</span><span class="sxs-lookup"><span data-stu-id="c1503-168">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|<span data-ttu-id="c1503-169">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c1503-169">notConfigured</span></span>|<span data-ttu-id="c1503-170">策略启用此用户以将此方法用作主登录，但需要执行其他操作来配置它。</span><span class="sxs-lookup"><span data-stu-id="c1503-170">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|<span data-ttu-id="c1503-171">phoneNumberNotUnique</span><span class="sxs-lookup"><span data-stu-id="c1503-171">phoneNumberNotUnique</span></span>|<span data-ttu-id="c1503-172">此用户尝试将电话号码设置为主登录，但该号码不是唯一的，不能用作登录名。</span><span class="sxs-lookup"><span data-stu-id="c1503-172">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|<span data-ttu-id="c1503-173">ready</span><span class="sxs-lookup"><span data-stu-id="c1503-173">ready</span></span>|<span data-ttu-id="c1503-174">此身份验证方法已做好在主登录中的使用准备。</span><span class="sxs-lookup"><span data-stu-id="c1503-174">This authentication method is ready for use in primary sign-in.</span></span>|
|<span data-ttu-id="c1503-175">notEnabled</span><span class="sxs-lookup"><span data-stu-id="c1503-175">notEnabled</span></span>|<span data-ttu-id="c1503-176">此登录方法未启用</span><span class="sxs-lookup"><span data-stu-id="c1503-176">This sign-in method is not enabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1503-177">关系</span><span class="sxs-lookup"><span data-stu-id="c1503-177">Relationships</span></span>

<span data-ttu-id="c1503-178">无。</span><span class="sxs-lookup"><span data-stu-id="c1503-178">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1503-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1503-179">JSON representation</span></span>

<span data-ttu-id="c1503-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1503-180">The following is a JSON representation of the resource.</span></span>

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


