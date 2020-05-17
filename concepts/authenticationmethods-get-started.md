---
title: Microsoft Graph 身份验证方法 API 入门
description: Microsoft Graph 中的身份验证方法 API 使组织能够以编程方式管理其用户的身份验证方法，从而获得注册了多重身份验证（MFA）和自助服务密码重置（SSPR）的用户。
author: mmcla
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8f08ae59f7a2ad0e16c4fc0c3af5637bcbfaaca
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272807"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a><span data-ttu-id="034bc-103">Microsoft Graph 身份验证方法 API 入门</span><span class="sxs-lookup"><span data-stu-id="034bc-103">Get started with the Microsoft Graph authentication methods API</span></span>

<span data-ttu-id="034bc-104">[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)是用户在 Azure Active Directory （azure AD）中进行身份验证的方法。</span><span class="sxs-lookup"><span data-stu-id="034bc-104">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="034bc-105">Azure AD 中的身份验证方法包括密码和电话（例如，SMS 和语音呼叫），这些方法可在 Microsoft Graph 中进行管理，如 FIDO2 安全密钥和 Microsoft 身份验证器应用等许多其他内容。</span><span class="sxs-lookup"><span data-stu-id="034bc-105">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="034bc-106">身份验证方法在主要、第二因素和分步身份验证以及自助密码重置（SSPR）过程中也使用。</span><span class="sxs-lookup"><span data-stu-id="034bc-106">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="034bc-107">您可以使用身份验证方法 Api 来管理用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="034bc-107">You can use the authentication method APIs to manage a user's authentication methods.</span></span> <span data-ttu-id="034bc-108">例如，你能够：</span><span class="sxs-lookup"><span data-stu-id="034bc-108">For example, you can:</span></span>

* <span data-ttu-id="034bc-109">为用户添加电话号码，如果启用这些号码，则该号码可在策略中使用该号码进行短信和语音呼叫身份验证</span><span class="sxs-lookup"><span data-stu-id="034bc-109">Add a phone number for a user, who can then use that number for SMS and voice call authentication if they're enabled to use it by policy</span></span>
* <span data-ttu-id="034bc-110">更新或删除分配给用户的电话号码</span><span class="sxs-lookup"><span data-stu-id="034bc-110">Update or delete the phone number assigned to a user</span></span>
* <span data-ttu-id="034bc-111">启用或禁用 SMS 登录号码</span><span class="sxs-lookup"><span data-stu-id="034bc-111">Enable or disable the number for SMS sign-in</span></span>
* <span data-ttu-id="034bc-112">重置用户密码</span><span class="sxs-lookup"><span data-stu-id="034bc-112">Reset a user's password</span></span>

<span data-ttu-id="034bc-113">Api 是管理用户的身份验证方法的主要工具。</span><span class="sxs-lookup"><span data-stu-id="034bc-113">The APIs are a key tool to manage your users' authentication methods.</span></span>

<span data-ttu-id="034bc-114">在本教程中，你将了解如何执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="034bc-114">In this tutorial, you'll learn how to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="034bc-115">使用正确的角色和权限向 Azure AD 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="034bc-115">Authenticate to Azure AD with the right roles and permissions</span></span>
> * <span data-ttu-id="034bc-116">检查用户的身份验证方法</span><span class="sxs-lookup"><span data-stu-id="034bc-116">Check the user's authentication methods</span></span>
> * <span data-ttu-id="034bc-117">为用户添加新电话号码</span><span class="sxs-lookup"><span data-stu-id="034bc-117">Add new phone numbers for the user</span></span>
> * <span data-ttu-id="034bc-118">从用户中删除电话号码</span><span class="sxs-lookup"><span data-stu-id="034bc-118">Remove a phone number from the user</span></span>
> * <span data-ttu-id="034bc-119">重置用户的密码</span><span class="sxs-lookup"><span data-stu-id="034bc-119">Reset the user's password</span></span>

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a><span data-ttu-id="034bc-120">步骤1：使用正确的角色和权限向 Azure AD 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="034bc-120">Step 1: Authenticate to Azure AD with the right roles and permissions</span></span>

