---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0aef89c30fc67132352d9d70f9b0fc56e3a9063e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508903"
---
# <a name="update-user"></a><span data-ttu-id="e15d4-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="e15d4-103">Update user</span></span>

<span data-ttu-id="e15d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e15d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e15d4-105">更新 user 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e15d4-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e15d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="e15d4-106">Permissions</span></span>
<span data-ttu-id="e15d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e15d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e15d4-109">Permission type</span></span>      | <span data-ttu-id="e15d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e15d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e15d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e15d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e15d4-112">User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e15d4-112">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e15d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e15d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e15d4-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e15d4-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="e15d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e15d4-115">Application</span></span> | <span data-ttu-id="e15d4-116">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15d4-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="e15d4-117">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="e15d4-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="e15d4-118">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="e15d4-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="e15d4-119">有关详细信息，请参阅 [Azure AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="e15d4-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="e15d4-120">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="e15d4-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="e15d4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e15d4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="e15d4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e15d4-122">Request headers</span></span>
| <span data-ttu-id="e15d4-123">标头</span><span class="sxs-lookup"><span data-stu-id="e15d4-123">Header</span></span>       | <span data-ttu-id="e15d4-124">值</span><span class="sxs-lookup"><span data-stu-id="e15d4-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e15d4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e15d4-125">Authorization</span></span>  | <span data-ttu-id="e15d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e15d4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e15d4-128">Content-Type</span></span>  | <span data-ttu-id="e15d4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e15d4-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e15d4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e15d4-130">Request body</span></span>
<span data-ttu-id="e15d4-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e15d4-134">属性</span><span class="sxs-lookup"><span data-stu-id="e15d4-134">Property</span></span>     | <span data-ttu-id="e15d4-135">类型</span><span class="sxs-lookup"><span data-stu-id="e15d4-135">Type</span></span>   |<span data-ttu-id="e15d4-136">说明</span><span class="sxs-lookup"><span data-stu-id="e15d4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e15d4-137">aboutMe</span><span class="sxs-lookup"><span data-stu-id="e15d4-137">aboutMe</span></span>|<span data-ttu-id="e15d4-138">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-138">String</span></span>|<span data-ttu-id="e15d4-139">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="e15d4-139">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="e15d4-140">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e15d4-140">accountEnabled</span></span>|<span data-ttu-id="e15d4-141">布尔</span><span class="sxs-lookup"><span data-stu-id="e15d4-141">Boolean</span></span>| <span data-ttu-id="e15d4-142">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="e15d4-142">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="e15d4-143">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="e15d4-143">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="e15d4-144">birthday</span><span class="sxs-lookup"><span data-stu-id="e15d4-144">birthday</span></span>|<span data-ttu-id="e15d4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e15d4-145">DateTimeOffset</span></span>|<span data-ttu-id="e15d4-p106">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e15d4-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e15d4-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="e15d4-149">businessPhones</span></span>| <span data-ttu-id="e15d4-150">String collection</span><span class="sxs-lookup"><span data-stu-id="e15d4-150">String collection</span></span> | <span data-ttu-id="e15d4-p107">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="e15d4-153">城市</span><span class="sxs-lookup"><span data-stu-id="e15d4-153">city</span></span>|<span data-ttu-id="e15d4-154">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-154">String</span></span>|<span data-ttu-id="e15d4-155">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="e15d4-155">The city in which the user is located.</span></span>|
|<span data-ttu-id="e15d4-156">country</span><span class="sxs-lookup"><span data-stu-id="e15d4-156">country</span></span>|<span data-ttu-id="e15d4-157">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-157">String</span></span>|<span data-ttu-id="e15d4-158">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="e15d4-158">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="e15d4-159">department</span><span class="sxs-lookup"><span data-stu-id="e15d4-159">department</span></span>|<span data-ttu-id="e15d4-160">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-160">String</span></span>|<span data-ttu-id="e15d4-161">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="e15d4-161">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="e15d4-162">displayName</span><span class="sxs-lookup"><span data-stu-id="e15d4-162">displayName</span></span>|<span data-ttu-id="e15d4-163">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-163">String</span></span>|<span data-ttu-id="e15d4-p108">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="e15d4-168">givenName</span><span class="sxs-lookup"><span data-stu-id="e15d4-168">givenName</span></span>|<span data-ttu-id="e15d4-169">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-169">String</span></span>|<span data-ttu-id="e15d4-170">用户的名。</span><span class="sxs-lookup"><span data-stu-id="e15d4-170">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="e15d4-171">hireDate</span><span class="sxs-lookup"><span data-stu-id="e15d4-171">hireDate</span></span>|<span data-ttu-id="e15d4-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e15d4-172">DateTimeOffset</span></span>|<span data-ttu-id="e15d4-p109">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e15d4-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e15d4-176">interests</span><span class="sxs-lookup"><span data-stu-id="e15d4-176">interests</span></span>|<span data-ttu-id="e15d4-177">String collection</span><span class="sxs-lookup"><span data-stu-id="e15d4-177">String collection</span></span>|<span data-ttu-id="e15d4-178">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="e15d4-178">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="e15d4-179">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e15d4-179">jobTitle</span></span>|<span data-ttu-id="e15d4-180">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-180">String</span></span>|<span data-ttu-id="e15d4-181">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="e15d4-181">The user’s job title.</span></span>|
|<span data-ttu-id="e15d4-182">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e15d4-182">mailNickname</span></span>|<span data-ttu-id="e15d4-183">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-183">String</span></span>|<span data-ttu-id="e15d4-184">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="e15d4-184">The mail alias for the user.</span></span> <span data-ttu-id="e15d4-185">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="e15d4-185">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="e15d4-186">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e15d4-186">mobilePhone</span></span>|<span data-ttu-id="e15d4-187">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-187">String</span></span>|<span data-ttu-id="e15d4-188">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="e15d4-188">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="e15d4-189">mySite</span><span class="sxs-lookup"><span data-stu-id="e15d4-189">mySite</span></span>|<span data-ttu-id="e15d4-190">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-190">String</span></span>|<span data-ttu-id="e15d4-191">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="e15d4-191">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="e15d4-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e15d4-192">officeLocation</span></span>|<span data-ttu-id="e15d4-193">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-193">String</span></span>|<span data-ttu-id="e15d4-194">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="e15d4-194">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="e15d4-195">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="e15d4-195">onPremisesImmutableId</span></span>|<span data-ttu-id="e15d4-196">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-196">String</span></span>|<span data-ttu-id="e15d4-197">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="e15d4-197">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="e15d4-198">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="e15d4-198">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="e15d4-199">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="e15d4-199">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="e15d4-200">otherMails</span><span class="sxs-lookup"><span data-stu-id="e15d4-200">otherMails</span></span>|<span data-ttu-id="e15d4-201">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-201">String</span></span> |<span data-ttu-id="e15d4-202">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="e15d4-202">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="e15d4-203">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="e15d4-203">passwordPolicies</span></span>|<span data-ttu-id="e15d4-204">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-204">String</span></span>|<span data-ttu-id="e15d4-p112">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="e15d4-209">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e15d4-209">passwordProfile</span></span>|[<span data-ttu-id="e15d4-210">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="e15d4-210">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="e15d4-p113">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="e15d4-216">pastProjects</span><span class="sxs-lookup"><span data-stu-id="e15d4-216">pastProjects</span></span>|<span data-ttu-id="e15d4-217">String collection</span><span class="sxs-lookup"><span data-stu-id="e15d4-217">String collection</span></span>|<span data-ttu-id="e15d4-218">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="e15d4-218">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="e15d4-219">postalCode</span><span class="sxs-lookup"><span data-stu-id="e15d4-219">postalCode</span></span>|<span data-ttu-id="e15d4-220">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-220">String</span></span>|<span data-ttu-id="e15d4-p114">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="e15d4-224">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="e15d4-224">preferredLanguage</span></span>|<span data-ttu-id="e15d4-225">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-225">String</span></span>|<span data-ttu-id="e15d4-p115">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="e15d4-228">responsibilities</span><span class="sxs-lookup"><span data-stu-id="e15d4-228">responsibilities</span></span>|<span data-ttu-id="e15d4-229">String collection</span><span class="sxs-lookup"><span data-stu-id="e15d4-229">String collection</span></span>|<span data-ttu-id="e15d4-230">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="e15d4-230">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="e15d4-231">schools</span><span class="sxs-lookup"><span data-stu-id="e15d4-231">schools</span></span>|<span data-ttu-id="e15d4-232">String collection</span><span class="sxs-lookup"><span data-stu-id="e15d4-232">String collection</span></span>|<span data-ttu-id="e15d4-233">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="e15d4-233">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="e15d4-234">skills</span><span class="sxs-lookup"><span data-stu-id="e15d4-234">skills</span></span>|<span data-ttu-id="e15d4-235">String collection</span><span class="sxs-lookup"><span data-stu-id="e15d4-235">String collection</span></span>|<span data-ttu-id="e15d4-236">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="e15d4-236">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="e15d4-237">state</span><span class="sxs-lookup"><span data-stu-id="e15d4-237">state</span></span>|<span data-ttu-id="e15d4-238">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-238">String</span></span>|<span data-ttu-id="e15d4-239">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="e15d4-239">The state or province in the user's address.</span></span>|
|<span data-ttu-id="e15d4-240">streetAddress</span><span class="sxs-lookup"><span data-stu-id="e15d4-240">streetAddress</span></span>|<span data-ttu-id="e15d4-241">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-241">String</span></span>|<span data-ttu-id="e15d4-242">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="e15d4-242">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="e15d4-243">surname</span><span class="sxs-lookup"><span data-stu-id="e15d4-243">surname</span></span>|<span data-ttu-id="e15d4-244">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-244">String</span></span>|<span data-ttu-id="e15d4-245">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="e15d4-245">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="e15d4-246">usageLocation</span><span class="sxs-lookup"><span data-stu-id="e15d4-246">usageLocation</span></span>|<span data-ttu-id="e15d4-247">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-247">String</span></span>|<span data-ttu-id="e15d4-248">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="e15d4-248">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="e15d4-249">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="e15d4-249">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="e15d4-250">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="e15d4-250">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="e15d4-251">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e15d4-251">Not nullable.</span></span>|
|<span data-ttu-id="e15d4-252">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e15d4-252">userPrincipalName</span></span>|<span data-ttu-id="e15d4-253">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-253">String</span></span>|<span data-ttu-id="e15d4-p117">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="e15d4-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="e15d4-261">userType</span><span class="sxs-lookup"><span data-stu-id="e15d4-261">userType</span></span>|<span data-ttu-id="e15d4-262">String</span><span class="sxs-lookup"><span data-stu-id="e15d4-262">String</span></span>|<span data-ttu-id="e15d4-263">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="e15d4-263">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="e15d4-264">响应</span><span class="sxs-lookup"><span data-stu-id="e15d4-264">Response</span></span>

<span data-ttu-id="e15d4-265">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e15d4-265">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e15d4-266">示例</span><span class="sxs-lookup"><span data-stu-id="e15d4-266">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="e15d4-267">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="e15d4-267">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="e15d4-268">请求</span><span class="sxs-lookup"><span data-stu-id="e15d4-268">Request</span></span>

<span data-ttu-id="e15d4-269">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="e15d4-269">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e15d4-270">HTTP</span><span class="sxs-lookup"><span data-stu-id="e15d4-270">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e15d4-271">C#</span><span class="sxs-lookup"><span data-stu-id="e15d4-271">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e15d4-272">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e15d4-272">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e15d4-273">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e15d4-273">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e15d4-274">Java</span><span class="sxs-lookup"><span data-stu-id="e15d4-274">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e15d4-275">响应</span><span class="sxs-lookup"><span data-stu-id="e15d4-275">Response</span></span>
<span data-ttu-id="e15d4-276">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="e15d4-276">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="e15d4-277">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="e15d4-277">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="e15d4-278">请求</span><span class="sxs-lookup"><span data-stu-id="e15d4-278">Request</span></span>

<span data-ttu-id="e15d4-279">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="e15d4-279">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e15d4-280">HTTP</span><span class="sxs-lookup"><span data-stu-id="e15d4-280">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e15d4-281">C#</span><span class="sxs-lookup"><span data-stu-id="e15d4-281">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e15d4-282">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e15d4-282">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e15d4-283">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e15d4-283">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e15d4-284">Java</span><span class="sxs-lookup"><span data-stu-id="e15d4-284">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e15d4-285">响应</span><span class="sxs-lookup"><span data-stu-id="e15d4-285">Response</span></span>

<span data-ttu-id="e15d4-286">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="e15d4-286">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
