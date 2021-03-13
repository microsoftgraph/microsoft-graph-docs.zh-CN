---
title: Microsoft Graph 身份验证方法 API 入门
description: Microsoft Graph 中的身份验证方法 API 使组织能够以编程方式管理其用户身份验证方法，从而使已注册用户能够执行多重身份验证 (MFA) 和自助服务密码重置 (SSPR)。
author: mmcla
localization_priority: Priority
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36385345141daa8dc782b64fa154ef97c46b3091
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761449"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a><span data-ttu-id="1cf3e-103">Microsoft Graph 身份验证方法 API 入门</span><span class="sxs-lookup"><span data-stu-id="1cf3e-103">Get started with the Microsoft Graph authentication methods API</span></span>

<span data-ttu-id="1cf3e-104">[身份验证方法](/azure/active-directory/authentication/concept-authentication-methods) 是用户在 Azure Active Directory (Azure AD) 中的身份验证方式。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-104">[Authentication methods](/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1cf3e-105">Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-105">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="1cf3e-106">身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-106">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="1cf3e-107">可使用身份验证方法 API 来管理用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-107">You can use the authentication method APIs to manage a user's authentication methods.</span></span> <span data-ttu-id="1cf3e-108">例如，你能够：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-108">For example, you can:</span></span>

* <span data-ttu-id="1cf3e-109">为用户添加一个电话号码，通过策略启用短信和语音呼叫身份验证后，该用户即可使用该号码进行此类身份验证</span><span class="sxs-lookup"><span data-stu-id="1cf3e-109">Add a phone number for a user, who can then use that number for SMS and voice call authentication if they're enabled to use it by policy</span></span>
* <span data-ttu-id="1cf3e-110">更新或删除分配给用户的电话号码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-110">Update or delete the phone number assigned to a user</span></span>
* <span data-ttu-id="1cf3e-111">启用或禁用用于短信登录的号码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-111">Enable or disable the number for SMS sign-in</span></span>
* <span data-ttu-id="1cf3e-112">重置用户密码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-112">Reset a user's password</span></span>

<span data-ttu-id="1cf3e-113">API 是用于管理用户身份验证方法的一种关键工具。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-113">The APIs are a key tool to manage your users' authentication methods.</span></span>

<span data-ttu-id="1cf3e-114">在本教程中，你将学习如何：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-114">In this tutorial, you'll learn how to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="1cf3e-115">使用正确的角色和权限对 Azure AD 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="1cf3e-115">Authenticate to Azure AD with the right roles and permissions</span></span>
> * <span data-ttu-id="1cf3e-116">检查用户的身份验证方法</span><span class="sxs-lookup"><span data-stu-id="1cf3e-116">Check the user's authentication methods</span></span>
> * <span data-ttu-id="1cf3e-117">为用户添加新的电话号码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-117">Add new phone numbers for the user</span></span>
> * <span data-ttu-id="1cf3e-118">删除用户的电话号码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-118">Remove a phone number from the user</span></span>
> * <span data-ttu-id="1cf3e-119">重置用户密码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-119">Reset the user's password</span></span>

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a><span data-ttu-id="1cf3e-120">步骤 1：使用正确的角色和权限对 Azure AD 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="1cf3e-120">Step 1: Authenticate to Azure AD with the right roles and permissions</span></span>

