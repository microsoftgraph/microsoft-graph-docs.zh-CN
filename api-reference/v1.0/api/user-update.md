---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af8d2c99d814c8a7b82e905e3fbbc7d5709bb9d6
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396854"
---
# <a name="update-user"></a><span data-ttu-id="a4872-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="a4872-103">Update user</span></span>

<span data-ttu-id="a4872-104">更新 user 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4872-104">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4872-105">权限</span><span class="sxs-lookup"><span data-stu-id="a4872-105">Permissions</span></span>
<span data-ttu-id="a4872-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4872-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4872-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4872-108">Permission type</span></span>      | <span data-ttu-id="a4872-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4872-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4872-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4872-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4872-111">User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4872-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4872-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4872-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4872-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4872-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="a4872-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4872-114">Application</span></span> | <span data-ttu-id="a4872-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4872-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="a4872-116">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="a4872-116">When updating the passwordProfile property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="a4872-117">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="a4872-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="a4872-118">有关详细信息，请参阅 [Azure AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="a4872-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="a4872-119">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="a4872-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="a4872-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4872-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="a4872-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4872-121">Request headers</span></span>
| <span data-ttu-id="a4872-122">标头</span><span class="sxs-lookup"><span data-stu-id="a4872-122">Header</span></span>       | <span data-ttu-id="a4872-123">值</span><span class="sxs-lookup"><span data-stu-id="a4872-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a4872-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4872-124">Authorization</span></span>  | <span data-ttu-id="a4872-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4872-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4872-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4872-127">Content-Type</span></span>  | <span data-ttu-id="a4872-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a4872-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4872-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4872-129">Request body</span></span>
<span data-ttu-id="a4872-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a4872-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a4872-133">属性</span><span class="sxs-lookup"><span data-stu-id="a4872-133">Property</span></span>     | <span data-ttu-id="a4872-134">类型</span><span class="sxs-lookup"><span data-stu-id="a4872-134">Type</span></span>   |<span data-ttu-id="a4872-135">说明</span><span class="sxs-lookup"><span data-stu-id="a4872-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4872-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="a4872-136">aboutMe</span></span>|<span data-ttu-id="a4872-137">String</span><span class="sxs-lookup"><span data-stu-id="a4872-137">String</span></span>|<span data-ttu-id="a4872-138">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="a4872-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="a4872-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="a4872-139">accountEnabled</span></span>|<span data-ttu-id="a4872-140">布尔</span><span class="sxs-lookup"><span data-stu-id="a4872-140">Boolean</span></span>| <span data-ttu-id="a4872-141">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="a4872-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="a4872-142">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="a4872-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="a4872-143">birthday</span><span class="sxs-lookup"><span data-stu-id="a4872-143">birthday</span></span>|<span data-ttu-id="a4872-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4872-144">DateTimeOffset</span></span>|<span data-ttu-id="a4872-p106">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4872-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a4872-148">businessPhones</span><span class="sxs-lookup"><span data-stu-id="a4872-148">businessPhones</span></span>| <span data-ttu-id="a4872-149">String collection</span><span class="sxs-lookup"><span data-stu-id="a4872-149">String collection</span></span> | <span data-ttu-id="a4872-p107">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="a4872-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="a4872-152">城市</span><span class="sxs-lookup"><span data-stu-id="a4872-152">city</span></span>|<span data-ttu-id="a4872-153">String</span><span class="sxs-lookup"><span data-stu-id="a4872-153">String</span></span>|<span data-ttu-id="a4872-154">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="a4872-154">The city in which the user is located.</span></span>|
|<span data-ttu-id="a4872-155">country</span><span class="sxs-lookup"><span data-stu-id="a4872-155">country</span></span>|<span data-ttu-id="a4872-156">String</span><span class="sxs-lookup"><span data-stu-id="a4872-156">String</span></span>|<span data-ttu-id="a4872-157">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="a4872-157">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="a4872-158">department</span><span class="sxs-lookup"><span data-stu-id="a4872-158">department</span></span>|<span data-ttu-id="a4872-159">String</span><span class="sxs-lookup"><span data-stu-id="a4872-159">String</span></span>|<span data-ttu-id="a4872-160">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="a4872-160">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="a4872-161">displayName</span><span class="sxs-lookup"><span data-stu-id="a4872-161">displayName</span></span>|<span data-ttu-id="a4872-162">String</span><span class="sxs-lookup"><span data-stu-id="a4872-162">String</span></span>|<span data-ttu-id="a4872-p108">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="a4872-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="a4872-167">givenName</span><span class="sxs-lookup"><span data-stu-id="a4872-167">givenName</span></span>|<span data-ttu-id="a4872-168">String</span><span class="sxs-lookup"><span data-stu-id="a4872-168">String</span></span>|<span data-ttu-id="a4872-169">用户的名。</span><span class="sxs-lookup"><span data-stu-id="a4872-169">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="a4872-170">hireDate</span><span class="sxs-lookup"><span data-stu-id="a4872-170">hireDate</span></span>|<span data-ttu-id="a4872-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4872-171">DateTimeOffset</span></span>|<span data-ttu-id="a4872-p109">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4872-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a4872-175">interests</span><span class="sxs-lookup"><span data-stu-id="a4872-175">interests</span></span>|<span data-ttu-id="a4872-176">String collection</span><span class="sxs-lookup"><span data-stu-id="a4872-176">String collection</span></span>|<span data-ttu-id="a4872-177">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="a4872-177">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="a4872-178">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a4872-178">jobTitle</span></span>|<span data-ttu-id="a4872-179">String</span><span class="sxs-lookup"><span data-stu-id="a4872-179">String</span></span>|<span data-ttu-id="a4872-180">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="a4872-180">The user’s job title.</span></span>|
|<span data-ttu-id="a4872-181">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a4872-181">mailNickname</span></span>|<span data-ttu-id="a4872-182">String</span><span class="sxs-lookup"><span data-stu-id="a4872-182">String</span></span>|<span data-ttu-id="a4872-183">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="a4872-183">The mail alias for the user.</span></span> <span data-ttu-id="a4872-184">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="a4872-184">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="a4872-185">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="a4872-185">mobilePhone</span></span>|<span data-ttu-id="a4872-186">String</span><span class="sxs-lookup"><span data-stu-id="a4872-186">String</span></span>|<span data-ttu-id="a4872-187">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="a4872-187">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="a4872-188">mySite</span><span class="sxs-lookup"><span data-stu-id="a4872-188">mySite</span></span>|<span data-ttu-id="a4872-189">String</span><span class="sxs-lookup"><span data-stu-id="a4872-189">String</span></span>|<span data-ttu-id="a4872-190">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="a4872-190">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="a4872-191">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a4872-191">officeLocation</span></span>|<span data-ttu-id="a4872-192">String</span><span class="sxs-lookup"><span data-stu-id="a4872-192">String</span></span>|<span data-ttu-id="a4872-193">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="a4872-193">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="a4872-194">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="a4872-194">onPremisesImmutableId</span></span>|<span data-ttu-id="a4872-195">String</span><span class="sxs-lookup"><span data-stu-id="a4872-195">String</span></span>|<span data-ttu-id="a4872-196">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="a4872-196">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="a4872-197">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="a4872-197">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="a4872-198">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="a4872-198">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="a4872-199">otherMails</span><span class="sxs-lookup"><span data-stu-id="a4872-199">otherMails</span></span>|<span data-ttu-id="a4872-200">String</span><span class="sxs-lookup"><span data-stu-id="a4872-200">String</span></span> |<span data-ttu-id="a4872-201">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="a4872-201">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="a4872-202">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="a4872-202">passwordPolicies</span></span>|<span data-ttu-id="a4872-203">String</span><span class="sxs-lookup"><span data-stu-id="a4872-203">String</span></span>|<span data-ttu-id="a4872-p112">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="a4872-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="a4872-208">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="a4872-208">passwordProfile</span></span>|[<span data-ttu-id="a4872-209">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="a4872-209">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="a4872-p113">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="a4872-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="a4872-215">pastProjects</span><span class="sxs-lookup"><span data-stu-id="a4872-215">pastProjects</span></span>|<span data-ttu-id="a4872-216">String collection</span><span class="sxs-lookup"><span data-stu-id="a4872-216">String collection</span></span>|<span data-ttu-id="a4872-217">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="a4872-217">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="a4872-218">postalCode</span><span class="sxs-lookup"><span data-stu-id="a4872-218">postalCode</span></span>|<span data-ttu-id="a4872-219">String</span><span class="sxs-lookup"><span data-stu-id="a4872-219">String</span></span>|<span data-ttu-id="a4872-p114">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="a4872-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="a4872-223">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="a4872-223">preferredLanguage</span></span>|<span data-ttu-id="a4872-224">String</span><span class="sxs-lookup"><span data-stu-id="a4872-224">String</span></span>|<span data-ttu-id="a4872-p115">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="a4872-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="a4872-227">responsibilities</span><span class="sxs-lookup"><span data-stu-id="a4872-227">responsibilities</span></span>|<span data-ttu-id="a4872-228">String collection</span><span class="sxs-lookup"><span data-stu-id="a4872-228">String collection</span></span>|<span data-ttu-id="a4872-229">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="a4872-229">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="a4872-230">schools</span><span class="sxs-lookup"><span data-stu-id="a4872-230">schools</span></span>|<span data-ttu-id="a4872-231">String collection</span><span class="sxs-lookup"><span data-stu-id="a4872-231">String collection</span></span>|<span data-ttu-id="a4872-232">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="a4872-232">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="a4872-233">skills</span><span class="sxs-lookup"><span data-stu-id="a4872-233">skills</span></span>|<span data-ttu-id="a4872-234">String collection</span><span class="sxs-lookup"><span data-stu-id="a4872-234">String collection</span></span>|<span data-ttu-id="a4872-235">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="a4872-235">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="a4872-236">state</span><span class="sxs-lookup"><span data-stu-id="a4872-236">state</span></span>|<span data-ttu-id="a4872-237">String</span><span class="sxs-lookup"><span data-stu-id="a4872-237">String</span></span>|<span data-ttu-id="a4872-238">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="a4872-238">The state or province in the user's address.</span></span>|
|<span data-ttu-id="a4872-239">streetAddress</span><span class="sxs-lookup"><span data-stu-id="a4872-239">streetAddress</span></span>|<span data-ttu-id="a4872-240">String</span><span class="sxs-lookup"><span data-stu-id="a4872-240">String</span></span>|<span data-ttu-id="a4872-241">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="a4872-241">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="a4872-242">surname</span><span class="sxs-lookup"><span data-stu-id="a4872-242">surname</span></span>|<span data-ttu-id="a4872-243">String</span><span class="sxs-lookup"><span data-stu-id="a4872-243">String</span></span>|<span data-ttu-id="a4872-244">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="a4872-244">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="a4872-245">usageLocation</span><span class="sxs-lookup"><span data-stu-id="a4872-245">usageLocation</span></span>|<span data-ttu-id="a4872-246">String</span><span class="sxs-lookup"><span data-stu-id="a4872-246">String</span></span>|<span data-ttu-id="a4872-247">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="a4872-247">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="a4872-248">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="a4872-248">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="a4872-249">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="a4872-249">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="a4872-250">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="a4872-250">Not nullable.</span></span>|
|<span data-ttu-id="a4872-251">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4872-251">userPrincipalName</span></span>|<span data-ttu-id="a4872-252">String</span><span class="sxs-lookup"><span data-stu-id="a4872-252">String</span></span>|<span data-ttu-id="a4872-p117">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="a4872-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="a4872-260">userType</span><span class="sxs-lookup"><span data-stu-id="a4872-260">userType</span></span>|<span data-ttu-id="a4872-261">String</span><span class="sxs-lookup"><span data-stu-id="a4872-261">String</span></span>|<span data-ttu-id="a4872-262">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="a4872-262">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="a4872-263">响应</span><span class="sxs-lookup"><span data-stu-id="a4872-263">Response</span></span>

<span data-ttu-id="a4872-264">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4872-264">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4872-265">示例</span><span class="sxs-lookup"><span data-stu-id="a4872-265">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="a4872-266">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="a4872-266">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="a4872-267">请求</span><span class="sxs-lookup"><span data-stu-id="a4872-267">Request</span></span>

<span data-ttu-id="a4872-268">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="a4872-268">The following example shows how to create a request context.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4872-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4872-269">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4872-270">C#</span><span class="sxs-lookup"><span data-stu-id="a4872-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4872-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4872-271">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4872-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4872-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4872-273">Java</span><span class="sxs-lookup"><span data-stu-id="a4872-273">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a4872-274">响应</span><span class="sxs-lookup"><span data-stu-id="a4872-274">Response</span></span>
<span data-ttu-id="a4872-275">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a4872-275">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="a4872-276">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="a4872-276">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="a4872-277">请求</span><span class="sxs-lookup"><span data-stu-id="a4872-277">Request</span></span>

<span data-ttu-id="a4872-278">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="a4872-278">The following example shows how to create a request context.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a4872-279">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4872-279">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4872-280">C#</span><span class="sxs-lookup"><span data-stu-id="a4872-280">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4872-281">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4872-281">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4872-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4872-282">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4872-283">Java</span><span class="sxs-lookup"><span data-stu-id="a4872-283">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4872-284">响应</span><span class="sxs-lookup"><span data-stu-id="a4872-284">Response</span></span>

<span data-ttu-id="a4872-285">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a4872-285">The following example shows the response.</span></span>
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
