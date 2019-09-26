---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1662290791eb996d74f045a032d5f1b581121205
ms.sourcegitcommit: 8ef30790a4d7aa94879df93773eae80b37abbfa4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37203968"
---
# <a name="update-user"></a><span data-ttu-id="fe627-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="fe627-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe627-104">更新 [user](../resources/user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe627-104">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe627-105">权限</span><span class="sxs-lookup"><span data-stu-id="fe627-105">Permissions</span></span>
<span data-ttu-id="fe627-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe627-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe627-108">Permission type</span></span>      | <span data-ttu-id="fe627-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe627-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe627-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe627-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe627-111">所有的用户读写全部。所有</span><span class="sxs-lookup"><span data-stu-id="fe627-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe627-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe627-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe627-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe627-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="fe627-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe627-114">Application</span></span> | <span data-ttu-id="fe627-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe627-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="fe627-116">更新**passwordProfile**属性时，需要以下权限： directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="fe627-116">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="fe627-117">仅允许非管理员用户或分配了以下角色之一的用户更新另一个用户的**businessPhones**、 **mobilePhone**或**OtherMails**属性：目录读取器、来宾邀请者、消息中心读取器和报告读取器。</span><span class="sxs-lookup"><span data-stu-id="fe627-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="fe627-118">有关更多详细信息，请参阅[AZURE AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="fe627-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="fe627-119">对于授予了 User. ReadWrite、All 或 Directory 的所有委派或应用程序权限的应用程序，情况也是如此。</span><span class="sxs-lookup"><span data-stu-id="fe627-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="fe627-120">更新**标识**属性需要用户 ManageIdentities 权限。</span><span class="sxs-lookup"><span data-stu-id="fe627-120">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="fe627-121">此外，不允许将[B2C 本地帐户](../resources/objectidentity.md)添加到现有**user**对象，除非该**用户**对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="fe627-121">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe627-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe627-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="fe627-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe627-123">Request headers</span></span>
| <span data-ttu-id="fe627-124">标头</span><span class="sxs-lookup"><span data-stu-id="fe627-124">Header</span></span>       | <span data-ttu-id="fe627-125">值</span><span class="sxs-lookup"><span data-stu-id="fe627-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="fe627-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe627-126">Authorization</span></span>  | <span data-ttu-id="fe627-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe627-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe627-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe627-129">Content-Type</span></span>  | <span data-ttu-id="fe627-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fe627-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe627-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe627-131">Request body</span></span>
<span data-ttu-id="fe627-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fe627-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fe627-135">属性</span><span class="sxs-lookup"><span data-stu-id="fe627-135">Property</span></span>     | <span data-ttu-id="fe627-136">类型</span><span class="sxs-lookup"><span data-stu-id="fe627-136">Type</span></span>   |<span data-ttu-id="fe627-137">说明</span><span class="sxs-lookup"><span data-stu-id="fe627-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe627-138">aboutMe</span><span class="sxs-lookup"><span data-stu-id="fe627-138">aboutMe</span></span>|<span data-ttu-id="fe627-139">String</span><span class="sxs-lookup"><span data-stu-id="fe627-139">String</span></span>|<span data-ttu-id="fe627-140">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="fe627-140">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="fe627-141">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="fe627-141">accountEnabled</span></span>|<span data-ttu-id="fe627-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe627-142">Boolean</span></span>| <span data-ttu-id="fe627-143">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="fe627-143">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="fe627-144">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="fe627-144">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="fe627-145">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="fe627-145">assignedLicenses</span></span>|<span data-ttu-id="fe627-146">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe627-146">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="fe627-p107">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fe627-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="fe627-149">birthday</span><span class="sxs-lookup"><span data-stu-id="fe627-149">birthday</span></span>|<span data-ttu-id="fe627-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe627-150">DateTimeOffset</span></span>|<span data-ttu-id="fe627-p108">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fe627-p108">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fe627-154">businessPhones</span><span class="sxs-lookup"><span data-stu-id="fe627-154">businessPhones</span></span>| <span data-ttu-id="fe627-155">字符串集合</span><span class="sxs-lookup"><span data-stu-id="fe627-155">String collection</span></span> | <span data-ttu-id="fe627-p109">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="fe627-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="fe627-158">城市</span><span class="sxs-lookup"><span data-stu-id="fe627-158">city</span></span>|<span data-ttu-id="fe627-159">String</span><span class="sxs-lookup"><span data-stu-id="fe627-159">String</span></span>|<span data-ttu-id="fe627-160">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="fe627-160">The city in which the user is located.</span></span>|
|<span data-ttu-id="fe627-161">country</span><span class="sxs-lookup"><span data-stu-id="fe627-161">country</span></span>|<span data-ttu-id="fe627-162">字符串</span><span class="sxs-lookup"><span data-stu-id="fe627-162">String</span></span>|<span data-ttu-id="fe627-163">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="fe627-163">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="fe627-164">department</span><span class="sxs-lookup"><span data-stu-id="fe627-164">department</span></span>|<span data-ttu-id="fe627-165">String</span><span class="sxs-lookup"><span data-stu-id="fe627-165">String</span></span>|<span data-ttu-id="fe627-166">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="fe627-166">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="fe627-167">displayName</span><span class="sxs-lookup"><span data-stu-id="fe627-167">displayName</span></span>|<span data-ttu-id="fe627-168">String</span><span class="sxs-lookup"><span data-stu-id="fe627-168">String</span></span>|<span data-ttu-id="fe627-p110">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="fe627-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="fe627-173">employeeId</span><span class="sxs-lookup"><span data-stu-id="fe627-173">employeeId</span></span>|<span data-ttu-id="fe627-174">String</span><span class="sxs-lookup"><span data-stu-id="fe627-174">String</span></span>|<span data-ttu-id="fe627-175">由组织分配给该用户的员工标识符。</span><span class="sxs-lookup"><span data-stu-id="fe627-175">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="fe627-176">givenName</span><span class="sxs-lookup"><span data-stu-id="fe627-176">givenName</span></span>|<span data-ttu-id="fe627-177">String</span><span class="sxs-lookup"><span data-stu-id="fe627-177">String</span></span>|<span data-ttu-id="fe627-178">用户的名。</span><span class="sxs-lookup"><span data-stu-id="fe627-178">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="fe627-179">hireDate</span><span class="sxs-lookup"><span data-stu-id="fe627-179">hireDate</span></span>|<span data-ttu-id="fe627-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe627-180">DateTimeOffset</span></span>|<span data-ttu-id="fe627-p111">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fe627-p111">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fe627-184">身份</span><span class="sxs-lookup"><span data-stu-id="fe627-184">identities</span></span>|<span data-ttu-id="fe627-185">[objectIdentity](../resources/objectidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe627-185">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="fe627-186">表示可用于登录此用户帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="fe627-186">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="fe627-187">标识可由 Microsoft、组织或社会身份提供商（如 Facebook、Google 和 Microsoft）提供，并绑定到用户帐户。</span><span class="sxs-lookup"><span data-stu-id="fe627-187">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="fe627-188">对**标识**的任何更新都将替换整个集合，并且您必须在集合中提供 userPrincipalName **signInType**标识。</span><span class="sxs-lookup"><span data-stu-id="fe627-188">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="fe627-189">interests</span><span class="sxs-lookup"><span data-stu-id="fe627-189">interests</span></span>|<span data-ttu-id="fe627-190">String collection</span><span class="sxs-lookup"><span data-stu-id="fe627-190">String collection</span></span>|<span data-ttu-id="fe627-191">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="fe627-191">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="fe627-192">jobTitle</span><span class="sxs-lookup"><span data-stu-id="fe627-192">jobTitle</span></span>|<span data-ttu-id="fe627-193">String</span><span class="sxs-lookup"><span data-stu-id="fe627-193">String</span></span>|<span data-ttu-id="fe627-194">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="fe627-194">The user’s job title.</span></span>|
|<span data-ttu-id="fe627-195">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fe627-195">mailNickname</span></span>|<span data-ttu-id="fe627-196">String</span><span class="sxs-lookup"><span data-stu-id="fe627-196">String</span></span>|<span data-ttu-id="fe627-197">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="fe627-197">The mail alias for the user.</span></span> <span data-ttu-id="fe627-198">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="fe627-198">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="fe627-199">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="fe627-199">mobilePhone</span></span>|<span data-ttu-id="fe627-200">String</span><span class="sxs-lookup"><span data-stu-id="fe627-200">String</span></span>|<span data-ttu-id="fe627-201">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="fe627-201">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="fe627-202">mySite</span><span class="sxs-lookup"><span data-stu-id="fe627-202">mySite</span></span>|<span data-ttu-id="fe627-203">String</span><span class="sxs-lookup"><span data-stu-id="fe627-203">String</span></span>|<span data-ttu-id="fe627-204">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="fe627-204">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="fe627-205">officeLocation</span><span class="sxs-lookup"><span data-stu-id="fe627-205">officeLocation</span></span>|<span data-ttu-id="fe627-206">String</span><span class="sxs-lookup"><span data-stu-id="fe627-206">String</span></span>|<span data-ttu-id="fe627-207">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="fe627-207">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="fe627-208">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="fe627-208">onPremisesImmutableId</span></span>|<span data-ttu-id="fe627-209">String</span><span class="sxs-lookup"><span data-stu-id="fe627-209">String</span></span>|<span data-ttu-id="fe627-210">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="fe627-210">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="fe627-211">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="fe627-211">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="fe627-212">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="fe627-212">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="fe627-213">otherMails</span><span class="sxs-lookup"><span data-stu-id="fe627-213">otherMails</span></span>|<span data-ttu-id="fe627-214">String</span><span class="sxs-lookup"><span data-stu-id="fe627-214">String</span></span> |<span data-ttu-id="fe627-215">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="fe627-215">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="fe627-216">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="fe627-216">passwordPolicies</span></span>|<span data-ttu-id="fe627-217">String</span><span class="sxs-lookup"><span data-stu-id="fe627-217">String</span></span>|<span data-ttu-id="fe627-p115">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="fe627-p115">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="fe627-222">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="fe627-222">passwordProfile</span></span>|[<span data-ttu-id="fe627-223">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="fe627-223">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="fe627-p116">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="fe627-p116">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="fe627-229">pastProjects</span><span class="sxs-lookup"><span data-stu-id="fe627-229">pastProjects</span></span>|<span data-ttu-id="fe627-230">String collection</span><span class="sxs-lookup"><span data-stu-id="fe627-230">String collection</span></span>|<span data-ttu-id="fe627-231">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="fe627-231">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="fe627-232">postalCode</span><span class="sxs-lookup"><span data-stu-id="fe627-232">postalCode</span></span>|<span data-ttu-id="fe627-233">String</span><span class="sxs-lookup"><span data-stu-id="fe627-233">String</span></span>|<span data-ttu-id="fe627-p117">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="fe627-p117">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="fe627-237">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="fe627-237">preferredLanguage</span></span>|<span data-ttu-id="fe627-238">String</span><span class="sxs-lookup"><span data-stu-id="fe627-238">String</span></span>|<span data-ttu-id="fe627-p118">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="fe627-p118">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="fe627-241">responsibilities</span><span class="sxs-lookup"><span data-stu-id="fe627-241">responsibilities</span></span>|<span data-ttu-id="fe627-242">String collection</span><span class="sxs-lookup"><span data-stu-id="fe627-242">String collection</span></span>|<span data-ttu-id="fe627-243">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="fe627-243">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="fe627-244">schools</span><span class="sxs-lookup"><span data-stu-id="fe627-244">schools</span></span>|<span data-ttu-id="fe627-245">String collection</span><span class="sxs-lookup"><span data-stu-id="fe627-245">String collection</span></span>|<span data-ttu-id="fe627-246">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="fe627-246">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="fe627-247">skills</span><span class="sxs-lookup"><span data-stu-id="fe627-247">skills</span></span>|<span data-ttu-id="fe627-248">String collection</span><span class="sxs-lookup"><span data-stu-id="fe627-248">String collection</span></span>|<span data-ttu-id="fe627-249">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="fe627-249">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="fe627-250">state</span><span class="sxs-lookup"><span data-stu-id="fe627-250">state</span></span>|<span data-ttu-id="fe627-251">String</span><span class="sxs-lookup"><span data-stu-id="fe627-251">String</span></span>|<span data-ttu-id="fe627-252">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="fe627-252">The state or province in the user's address.</span></span>|
|<span data-ttu-id="fe627-253">streetAddress</span><span class="sxs-lookup"><span data-stu-id="fe627-253">streetAddress</span></span>|<span data-ttu-id="fe627-254">String</span><span class="sxs-lookup"><span data-stu-id="fe627-254">String</span></span>|<span data-ttu-id="fe627-255">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="fe627-255">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="fe627-256">surname</span><span class="sxs-lookup"><span data-stu-id="fe627-256">surname</span></span>|<span data-ttu-id="fe627-257">String</span><span class="sxs-lookup"><span data-stu-id="fe627-257">String</span></span>|<span data-ttu-id="fe627-258">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="fe627-258">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="fe627-259">usageLocation</span><span class="sxs-lookup"><span data-stu-id="fe627-259">usageLocation</span></span>|<span data-ttu-id="fe627-260">字符串</span><span class="sxs-lookup"><span data-stu-id="fe627-260">String</span></span>|<span data-ttu-id="fe627-261">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="fe627-261">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="fe627-262">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="fe627-262">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="fe627-263">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="fe627-263">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="fe627-264">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fe627-264">Not nullable.</span></span>|
|<span data-ttu-id="fe627-265">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe627-265">userPrincipalName</span></span>|<span data-ttu-id="fe627-266">字符串</span><span class="sxs-lookup"><span data-stu-id="fe627-266">String</span></span>|<span data-ttu-id="fe627-p120">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="fe627-p120">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="fe627-274">userType</span><span class="sxs-lookup"><span data-stu-id="fe627-274">userType</span></span>|<span data-ttu-id="fe627-275">String</span><span class="sxs-lookup"><span data-stu-id="fe627-275">String</span></span>|<span data-ttu-id="fe627-276">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="fe627-276">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="fe627-277">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用该`PATCH`操作在现有**用户**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="fe627-277">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="fe627-278">响应</span><span class="sxs-lookup"><span data-stu-id="fe627-278">Response</span></span>