<span data-ttu-id="1cf3e-121">使用你喜欢的[工具与 Microsoft Graph 交互](use-the-api.md#tools-for-interacting-with-microsoft-graph)，使用具有以下一种角色的帐户登录：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-121">Using your favorite [tool for interacting with Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), sign in using an account with one of these roles:</span></span>

* <span data-ttu-id="1cf3e-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1cf3e-122">Global administrator</span></span>
* <span data-ttu-id="1cf3e-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="1cf3e-123">Privileged authentication administrator</span></span>
* <span data-ttu-id="1cf3e-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="1cf3e-124">Authentication administrator</span></span>

<span data-ttu-id="1cf3e-125">接下来，修改你的权限。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-125">Next, modify your permissions.</span></span> <span data-ttu-id="1cf3e-126">在本教程中，我们将使用 [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview)，因此，请确保已在 Graph 浏览器或你的应用中启用此权限。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-126">We'll use [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) for this tutorial, so make sure it's enabled in Graph Explorer or your app.</span></span>

<span data-ttu-id="1cf3e-127">分配范围并获得同意后，即可开始使用 API。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-127">Once the scope is assigned and consented, you can start using the API.</span></span> <span data-ttu-id="1cf3e-128">此处的示例使用名为 Avery Howard 的标准用户。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-128">The examples here use a standard user named Avery Howard.</span></span> <span data-ttu-id="1cf3e-129">您应该使用现有的测试帐户，或按照[这些说明](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user)创建一个新的测试帐户。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-129">You should use a preexisting test account or create a new one following [these instructions](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span></span> <span data-ttu-id="1cf3e-130">这些 API 是实时的，因此请不要在实际用户上对其进行测试。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-130">These APIs are live so don't test them on real users.</span></span>

## <a name="step-2-check-the-users-authentication-methods"></a><span data-ttu-id="1cf3e-131">步骤 2：检查用户的身份验证方法</span><span class="sxs-lookup"><span data-stu-id="1cf3e-131">Step 2: Check the user's authentication methods</span></span>

<span data-ttu-id="1cf3e-132">拨打电话，以查看用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-132">Make a call to see the user's authentication methods.</span></span> <span data-ttu-id="1cf3e-133">获取 URL 以查看用户的个人资料并添加 `/authentication/methods`：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-133">Take the URL to see a user's profile and add `/authentication/methods`:</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-134">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="1cf3e-135">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-135">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

## <a name="step-3-add-new-phone-numbers-for-the-user"></a><span data-ttu-id="1cf3e-136">步骤 3：为用户添加新的电话号码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-136">Step 3: Add new phone numbers for the user</span></span>

<span data-ttu-id="1cf3e-137">在上一步中，新用户 (Avery) 仅注册了密码。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-137">From the previous step, a new user (Avery) only has a password registered.</span></span> <span data-ttu-id="1cf3e-138">若要分配新的电话号码供 Avery 使用，请在正文中使用电话类型和号码发出 `POST` 请求。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-138">To assign a new phone number for Avery to use, make a `POST` request with the phone type and number in the body.</span></span> <span data-ttu-id="1cf3e-139">若要告知系统正在添加电话号码，还需要将 URL 的末尾从 `methods` 更改为 `phoneMethods`。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-139">To tell the system that a phone number is being added, you'll also need to change the end of the URL from `methods` to `phoneMethods`.</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-140">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-140">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "mobile",
    "phoneNumber": "+1 2065550123"
}
```

### <a name="response"></a><span data-ttu-id="1cf3e-141">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-141">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

<span data-ttu-id="1cf3e-142">要添加 Avery 的办公室号码，你将再次`POST`访问相同的 URL，但要更新电话类型和电话号码：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-142">To add Avery's office number, you'll `POST` again to the same URL but update the phone type and number:</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-143">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-143">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "office",
    "phoneNumber": "+1 4255550199"
}
```

### <a name="response"></a><span data-ttu-id="1cf3e-144">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-144">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

<span data-ttu-id="1cf3e-145">对电话方法 URL 再执行一次 `GET`，以查看 Avery 的所有电话号码：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-145">Do one more `GET` to the phone methods URL to see all of Avery's phone numbers:</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-146">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-146">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a><span data-ttu-id="1cf3e-147">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-147">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods",
    "value": [
        {
            "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
            "phoneNumber": "+1 4255550199",
            "phoneType": "office",
            "smsSignInState": "notSupported"
        },
        {
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        }
    ]
}
```

<span data-ttu-id="1cf3e-148">确认你可以按预期看到这两个号码。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-148">Confirm that you can see both numbers as expected.</span></span>

## <a name="step-4-remove-a-phone-number-from-the-user"></a><span data-ttu-id="1cf3e-149">步骤 4：删除用户的电话号码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-149">Step 4: Remove a phone number from the user</span></span>

<span data-ttu-id="1cf3e-150">在本场景中，Avery 现在在家工作，你需要从他们的帐户中删除他们的办公室号码。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-150">In this scenario, Avery is now working from home you need to remove their office number from their account.</span></span> <span data-ttu-id="1cf3e-151">需要在办公室电话 URL 上呼叫 `DELETE`，可以通过将办公室电话的 ID 附加到电话方法 URL 来创建办公室电话 URL。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-151">You need to call `DELETE` on the office phone URL, which you can create by appending the office phone's ID to the phone methods URL.</span></span> <span data-ttu-id="1cf3e-152">查看上面的 Avery 电话列表：办公室电话 ID 以“e37f”开头。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-152">Look at Avery's list of phones above: the office phone ID starts with "e37f".</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-153">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-153">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

<span data-ttu-id="1cf3e-154">响应中没有数据，因为没有更多符合预期的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-154">There's no data in the response because there's no more office phone as intended.</span></span> <span data-ttu-id="1cf3e-155">可通过查看 Avery 的所有方法来确认它已删除，与之前的发出的 `GET` 相同：</span><span class="sxs-lookup"><span data-stu-id="1cf3e-155">You can confirm it's gone by looking at all of Avery's methods, which is the same `GET` that was made previously:</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-156">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-156">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="1cf3e-157">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-157">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        },
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

<span data-ttu-id="1cf3e-158">正如预期的那样，用户现在又回到只有一部手机和一个密码的状态。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-158">As expected, the user is now back to only having one mobile phone and a password.</span></span>

## <a name="step-5-reset-the-users-password"></a><span data-ttu-id="1cf3e-159">步骤 5：重置用户密码</span><span class="sxs-lookup"><span data-stu-id="1cf3e-159">Step 5: Reset the user's password</span></span>

<span data-ttu-id="1cf3e-160">在此场景中，Avery 忘记了密码，你需要为他们重置。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-160">In this scenario, Avery has forgotten their password and you need to reset it for them.</span></span> <span data-ttu-id="1cf3e-161">若要重置密码，你需要向其密码的 URL 发出 `POST`（请查看 Avery 身份验证方法列表中以“28c1”开头的 ID），并指定“resetPassword”操作。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-161">To reset, you'll make a `POST` to their password's URL (see the ID starting with "28c1" above in Avery's list of authentication methods), specifying the "resetPassword" action.</span></span> <span data-ttu-id="1cf3e-162">在请求正文中提供新密码。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-162">Provide the new password in the request body.</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-163">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a><span data-ttu-id="1cf3e-164">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-164">Response</span></span>

``` http
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

