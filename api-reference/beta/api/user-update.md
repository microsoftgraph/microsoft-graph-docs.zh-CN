---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bda197e1f0ce619fe0830da38a8b1b5b5df45c0f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996117"
---
# <a name="update-user"></a><span data-ttu-id="5e053-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="5e053-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e053-104">更新 [user](../resources/user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e053-104">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e053-105">权限</span><span class="sxs-lookup"><span data-stu-id="5e053-105">Permissions</span></span>
<span data-ttu-id="5e053-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e053-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e053-108">Permission type</span></span>      | <span data-ttu-id="5e053-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e053-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e053-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e053-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e053-111">所有的用户读写全部。所有</span><span class="sxs-lookup"><span data-stu-id="5e053-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e053-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e053-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e053-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e053-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="5e053-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e053-114">Application</span></span> | <span data-ttu-id="5e053-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e053-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="5e053-116">更新**passwordProfile**属性时, 需要以下权限: directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="5e053-116">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="5e053-117">仅允许非管理员用户或分配了以下角色之一的用户更新另一个用户的**businessPhones**、 **mobilePhone**或**OtherMails**属性: 目录读取器、来宾邀请者、消息中心读取器和报告读取器。</span><span class="sxs-lookup"><span data-stu-id="5e053-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="5e053-118">有关更多详细信息, 请参阅[AZURE AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员 (密码) 管理员。</span><span class="sxs-lookup"><span data-stu-id="5e053-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="5e053-119">对于授予了 User. ReadWrite、All 或 Directory 的所有委派或应用程序权限的应用程序, 情况也是如此。</span><span class="sxs-lookup"><span data-stu-id="5e053-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>