<span data-ttu-id="fe627-279">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fe627-279">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe627-280">示例</span><span class="sxs-lookup"><span data-stu-id="fe627-280">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="fe627-281">示例1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="fe627-281">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="fe627-282">请求</span><span class="sxs-lookup"><span data-stu-id="fe627-282">Request</span></span>

<span data-ttu-id="fe627-283">下面的示例演示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="fe627-283">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe627-284">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fe627-284">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe627-285">C#</span><span class="sxs-lookup"><span data-stu-id="fe627-285">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe627-286">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe627-286">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe627-287">目标-C</span><span class="sxs-lookup"><span data-stu-id="fe627-287">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="fe627-288">响应</span><span class="sxs-lookup"><span data-stu-id="fe627-288">Response</span></span>

<span data-ttu-id="fe627-289">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="fe627-289">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="fe627-290">示例2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="fe627-290">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="fe627-291">请求</span><span class="sxs-lookup"><span data-stu-id="fe627-291">Request</span></span>

<span data-ttu-id="fe627-292">下面的示例演示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="fe627-292">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe627-293">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fe627-293">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe627-294">C#</span><span class="sxs-lookup"><span data-stu-id="fe627-294">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe627-295">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe627-295">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe627-296">目标-C</span><span class="sxs-lookup"><span data-stu-id="fe627-296">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fe627-297">响应</span><span class="sxs-lookup"><span data-stu-id="fe627-297">Response</span></span>

<span data-ttu-id="fe627-298">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="fe627-298">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="fe627-299">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fe627-299">See also</span></span>

- [<span data-ttu-id="fe627-300">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fe627-300">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fe627-301">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fe627-301">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fe627-302">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fe627-302">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