<span data-ttu-id="1cf3e-165">由于这是将密码向下同步到租户的本地基础结构中的 Active Directory，可能需要几分钟，因此你有一个可以查看其是否完整的地址。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-165">Because this is syncing the password down to Active Directory in the tenant's on-prem infrastructure, it might take a few minutes, so you have an address where you can check to see if it's complete.</span></span> <span data-ttu-id="1cf3e-166">此地址位于响应的位置标头中，可查看该 URL 上的 `GET` 状态。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-166">This address is in the location header of the response, and to see the status do a `GET` on that URL.</span></span>

### <a name="request"></a><span data-ttu-id="1cf3e-167">请求</span><span class="sxs-lookup"><span data-stu-id="1cf3e-167">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a><span data-ttu-id="1cf3e-168">响应</span><span class="sxs-lookup"><span data-stu-id="1cf3e-168">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ed178e23-7447-4892-baf8-fc46f8af26ce')/authentication/operations/$entity",
    "id": "74bfa1a6-c0e0-4957-8c37-f91048f4959e",
    "createdDateTime": "2020-05-14T00:23:40Z",
    "lastActionDateTime": "2020-05-14T00:23:41Z",
    "status": "succeeded",
    "statusDetail": "ResetSuccess",
    "resourceLocation": "https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/methods/28c10230-6103-485e-b985-444c60001490"
}
```

<span data-ttu-id="1cf3e-169">成功！</span><span class="sxs-lookup"><span data-stu-id="1cf3e-169">And success!</span></span> <span data-ttu-id="1cf3e-170">你已经演练了查看用户个人资料、查看用户的身份验证方法、添加和删除电话号码以及重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-170">You've walked through seeing a user's profile, their auth methods, adding and removing phone numbers, and resetting their password.</span></span> <span data-ttu-id="1cf3e-171">现在可以开始管理自己用户的方法了。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-171">Now you're ready to go manage your own users' methods.</span></span>

## <a name="api-reference"></a><span data-ttu-id="1cf3e-172">API 参考</span><span class="sxs-lookup"><span data-stu-id="1cf3e-172">API reference</span></span>

<span data-ttu-id="1cf3e-173">在查找身份验证方法的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="1cf3e-173">Looking for the API reference for authentication methods?</span></span>

* <span data-ttu-id="1cf3e-174">请参阅 [Azure AD 身份验证方法 API 概述](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="1cf3e-174">See [Azure AD authentication methods API overview](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span></span>

## <a name="next-steps"></a><span data-ttu-id="1cf3e-175">后续步骤</span><span class="sxs-lookup"><span data-stu-id="1cf3e-175">Next steps</span></span>

* <span data-ttu-id="1cf3e-176">了解如何[使用身份验证方法 REST API](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-176">Find out how to [use the authentication method REST APIs](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span></span>
* <span data-ttu-id="1cf3e-177">使用 Azure AD 对 Microsoft Graph [进行身份验证](./auth/index.yml)。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-177">Use Azure AD to [authenticate](./auth/index.yml) to Microsoft Graph.</span></span>
* <span data-ttu-id="1cf3e-178">将 [Azure AD 登录](https://azure.microsoft.com/develop/identity/signin/)集成到应用或网站中。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-178">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
* <span data-ttu-id="1cf3e-179">有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-179">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
* <span data-ttu-id="1cf3e-180">浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。</span><span class="sxs-lookup"><span data-stu-id="1cf3e-180">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>