## <a name="http-request"></a><span data-ttu-id="5e053-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e053-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="5e053-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e053-121">Request headers</span></span>
| <span data-ttu-id="5e053-122">标头</span><span class="sxs-lookup"><span data-stu-id="5e053-122">Header</span></span>       | <span data-ttu-id="5e053-123">值</span><span class="sxs-lookup"><span data-stu-id="5e053-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5e053-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e053-124">Authorization</span></span>  | <span data-ttu-id="5e053-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e053-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e053-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e053-127">Content-Type</span></span>  | <span data-ttu-id="5e053-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5e053-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e053-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e053-129">Request body</span></span>
<span data-ttu-id="5e053-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5e053-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e053-133">属性</span><span class="sxs-lookup"><span data-stu-id="5e053-133">Property</span></span>     | <span data-ttu-id="5e053-134">类型</span><span class="sxs-lookup"><span data-stu-id="5e053-134">Type</span></span>   |<span data-ttu-id="5e053-135">说明</span><span class="sxs-lookup"><span data-stu-id="5e053-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e053-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="5e053-136">aboutMe</span></span>|<span data-ttu-id="5e053-137">String</span><span class="sxs-lookup"><span data-stu-id="5e053-137">String</span></span>|<span data-ttu-id="5e053-138">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="5e053-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="5e053-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="5e053-139">accountEnabled</span></span>|<span data-ttu-id="5e053-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e053-140">Boolean</span></span>| <span data-ttu-id="5e053-141">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="5e053-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="5e053-142">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="5e053-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="5e053-143">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="5e053-143">assignedLicenses</span></span>|<span data-ttu-id="5e053-144">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="5e053-144">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="5e053-p106">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5e053-p106">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="5e053-147">birthday</span><span class="sxs-lookup"><span data-stu-id="5e053-147">birthday</span></span>|<span data-ttu-id="5e053-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e053-148">DateTimeOffset</span></span>|<span data-ttu-id="5e053-p107">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5e053-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5e053-152">businessPhones</span><span class="sxs-lookup"><span data-stu-id="5e053-152">businessPhones</span></span>| <span data-ttu-id="5e053-153">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5e053-153">String collection</span></span> | <span data-ttu-id="5e053-p108">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="5e053-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="5e053-156">城市</span><span class="sxs-lookup"><span data-stu-id="5e053-156">city</span></span>|<span data-ttu-id="5e053-157">String</span><span class="sxs-lookup"><span data-stu-id="5e053-157">String</span></span>|<span data-ttu-id="5e053-158">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="5e053-158">The city in which the user is located.</span></span>|
|<span data-ttu-id="5e053-159">country</span><span class="sxs-lookup"><span data-stu-id="5e053-159">country</span></span>|<span data-ttu-id="5e053-160">字符串</span><span class="sxs-lookup"><span data-stu-id="5e053-160">String</span></span>|<span data-ttu-id="5e053-161">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="5e053-161">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="5e053-162">department</span><span class="sxs-lookup"><span data-stu-id="5e053-162">department</span></span>|<span data-ttu-id="5e053-163">String</span><span class="sxs-lookup"><span data-stu-id="5e053-163">String</span></span>|<span data-ttu-id="5e053-164">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="5e053-164">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="5e053-165">displayName</span><span class="sxs-lookup"><span data-stu-id="5e053-165">displayName</span></span>|<span data-ttu-id="5e053-166">String</span><span class="sxs-lookup"><span data-stu-id="5e053-166">String</span></span>|<span data-ttu-id="5e053-p109">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="5e053-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="5e053-171">employeeId</span><span class="sxs-lookup"><span data-stu-id="5e053-171">employeeId</span></span>|<span data-ttu-id="5e053-172">String</span><span class="sxs-lookup"><span data-stu-id="5e053-172">String</span></span>|<span data-ttu-id="5e053-173">由组织分配给该用户的员工标识符。</span><span class="sxs-lookup"><span data-stu-id="5e053-173">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="5e053-174">givenName</span><span class="sxs-lookup"><span data-stu-id="5e053-174">givenName</span></span>|<span data-ttu-id="5e053-175">String</span><span class="sxs-lookup"><span data-stu-id="5e053-175">String</span></span>|<span data-ttu-id="5e053-176">用户的名。</span><span class="sxs-lookup"><span data-stu-id="5e053-176">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="5e053-177">hireDate</span><span class="sxs-lookup"><span data-stu-id="5e053-177">hireDate</span></span>|<span data-ttu-id="5e053-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e053-178">DateTimeOffset</span></span>|<span data-ttu-id="5e053-p110">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5e053-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5e053-182">interests</span><span class="sxs-lookup"><span data-stu-id="5e053-182">interests</span></span>|<span data-ttu-id="5e053-183">String collection</span><span class="sxs-lookup"><span data-stu-id="5e053-183">String collection</span></span>|<span data-ttu-id="5e053-184">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="5e053-184">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="5e053-185">jobTitle</span><span class="sxs-lookup"><span data-stu-id="5e053-185">jobTitle</span></span>|<span data-ttu-id="5e053-186">String</span><span class="sxs-lookup"><span data-stu-id="5e053-186">String</span></span>|<span data-ttu-id="5e053-187">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="5e053-187">The user’s job title.</span></span>|
|<span data-ttu-id="5e053-188">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5e053-188">mailNickname</span></span>|<span data-ttu-id="5e053-189">String</span><span class="sxs-lookup"><span data-stu-id="5e053-189">String</span></span>|<span data-ttu-id="5e053-190">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="5e053-190">The mail alias for the user.</span></span> <span data-ttu-id="5e053-191">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="5e053-191">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="5e053-192">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="5e053-192">mobilePhone</span></span>|<span data-ttu-id="5e053-193">String</span><span class="sxs-lookup"><span data-stu-id="5e053-193">String</span></span>|<span data-ttu-id="5e053-194">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="5e053-194">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="5e053-195">mySite</span><span class="sxs-lookup"><span data-stu-id="5e053-195">mySite</span></span>|<span data-ttu-id="5e053-196">String</span><span class="sxs-lookup"><span data-stu-id="5e053-196">String</span></span>|<span data-ttu-id="5e053-197">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="5e053-197">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="5e053-198">officeLocation</span><span class="sxs-lookup"><span data-stu-id="5e053-198">officeLocation</span></span>|<span data-ttu-id="5e053-199">String</span><span class="sxs-lookup"><span data-stu-id="5e053-199">String</span></span>|<span data-ttu-id="5e053-200">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="5e053-200">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="5e053-201">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="5e053-201">onPremisesImmutableId</span></span>|<span data-ttu-id="5e053-202">String</span><span class="sxs-lookup"><span data-stu-id="5e053-202">String</span></span>|<span data-ttu-id="5e053-203">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="5e053-203">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="5e053-204">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="5e053-204">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="5e053-205">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="5e053-205">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="5e053-206">otherMails</span><span class="sxs-lookup"><span data-stu-id="5e053-206">otherMails</span></span>|<span data-ttu-id="5e053-207">String</span><span class="sxs-lookup"><span data-stu-id="5e053-207">String</span></span> |<span data-ttu-id="5e053-208">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="5e053-208">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="5e053-209">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="5e053-209">passwordPolicies</span></span>|<span data-ttu-id="5e053-210">String</span><span class="sxs-lookup"><span data-stu-id="5e053-210">String</span></span>|<span data-ttu-id="5e053-p113">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="5e053-p113">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="5e053-215">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="5e053-215">passwordProfile</span></span>|[<span data-ttu-id="5e053-216">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="5e053-216">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="5e053-p114">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="5e053-p114">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="5e053-222">pastProjects</span><span class="sxs-lookup"><span data-stu-id="5e053-222">pastProjects</span></span>|<span data-ttu-id="5e053-223">String collection</span><span class="sxs-lookup"><span data-stu-id="5e053-223">String collection</span></span>|<span data-ttu-id="5e053-224">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="5e053-224">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="5e053-225">postalCode</span><span class="sxs-lookup"><span data-stu-id="5e053-225">postalCode</span></span>|<span data-ttu-id="5e053-226">String</span><span class="sxs-lookup"><span data-stu-id="5e053-226">String</span></span>|<span data-ttu-id="5e053-p115">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="5e053-p115">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="5e053-230">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="5e053-230">preferredLanguage</span></span>|<span data-ttu-id="5e053-231">String</span><span class="sxs-lookup"><span data-stu-id="5e053-231">String</span></span>|<span data-ttu-id="5e053-p116">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="5e053-p116">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="5e053-234">responsibilities</span><span class="sxs-lookup"><span data-stu-id="5e053-234">responsibilities</span></span>|<span data-ttu-id="5e053-235">String collection</span><span class="sxs-lookup"><span data-stu-id="5e053-235">String collection</span></span>|<span data-ttu-id="5e053-236">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="5e053-236">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="5e053-237">schools</span><span class="sxs-lookup"><span data-stu-id="5e053-237">schools</span></span>|<span data-ttu-id="5e053-238">String collection</span><span class="sxs-lookup"><span data-stu-id="5e053-238">String collection</span></span>|<span data-ttu-id="5e053-239">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="5e053-239">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="5e053-240">skills</span><span class="sxs-lookup"><span data-stu-id="5e053-240">skills</span></span>|<span data-ttu-id="5e053-241">String collection</span><span class="sxs-lookup"><span data-stu-id="5e053-241">String collection</span></span>|<span data-ttu-id="5e053-242">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="5e053-242">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="5e053-243">state</span><span class="sxs-lookup"><span data-stu-id="5e053-243">state</span></span>|<span data-ttu-id="5e053-244">String</span><span class="sxs-lookup"><span data-stu-id="5e053-244">String</span></span>|<span data-ttu-id="5e053-245">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="5e053-245">The state or province in the user's address.</span></span>|
|<span data-ttu-id="5e053-246">streetAddress</span><span class="sxs-lookup"><span data-stu-id="5e053-246">streetAddress</span></span>|<span data-ttu-id="5e053-247">String</span><span class="sxs-lookup"><span data-stu-id="5e053-247">String</span></span>|<span data-ttu-id="5e053-248">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="5e053-248">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="5e053-249">surname</span><span class="sxs-lookup"><span data-stu-id="5e053-249">surname</span></span>|<span data-ttu-id="5e053-250">String</span><span class="sxs-lookup"><span data-stu-id="5e053-250">String</span></span>|<span data-ttu-id="5e053-251">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="5e053-251">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="5e053-252">usageLocation</span><span class="sxs-lookup"><span data-stu-id="5e053-252">usageLocation</span></span>|<span data-ttu-id="5e053-253">字符串</span><span class="sxs-lookup"><span data-stu-id="5e053-253">String</span></span>|<span data-ttu-id="5e053-254">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="5e053-254">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="5e053-255">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="5e053-255">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="5e053-256">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="5e053-256">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="5e053-257">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5e053-257">Not nullable.</span></span>|
|<span data-ttu-id="5e053-258">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e053-258">userPrincipalName</span></span>|<span data-ttu-id="5e053-259">字符串</span><span class="sxs-lookup"><span data-stu-id="5e053-259">String</span></span>|<span data-ttu-id="5e053-p118">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="5e053-p118">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="5e053-267">userType</span><span class="sxs-lookup"><span data-stu-id="5e053-267">userType</span></span>|<span data-ttu-id="5e053-268">String</span><span class="sxs-lookup"><span data-stu-id="5e053-268">String</span></span>|<span data-ttu-id="5e053-269">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="5e053-269">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="5e053-270">由于**用户**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**用户**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="5e053-270">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="5e053-271">响应</span><span class="sxs-lookup"><span data-stu-id="5e053-271">Response</span></span>

<span data-ttu-id="5e053-272">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e053-272">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="5e053-273">示例</span><span class="sxs-lookup"><span data-stu-id="5e053-273">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e053-274">请求</span><span class="sxs-lookup"><span data-stu-id="5e053-274">Request</span></span>
<span data-ttu-id="5e053-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e053-275">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e053-276">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5e053-276">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e053-277">C#</span><span class="sxs-lookup"><span data-stu-id="5e053-277">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e053-278">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e053-278">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e053-279">目标-C</span><span class="sxs-lookup"><span data-stu-id="5e053-279">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5e053-280">Java</span><span class="sxs-lookup"><span data-stu-id="5e053-280">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e053-281">响应</span><span class="sxs-lookup"><span data-stu-id="5e053-281">Response</span></span>
<span data-ttu-id="5e053-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e053-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5e053-285">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5e053-285">See also</span></span>

- [<span data-ttu-id="5e053-286">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5e053-286">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5e053-287">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5e053-287">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5e053-288">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5e053-288">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
