---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 66ad944f99010e643adfdab039be8b9c33884b35
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278636"
---
# <a name="update-user"></a><span data-ttu-id="62329-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="62329-103">Update user</span></span>

<span data-ttu-id="62329-104">更新 user 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="62329-104">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62329-105">权限</span><span class="sxs-lookup"><span data-stu-id="62329-105">Permissions</span></span>
<span data-ttu-id="62329-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62329-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="62329-108">Permission type</span></span>      | <span data-ttu-id="62329-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62329-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62329-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62329-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62329-111">User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62329-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62329-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62329-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62329-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62329-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="62329-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="62329-114">Application</span></span> | <span data-ttu-id="62329-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62329-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="62329-116">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="62329-116">When updating the passwordProfile property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="62329-117">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="62329-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="62329-118">有关详细信息，请参阅 [Azure AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="62329-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="62329-119">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="62329-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="62329-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62329-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="62329-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="62329-121">Request headers</span></span>
| <span data-ttu-id="62329-122">标头</span><span class="sxs-lookup"><span data-stu-id="62329-122">Header</span></span>       | <span data-ttu-id="62329-123">值</span><span class="sxs-lookup"><span data-stu-id="62329-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="62329-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="62329-124">Authorization</span></span>  | <span data-ttu-id="62329-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62329-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62329-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62329-127">Content-Type</span></span>  | <span data-ttu-id="62329-128">application/json</span><span class="sxs-lookup"><span data-stu-id="62329-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62329-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="62329-129">Request body</span></span>
<span data-ttu-id="62329-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="62329-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="62329-133">属性</span><span class="sxs-lookup"><span data-stu-id="62329-133">Property</span></span>     | <span data-ttu-id="62329-134">类型</span><span class="sxs-lookup"><span data-stu-id="62329-134">Type</span></span>   |<span data-ttu-id="62329-135">说明</span><span class="sxs-lookup"><span data-stu-id="62329-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62329-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="62329-136">aboutMe</span></span>|<span data-ttu-id="62329-137">String</span><span class="sxs-lookup"><span data-stu-id="62329-137">String</span></span>|<span data-ttu-id="62329-138">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="62329-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="62329-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="62329-139">accountEnabled</span></span>|<span data-ttu-id="62329-140">布尔</span><span class="sxs-lookup"><span data-stu-id="62329-140">Boolean</span></span>| <span data-ttu-id="62329-141">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="62329-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="62329-142">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="62329-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="62329-143">birthday</span><span class="sxs-lookup"><span data-stu-id="62329-143">birthday</span></span>|<span data-ttu-id="62329-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62329-144">DateTimeOffset</span></span>|<span data-ttu-id="62329-p106">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="62329-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="62329-148">businessPhones</span><span class="sxs-lookup"><span data-stu-id="62329-148">businessPhones</span></span>| <span data-ttu-id="62329-149">String collection</span><span class="sxs-lookup"><span data-stu-id="62329-149">String collection</span></span> | <span data-ttu-id="62329-p107">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="62329-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="62329-152">城市</span><span class="sxs-lookup"><span data-stu-id="62329-152">city</span></span>|<span data-ttu-id="62329-153">String</span><span class="sxs-lookup"><span data-stu-id="62329-153">String</span></span>|<span data-ttu-id="62329-154">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="62329-154">The city in which the user is located.</span></span>|
|<span data-ttu-id="62329-155">country</span><span class="sxs-lookup"><span data-stu-id="62329-155">country</span></span>|<span data-ttu-id="62329-156">String</span><span class="sxs-lookup"><span data-stu-id="62329-156">String</span></span>|<span data-ttu-id="62329-157">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="62329-157">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="62329-158">department</span><span class="sxs-lookup"><span data-stu-id="62329-158">department</span></span>|<span data-ttu-id="62329-159">String</span><span class="sxs-lookup"><span data-stu-id="62329-159">String</span></span>|<span data-ttu-id="62329-160">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="62329-160">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="62329-161">displayName</span><span class="sxs-lookup"><span data-stu-id="62329-161">displayName</span></span>|<span data-ttu-id="62329-162">String</span><span class="sxs-lookup"><span data-stu-id="62329-162">String</span></span>|<span data-ttu-id="62329-p108">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="62329-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="62329-167">givenName</span><span class="sxs-lookup"><span data-stu-id="62329-167">givenName</span></span>|<span data-ttu-id="62329-168">String</span><span class="sxs-lookup"><span data-stu-id="62329-168">String</span></span>|<span data-ttu-id="62329-169">用户的名。</span><span class="sxs-lookup"><span data-stu-id="62329-169">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="62329-170">hireDate</span><span class="sxs-lookup"><span data-stu-id="62329-170">hireDate</span></span>|<span data-ttu-id="62329-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62329-171">DateTimeOffset</span></span>|<span data-ttu-id="62329-p109">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="62329-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="62329-175">interests</span><span class="sxs-lookup"><span data-stu-id="62329-175">interests</span></span>|<span data-ttu-id="62329-176">String collection</span><span class="sxs-lookup"><span data-stu-id="62329-176">String collection</span></span>|<span data-ttu-id="62329-177">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="62329-177">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="62329-178">jobTitle</span><span class="sxs-lookup"><span data-stu-id="62329-178">jobTitle</span></span>|<span data-ttu-id="62329-179">String</span><span class="sxs-lookup"><span data-stu-id="62329-179">String</span></span>|<span data-ttu-id="62329-180">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="62329-180">The user’s job title.</span></span>|
|<span data-ttu-id="62329-181">mailNickname</span><span class="sxs-lookup"><span data-stu-id="62329-181">mailNickname</span></span>|<span data-ttu-id="62329-182">String</span><span class="sxs-lookup"><span data-stu-id="62329-182">String</span></span>|<span data-ttu-id="62329-183">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="62329-183">The mail alias for the user.</span></span> <span data-ttu-id="62329-184">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="62329-184">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="62329-185">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="62329-185">mobilePhone</span></span>|<span data-ttu-id="62329-186">String</span><span class="sxs-lookup"><span data-stu-id="62329-186">String</span></span>|<span data-ttu-id="62329-187">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="62329-187">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="62329-188">mySite</span><span class="sxs-lookup"><span data-stu-id="62329-188">mySite</span></span>|<span data-ttu-id="62329-189">String</span><span class="sxs-lookup"><span data-stu-id="62329-189">String</span></span>|<span data-ttu-id="62329-190">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="62329-190">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="62329-191">officeLocation</span><span class="sxs-lookup"><span data-stu-id="62329-191">officeLocation</span></span>|<span data-ttu-id="62329-192">String</span><span class="sxs-lookup"><span data-stu-id="62329-192">String</span></span>|<span data-ttu-id="62329-193">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="62329-193">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="62329-194">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="62329-194">onPremisesImmutableId</span></span>|<span data-ttu-id="62329-195">String</span><span class="sxs-lookup"><span data-stu-id="62329-195">String</span></span>|<span data-ttu-id="62329-196">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="62329-196">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="62329-197">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="62329-197">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="62329-198">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="62329-198">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="62329-199">otherMails</span><span class="sxs-lookup"><span data-stu-id="62329-199">otherMails</span></span>|<span data-ttu-id="62329-200">String</span><span class="sxs-lookup"><span data-stu-id="62329-200">String</span></span> |<span data-ttu-id="62329-201">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="62329-201">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="62329-202">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="62329-202">passwordPolicies</span></span>|<span data-ttu-id="62329-203">String</span><span class="sxs-lookup"><span data-stu-id="62329-203">String</span></span>|<span data-ttu-id="62329-p112">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="62329-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="62329-208">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="62329-208">passwordProfile</span></span>|[<span data-ttu-id="62329-209">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="62329-209">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="62329-p113">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="62329-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="62329-215">pastProjects</span><span class="sxs-lookup"><span data-stu-id="62329-215">pastProjects</span></span>|<span data-ttu-id="62329-216">String collection</span><span class="sxs-lookup"><span data-stu-id="62329-216">String collection</span></span>|<span data-ttu-id="62329-217">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="62329-217">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="62329-218">postalCode</span><span class="sxs-lookup"><span data-stu-id="62329-218">postalCode</span></span>|<span data-ttu-id="62329-219">String</span><span class="sxs-lookup"><span data-stu-id="62329-219">String</span></span>|<span data-ttu-id="62329-p114">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="62329-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="62329-223">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="62329-223">preferredLanguage</span></span>|<span data-ttu-id="62329-224">String</span><span class="sxs-lookup"><span data-stu-id="62329-224">String</span></span>|<span data-ttu-id="62329-p115">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="62329-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="62329-227">responsibilities</span><span class="sxs-lookup"><span data-stu-id="62329-227">responsibilities</span></span>|<span data-ttu-id="62329-228">String collection</span><span class="sxs-lookup"><span data-stu-id="62329-228">String collection</span></span>|<span data-ttu-id="62329-229">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="62329-229">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="62329-230">schools</span><span class="sxs-lookup"><span data-stu-id="62329-230">schools</span></span>|<span data-ttu-id="62329-231">String collection</span><span class="sxs-lookup"><span data-stu-id="62329-231">String collection</span></span>|<span data-ttu-id="62329-232">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="62329-232">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="62329-233">skills</span><span class="sxs-lookup"><span data-stu-id="62329-233">skills</span></span>|<span data-ttu-id="62329-234">String collection</span><span class="sxs-lookup"><span data-stu-id="62329-234">String collection</span></span>|<span data-ttu-id="62329-235">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="62329-235">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="62329-236">state</span><span class="sxs-lookup"><span data-stu-id="62329-236">state</span></span>|<span data-ttu-id="62329-237">String</span><span class="sxs-lookup"><span data-stu-id="62329-237">String</span></span>|<span data-ttu-id="62329-238">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="62329-238">The state or province in the user's address.</span></span>|
|<span data-ttu-id="62329-239">streetAddress</span><span class="sxs-lookup"><span data-stu-id="62329-239">streetAddress</span></span>|<span data-ttu-id="62329-240">String</span><span class="sxs-lookup"><span data-stu-id="62329-240">String</span></span>|<span data-ttu-id="62329-241">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="62329-241">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="62329-242">surname</span><span class="sxs-lookup"><span data-stu-id="62329-242">surname</span></span>|<span data-ttu-id="62329-243">String</span><span class="sxs-lookup"><span data-stu-id="62329-243">String</span></span>|<span data-ttu-id="62329-244">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="62329-244">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="62329-245">usageLocation</span><span class="sxs-lookup"><span data-stu-id="62329-245">usageLocation</span></span>|<span data-ttu-id="62329-246">String</span><span class="sxs-lookup"><span data-stu-id="62329-246">String</span></span>|<span data-ttu-id="62329-247">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="62329-247">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="62329-248">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="62329-248">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="62329-249">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="62329-249">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="62329-250">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="62329-250">Not nullable.</span></span>|
|<span data-ttu-id="62329-251">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62329-251">userPrincipalName</span></span>|<span data-ttu-id="62329-252">String</span><span class="sxs-lookup"><span data-stu-id="62329-252">String</span></span>|<span data-ttu-id="62329-p117">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="62329-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="62329-260">userType</span><span class="sxs-lookup"><span data-stu-id="62329-260">userType</span></span>|<span data-ttu-id="62329-261">String</span><span class="sxs-lookup"><span data-stu-id="62329-261">String</span></span>|<span data-ttu-id="62329-262">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="62329-262">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="62329-263">响应</span><span class="sxs-lookup"><span data-stu-id="62329-263">Response</span></span>

<span data-ttu-id="62329-264">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="62329-264">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="62329-265">示例</span><span class="sxs-lookup"><span data-stu-id="62329-265">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62329-266">请求</span><span class="sxs-lookup"><span data-stu-id="62329-266">Request</span></span>
<span data-ttu-id="62329-267">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62329-267">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a><span data-ttu-id="62329-268">响应</span><span class="sxs-lookup"><span data-stu-id="62329-268">Response</span></span>
<span data-ttu-id="62329-269">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="62329-269">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62329-270">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="62329-270">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62329-271">C#</span><span class="sxs-lookup"><span data-stu-id="62329-271">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62329-272">Javascript</span><span class="sxs-lookup"><span data-stu-id="62329-272">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="62329-273">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62329-273">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
