---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91075356fab7906ce578c0e8a3bcbf5ce49d9c16
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815997"
---
# <a name="update-user"></a><span data-ttu-id="cd935-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="cd935-103">Update user</span></span>

<span data-ttu-id="cd935-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd935-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd935-105">更新 user 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd935-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd935-106">权限</span><span class="sxs-lookup"><span data-stu-id="cd935-106">Permissions</span></span>
<span data-ttu-id="cd935-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd935-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd935-109">Permission type</span></span>      | <span data-ttu-id="cd935-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd935-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd935-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd935-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd935-112">User.ReadWrite、User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd935-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd935-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd935-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd935-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd935-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="cd935-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd935-115">Application</span></span> | <span data-ttu-id="cd935-116">User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd935-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="cd935-117">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="cd935-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="cd935-118">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="cd935-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="cd935-119">有关详细信息，请参阅 [Azure AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="cd935-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="cd935-120">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="cd935-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="cd935-121">更新 **identities** 属性需要 User.ManageIdentities.All 权限。</span><span class="sxs-lookup"><span data-stu-id="cd935-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="cd935-122">此外，不允许将 [B2C 本地帐户](../resources/objectidentity.md)添加到现有 **user** 对象，除非 **user** 对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="cd935-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="cd935-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd935-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="cd935-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd935-124">Request headers</span></span>
| <span data-ttu-id="cd935-125">标头</span><span class="sxs-lookup"><span data-stu-id="cd935-125">Header</span></span>       | <span data-ttu-id="cd935-126">值</span><span class="sxs-lookup"><span data-stu-id="cd935-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cd935-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd935-127">Authorization</span></span>  | <span data-ttu-id="cd935-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd935-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd935-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd935-130">Content-Type</span></span>  | <span data-ttu-id="cd935-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cd935-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd935-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd935-132">Request body</span></span>
<span data-ttu-id="cd935-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cd935-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd935-136">属性</span><span class="sxs-lookup"><span data-stu-id="cd935-136">Property</span></span>     | <span data-ttu-id="cd935-137">类型</span><span class="sxs-lookup"><span data-stu-id="cd935-137">Type</span></span>   |<span data-ttu-id="cd935-138">说明</span><span class="sxs-lookup"><span data-stu-id="cd935-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd935-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="cd935-139">aboutMe</span></span>|<span data-ttu-id="cd935-140">String</span><span class="sxs-lookup"><span data-stu-id="cd935-140">String</span></span>|<span data-ttu-id="cd935-141">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="cd935-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="cd935-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="cd935-142">accountEnabled</span></span>|<span data-ttu-id="cd935-143">布尔</span><span class="sxs-lookup"><span data-stu-id="cd935-143">Boolean</span></span>| <span data-ttu-id="cd935-144">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="cd935-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="cd935-145">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="cd935-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="cd935-146">birthday</span><span class="sxs-lookup"><span data-stu-id="cd935-146">birthday</span></span>|<span data-ttu-id="cd935-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd935-147">DateTimeOffset</span></span>|<span data-ttu-id="cd935-p107">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cd935-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cd935-151">businessPhones</span><span class="sxs-lookup"><span data-stu-id="cd935-151">businessPhones</span></span>| <span data-ttu-id="cd935-152">String collection</span><span class="sxs-lookup"><span data-stu-id="cd935-152">String collection</span></span> | <span data-ttu-id="cd935-p108">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="cd935-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="cd935-155">城市</span><span class="sxs-lookup"><span data-stu-id="cd935-155">city</span></span>|<span data-ttu-id="cd935-156">String</span><span class="sxs-lookup"><span data-stu-id="cd935-156">String</span></span>|<span data-ttu-id="cd935-157">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="cd935-157">The city in which the user is located.</span></span>|
|<span data-ttu-id="cd935-158">country</span><span class="sxs-lookup"><span data-stu-id="cd935-158">country</span></span>|<span data-ttu-id="cd935-159">String</span><span class="sxs-lookup"><span data-stu-id="cd935-159">String</span></span>|<span data-ttu-id="cd935-160">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="cd935-160">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="cd935-161">department</span><span class="sxs-lookup"><span data-stu-id="cd935-161">department</span></span>|<span data-ttu-id="cd935-162">String</span><span class="sxs-lookup"><span data-stu-id="cd935-162">String</span></span>|<span data-ttu-id="cd935-163">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="cd935-163">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="cd935-164">displayName</span><span class="sxs-lookup"><span data-stu-id="cd935-164">displayName</span></span>|<span data-ttu-id="cd935-165">String</span><span class="sxs-lookup"><span data-stu-id="cd935-165">String</span></span>|<span data-ttu-id="cd935-p109">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="cd935-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="cd935-170">givenName</span><span class="sxs-lookup"><span data-stu-id="cd935-170">givenName</span></span>|<span data-ttu-id="cd935-171">String</span><span class="sxs-lookup"><span data-stu-id="cd935-171">String</span></span>|<span data-ttu-id="cd935-172">用户的名。</span><span class="sxs-lookup"><span data-stu-id="cd935-172">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="cd935-173">hireDate</span><span class="sxs-lookup"><span data-stu-id="cd935-173">hireDate</span></span>|<span data-ttu-id="cd935-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd935-174">DateTimeOffset</span></span>|<span data-ttu-id="cd935-p110">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cd935-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cd935-178">interests</span><span class="sxs-lookup"><span data-stu-id="cd935-178">interests</span></span>|<span data-ttu-id="cd935-179">String collection</span><span class="sxs-lookup"><span data-stu-id="cd935-179">String collection</span></span>|<span data-ttu-id="cd935-180">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="cd935-180">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="cd935-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="cd935-181">jobTitle</span></span>|<span data-ttu-id="cd935-182">String</span><span class="sxs-lookup"><span data-stu-id="cd935-182">String</span></span>|<span data-ttu-id="cd935-183">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="cd935-183">The user’s job title.</span></span>|
|<span data-ttu-id="cd935-184">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cd935-184">mailNickname</span></span>|<span data-ttu-id="cd935-185">String</span><span class="sxs-lookup"><span data-stu-id="cd935-185">String</span></span>|<span data-ttu-id="cd935-186">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="cd935-186">The mail alias for the user.</span></span> <span data-ttu-id="cd935-187">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="cd935-187">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="cd935-188">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="cd935-188">mobilePhone</span></span>|<span data-ttu-id="cd935-189">String</span><span class="sxs-lookup"><span data-stu-id="cd935-189">String</span></span>|<span data-ttu-id="cd935-190">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="cd935-190">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="cd935-191">mySite</span><span class="sxs-lookup"><span data-stu-id="cd935-191">mySite</span></span>|<span data-ttu-id="cd935-192">String</span><span class="sxs-lookup"><span data-stu-id="cd935-192">String</span></span>|<span data-ttu-id="cd935-193">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="cd935-193">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="cd935-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="cd935-194">officeLocation</span></span>|<span data-ttu-id="cd935-195">String</span><span class="sxs-lookup"><span data-stu-id="cd935-195">String</span></span>|<span data-ttu-id="cd935-196">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="cd935-196">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="cd935-197">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="cd935-197">onPremisesImmutableId</span></span>|<span data-ttu-id="cd935-198">String</span><span class="sxs-lookup"><span data-stu-id="cd935-198">String</span></span>|<span data-ttu-id="cd935-199">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="cd935-199">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="cd935-200">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="cd935-200">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="cd935-201">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="cd935-201">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="cd935-202">otherMails</span><span class="sxs-lookup"><span data-stu-id="cd935-202">otherMails</span></span>|<span data-ttu-id="cd935-203">String</span><span class="sxs-lookup"><span data-stu-id="cd935-203">String</span></span> |<span data-ttu-id="cd935-204">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="cd935-204">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="cd935-205">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="cd935-205">passwordPolicies</span></span>|<span data-ttu-id="cd935-206">String</span><span class="sxs-lookup"><span data-stu-id="cd935-206">String</span></span>|<span data-ttu-id="cd935-p113">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="cd935-p113">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="cd935-211">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="cd935-211">passwordProfile</span></span>|[<span data-ttu-id="cd935-212">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="cd935-212">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="cd935-p114">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="cd935-p114">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="cd935-218">pastProjects</span><span class="sxs-lookup"><span data-stu-id="cd935-218">pastProjects</span></span>|<span data-ttu-id="cd935-219">String collection</span><span class="sxs-lookup"><span data-stu-id="cd935-219">String collection</span></span>|<span data-ttu-id="cd935-220">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="cd935-220">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="cd935-221">postalCode</span><span class="sxs-lookup"><span data-stu-id="cd935-221">postalCode</span></span>|<span data-ttu-id="cd935-222">String</span><span class="sxs-lookup"><span data-stu-id="cd935-222">String</span></span>|<span data-ttu-id="cd935-p115">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="cd935-p115">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="cd935-226">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="cd935-226">preferredLanguage</span></span>|<span data-ttu-id="cd935-227">String</span><span class="sxs-lookup"><span data-stu-id="cd935-227">String</span></span>|<span data-ttu-id="cd935-p116">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="cd935-p116">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="cd935-230">responsibilities</span><span class="sxs-lookup"><span data-stu-id="cd935-230">responsibilities</span></span>|<span data-ttu-id="cd935-231">String collection</span><span class="sxs-lookup"><span data-stu-id="cd935-231">String collection</span></span>|<span data-ttu-id="cd935-232">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="cd935-232">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="cd935-233">schools</span><span class="sxs-lookup"><span data-stu-id="cd935-233">schools</span></span>|<span data-ttu-id="cd935-234">String collection</span><span class="sxs-lookup"><span data-stu-id="cd935-234">String collection</span></span>|<span data-ttu-id="cd935-235">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="cd935-235">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="cd935-236">skills</span><span class="sxs-lookup"><span data-stu-id="cd935-236">skills</span></span>|<span data-ttu-id="cd935-237">String collection</span><span class="sxs-lookup"><span data-stu-id="cd935-237">String collection</span></span>|<span data-ttu-id="cd935-238">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="cd935-238">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="cd935-239">state</span><span class="sxs-lookup"><span data-stu-id="cd935-239">state</span></span>|<span data-ttu-id="cd935-240">String</span><span class="sxs-lookup"><span data-stu-id="cd935-240">String</span></span>|<span data-ttu-id="cd935-241">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="cd935-241">The state or province in the user's address.</span></span>|
|<span data-ttu-id="cd935-242">streetAddress</span><span class="sxs-lookup"><span data-stu-id="cd935-242">streetAddress</span></span>|<span data-ttu-id="cd935-243">String</span><span class="sxs-lookup"><span data-stu-id="cd935-243">String</span></span>|<span data-ttu-id="cd935-244">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="cd935-244">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="cd935-245">surname</span><span class="sxs-lookup"><span data-stu-id="cd935-245">surname</span></span>|<span data-ttu-id="cd935-246">String</span><span class="sxs-lookup"><span data-stu-id="cd935-246">String</span></span>|<span data-ttu-id="cd935-247">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="cd935-247">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="cd935-248">usageLocation</span><span class="sxs-lookup"><span data-stu-id="cd935-248">usageLocation</span></span>|<span data-ttu-id="cd935-249">String</span><span class="sxs-lookup"><span data-stu-id="cd935-249">String</span></span>|<span data-ttu-id="cd935-250">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="cd935-250">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="cd935-251">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="cd935-251">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="cd935-252">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="cd935-252">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="cd935-253">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="cd935-253">Not nullable.</span></span>|
|<span data-ttu-id="cd935-254">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cd935-254">userPrincipalName</span></span>|<span data-ttu-id="cd935-255">String</span><span class="sxs-lookup"><span data-stu-id="cd935-255">String</span></span>|<span data-ttu-id="cd935-p118">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="cd935-p118">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="cd935-263">userType</span><span class="sxs-lookup"><span data-stu-id="cd935-263">userType</span></span>|<span data-ttu-id="cd935-264">String</span><span class="sxs-lookup"><span data-stu-id="cd935-264">String</span></span>|<span data-ttu-id="cd935-265">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="cd935-265">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="cd935-266">响应</span><span class="sxs-lookup"><span data-stu-id="cd935-266">Response</span></span>

<span data-ttu-id="cd935-267">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd935-267">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd935-268">示例</span><span class="sxs-lookup"><span data-stu-id="cd935-268">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="cd935-269">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="cd935-269">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="cd935-270">请求</span><span class="sxs-lookup"><span data-stu-id="cd935-270">Request</span></span>

<span data-ttu-id="cd935-271">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="cd935-271">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd935-272">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd935-272">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd935-273">C#</span><span class="sxs-lookup"><span data-stu-id="cd935-273">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd935-274">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd935-274">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd935-275">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd935-275">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd935-276">Java</span><span class="sxs-lookup"><span data-stu-id="cd935-276">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cd935-277">响应</span><span class="sxs-lookup"><span data-stu-id="cd935-277">Response</span></span>
<span data-ttu-id="cd935-278">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="cd935-278">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="cd935-279">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="cd935-279">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="cd935-280">请求</span><span class="sxs-lookup"><span data-stu-id="cd935-280">Request</span></span>

<span data-ttu-id="cd935-281">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="cd935-281">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cd935-282">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd935-282">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd935-283">C#</span><span class="sxs-lookup"><span data-stu-id="cd935-283">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd935-284">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd935-284">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd935-285">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd935-285">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd935-286">Java</span><span class="sxs-lookup"><span data-stu-id="cd935-286">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd935-287">响应</span><span class="sxs-lookup"><span data-stu-id="cd935-287">Response</span></span>

<span data-ttu-id="cd935-288">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="cd935-288">The following example shows the response.</span></span>
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