<span data-ttu-id="034bc-121">使用您喜爱的[工具与 Microsoft Graph 交互](use-the-api.md#tools-for-interacting-with-microsoft-graph)，使用具有以下角色之一的帐户登录：</span><span class="sxs-lookup"><span data-stu-id="034bc-121">Using your favorite [tool for interacting with Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), sign in using an account with one of these roles:</span></span>

* <span data-ttu-id="034bc-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="034bc-122">Global administrator</span></span>
* <span data-ttu-id="034bc-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="034bc-123">Privileged authentication administrator</span></span>
* <span data-ttu-id="034bc-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="034bc-124">Authentication administrator</span></span>

<span data-ttu-id="034bc-125">接下来，修改您的权限。</span><span class="sxs-lookup"><span data-stu-id="034bc-125">Next, modify your permissions.</span></span> <span data-ttu-id="034bc-126">我们将使用[UserAuthenticationMethod](permissions-reference.md#user-authentication-method-permissions-preview) ，以确保在 Graph 资源管理器或你的应用程序中启用了此教程。</span><span class="sxs-lookup"><span data-stu-id="034bc-126">We'll use [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) for this tutorial, so make sure it's enabled in Graph Explorer or your app.</span></span>

<span data-ttu-id="034bc-127">在分配并许可范围后，即可开始使用 API。</span><span class="sxs-lookup"><span data-stu-id="034bc-127">Once the scope is assigned and consented, you can start using the API.</span></span> <span data-ttu-id="034bc-128">此处的示例使用名为 "Avery Howard" 的标准用户。</span><span class="sxs-lookup"><span data-stu-id="034bc-128">The examples here use a standard user named Avery Howard.</span></span> <span data-ttu-id="034bc-129">应使用预先存在的测试帐户，或按照[这些说明](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user)创建一个新的测试帐户。</span><span class="sxs-lookup"><span data-stu-id="034bc-129">You should use a preexisting test account or create a new one following [these instructions](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span></span> <span data-ttu-id="034bc-130">这些 Api 是实时的，因此不会对真实用户进行测试。</span><span class="sxs-lookup"><span data-stu-id="034bc-130">These APIs are live so don't test them on real users.</span></span>

## <a name="step-2-check-the-users-authentication-methods"></a><span data-ttu-id="034bc-131">步骤2：检查用户的身份验证方法</span><span class="sxs-lookup"><span data-stu-id="034bc-131">Step 2: Check the user's authentication methods</span></span>

<span data-ttu-id="034bc-132">打电话以查看用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="034bc-132">Make a call to see the user's authentication methods.</span></span> <span data-ttu-id="034bc-133">获取 URL 以查看用户的配置文件并添加 `/authentication/methods` ：</span><span class="sxs-lookup"><span data-stu-id="034bc-133">Take the URL to see a user's profile and add `/authentication/methods`:</span></span>

### <a name="request"></a><span data-ttu-id="034bc-134">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="034bc-135">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-135">Response</span></span>

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

## <a name="step-3-add-new-phone-numbers-for-the-user"></a><span data-ttu-id="034bc-136">步骤3：为用户添加新电话号码</span><span class="sxs-lookup"><span data-stu-id="034bc-136">Step 3: Add new phone numbers for the user</span></span>

<span data-ttu-id="034bc-137">在上一步中，新用户（Avery）仅注册了密码。</span><span class="sxs-lookup"><span data-stu-id="034bc-137">From the previous step, a new user (Avery) only has a password registered.</span></span> <span data-ttu-id="034bc-138">若要将新电话号码分配给 Avery 以供使用，请 `POST` 在正文中使用电话类型和号码发出请求。</span><span class="sxs-lookup"><span data-stu-id="034bc-138">To assign a new phone number for Avery to use, make a `POST` request with the phone type and number in the body.</span></span> <span data-ttu-id="034bc-139">若要告知系统正在添加的电话号码，您还需要将 URL 的结束值从更改 `methods` 为 `phoneMethods` 。</span><span class="sxs-lookup"><span data-stu-id="034bc-139">To tell the system that a phone number is being added, you'll also need to change the end of the URL from `methods` to `phoneMethods`.</span></span>

### <a name="request"></a><span data-ttu-id="034bc-140">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-140">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="034bc-141">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-141">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

<span data-ttu-id="034bc-142">若要添加 Avery 的办公室号码，您将 `POST` 再次指向相同的 URL，但会更新电话类型和号码：</span><span class="sxs-lookup"><span data-stu-id="034bc-142">To add Avery's office number, you'll `POST` again to the same URL but update the phone type and number:</span></span>

### <a name="request"></a><span data-ttu-id="034bc-143">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-143">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="034bc-144">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-144">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

<span data-ttu-id="034bc-145">对电话方法 URL 执行更多操作 `GET` ，以查看所有 Avery 的电话号码：</span><span class="sxs-lookup"><span data-stu-id="034bc-145">Do one more `GET` to the phone methods URL to see all of Avery's phone numbers:</span></span>

### <a name="request"></a><span data-ttu-id="034bc-146">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-146">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a><span data-ttu-id="034bc-147">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-147">Response</span></span>

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

<span data-ttu-id="034bc-148">确认您可以按预期看到两个数字。</span><span class="sxs-lookup"><span data-stu-id="034bc-148">Confirm that you can see both numbers as expected.</span></span>

## <a name="step-4-remove-a-phone-number-from-the-user"></a><span data-ttu-id="034bc-149">步骤4：从用户中删除电话号码</span><span class="sxs-lookup"><span data-stu-id="034bc-149">Step 4: Remove a phone number from the user</span></span>

<span data-ttu-id="034bc-150">在这种情况下，Avery 现在在家工作，您需要从其帐户中删除其办公室号码。</span><span class="sxs-lookup"><span data-stu-id="034bc-150">In this scenario, Avery is now working from home you need to remove their office number from their account.</span></span> <span data-ttu-id="034bc-151">您需要通过将 `DELETE` office PHONE ID 追加到电话方法 url 来创建 office 电话 url。</span><span class="sxs-lookup"><span data-stu-id="034bc-151">You need to call `DELETE` on the office phone URL, which you can create by appending the office phone's ID to the phone methods URL.</span></span> <span data-ttu-id="034bc-152">查看上 Avery 的手机列表： office 电话 ID 以 "e37f" 开头。</span><span class="sxs-lookup"><span data-stu-id="034bc-152">Look at Avery's list of phones above: the office phone ID starts with "e37f".</span></span>

### <a name="request"></a><span data-ttu-id="034bc-153">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-153">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

<span data-ttu-id="034bc-154">由于没有其他需要的办公室电话，响应中没有数据。</span><span class="sxs-lookup"><span data-stu-id="034bc-154">There's no data in the response because there's no more office phone as intended.</span></span> <span data-ttu-id="034bc-155">您可以通过查看所有 Avery 的方法来确认它是否已消失，这与 `GET` 之前所做的完全相同：</span><span class="sxs-lookup"><span data-stu-id="034bc-155">You can confirm it's gone by looking at all of Avery's methods, which is the same `GET` that was made previously:</span></span>

### <a name="request"></a><span data-ttu-id="034bc-156">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-156">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="034bc-157">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-157">Response</span></span>

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

<span data-ttu-id="034bc-158">正如预期一样，用户现在可以返回到仅拥有一个移动电话和一个密码。</span><span class="sxs-lookup"><span data-stu-id="034bc-158">As expected, the user is now back to only having one mobile phone and a password.</span></span>

## <a name="step-5-reset-the-users-password"></a><span data-ttu-id="034bc-159">步骤5：重置用户的密码</span><span class="sxs-lookup"><span data-stu-id="034bc-159">Step 5: Reset the user's password</span></span>

<span data-ttu-id="034bc-160">在这种情况下，Avery 忘记了密码，你需要为其重置。</span><span class="sxs-lookup"><span data-stu-id="034bc-160">In this scenario, Avery has forgotten their password and you need to reset it for them.</span></span> <span data-ttu-id="034bc-161">若要重置，您将 `POST` 为其密码的 URL （请参阅在 Avery 的身份验证方法列表中以 "28c1" 开头的 ID），并指定 "resetPassword" 操作。</span><span class="sxs-lookup"><span data-stu-id="034bc-161">To reset, you'll make a `POST` to their password's URL (see the ID starting with "28c1" above in Avery's list of authentication methods), specifying the "resetPassword" action.</span></span> <span data-ttu-id="034bc-162">在请求正文中提供新密码。</span><span class="sxs-lookup"><span data-stu-id="034bc-162">Provide the new password in the request body.</span></span>

### <a name="request"></a><span data-ttu-id="034bc-163">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a><span data-ttu-id="034bc-164">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-164">Response</span></span>

```
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

<span data-ttu-id="034bc-165">由于这会将密码同步到租户的本地基础结构中的 Active Directory，因此可能需要几分钟时间，因此您有一个地址，您可以在其中查看它是否已完成。</span><span class="sxs-lookup"><span data-stu-id="034bc-165">Because this is syncing the password down to Active Directory in the tenant's on-prem infrastructure, it might take a few minutes, so you have an address where you can check to see if it's complete.</span></span> <span data-ttu-id="034bc-166">此地址位于响应的位置标头中，可查看该 URL 上的状态 do `GET` 。</span><span class="sxs-lookup"><span data-stu-id="034bc-166">This address is in the location header of the response, and to see the status do a `GET` on that URL.</span></span>

### <a name="request"></a><span data-ttu-id="034bc-167">请求</span><span class="sxs-lookup"><span data-stu-id="034bc-167">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a><span data-ttu-id="034bc-168">响应</span><span class="sxs-lookup"><span data-stu-id="034bc-168">Response</span></span>

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

<span data-ttu-id="034bc-169">和成功！</span><span class="sxs-lookup"><span data-stu-id="034bc-169">And success!</span></span> <span data-ttu-id="034bc-170">您已完成查看用户的配置文件、其身份验证方法、添加和删除电话号码以及重置其密码。</span><span class="sxs-lookup"><span data-stu-id="034bc-170">You've walked through seeing a user's profile, their auth methods, adding and removing phone numbers, and resetting their password.</span></span> <span data-ttu-id="034bc-171">现在，你可以开始管理自己的用户的方法。</span><span class="sxs-lookup"><span data-stu-id="034bc-171">Now you're ready to go manage your own users' methods.</span></span>

## <a name="api-reference"></a><span data-ttu-id="034bc-172">API 参考</span><span class="sxs-lookup"><span data-stu-id="034bc-172">API reference</span></span>

<span data-ttu-id="034bc-173">查找身份验证方法的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="034bc-173">Looking for the API reference for authentication methods?</span></span>

* <span data-ttu-id="034bc-174">请参阅[AZURE AD 身份验证方法 API 概述](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="034bc-174">See [Azure AD authentication methods API overview](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span></span>

## <a name="next-steps"></a><span data-ttu-id="034bc-175">后续步骤</span><span class="sxs-lookup"><span data-stu-id="034bc-175">Next steps</span></span>

* <span data-ttu-id="034bc-176">了解如何[使用身份验证方法 REST api](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="034bc-176">Find out how to [use the authentication method REST APIs](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span></span>
* <span data-ttu-id="034bc-177">使用 Azure AD 对 Microsoft Graph [进行身份验证](/graph/auth)。</span><span class="sxs-lookup"><span data-stu-id="034bc-177">Use Azure AD to [authenticate](/graph/auth) to Microsoft Graph.</span></span>
* <span data-ttu-id="034bc-178">将 [Azure AD 登录](https://azure.microsoft.com/develop/identity/signin/)集成到应用或网站中。</span><span class="sxs-lookup"><span data-stu-id="034bc-178">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
* <span data-ttu-id="034bc-179">有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="034bc-179">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
* <span data-ttu-id="034bc-180">浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。</span><span class="sxs-lookup"><span data-stu-id="034bc-180">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
