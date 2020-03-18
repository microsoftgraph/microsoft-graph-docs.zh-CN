---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56276f47c3dc227cac0a53f82cb54e198d4d0c1e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799509"
---
# <a name="update-user"></a><span data-ttu-id="a09ee-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="a09ee-103">Update user</span></span>

<span data-ttu-id="a09ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a09ee-105">更新 [user](../resources/user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a09ee-105">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a09ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="a09ee-106">Permissions</span></span>
<span data-ttu-id="a09ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09ee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a09ee-109">Permission type</span></span>      | <span data-ttu-id="a09ee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a09ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a09ee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a09ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a09ee-112">"ManageIdentities"、"全部"、"全部"、"全部"、"全部"、"全部"</span><span class="sxs-lookup"><span data-stu-id="a09ee-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a09ee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a09ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a09ee-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a09ee-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="a09ee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a09ee-115">Application</span></span> | <span data-ttu-id="a09ee-116">ManageIdentities，all，all，All，All</span><span class="sxs-lookup"><span data-stu-id="a09ee-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="a09ee-117">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="a09ee-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="a09ee-118">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="a09ee-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="a09ee-119">有关详细信息，请参阅 [Azure AD 可用角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="a09ee-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="a09ee-120">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="a09ee-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="a09ee-121">更新**标识**属性需要用户 ManageIdentities 权限。</span><span class="sxs-lookup"><span data-stu-id="a09ee-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="a09ee-122">此外，不允许将[B2C 本地帐户](../resources/objectidentity.md)添加到现有**user**对象，除非该**用户**对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="a09ee-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="a09ee-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a09ee-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="a09ee-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a09ee-124">Request headers</span></span>
| <span data-ttu-id="a09ee-125">标头</span><span class="sxs-lookup"><span data-stu-id="a09ee-125">Header</span></span>       | <span data-ttu-id="a09ee-126">值</span><span class="sxs-lookup"><span data-stu-id="a09ee-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a09ee-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a09ee-127">Authorization</span></span>  | <span data-ttu-id="a09ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a09ee-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a09ee-130">Content-Type</span></span>  | <span data-ttu-id="a09ee-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a09ee-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a09ee-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a09ee-132">Request body</span></span>
<span data-ttu-id="a09ee-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a09ee-136">属性</span><span class="sxs-lookup"><span data-stu-id="a09ee-136">Property</span></span>     | <span data-ttu-id="a09ee-137">类型</span><span class="sxs-lookup"><span data-stu-id="a09ee-137">Type</span></span>   |<span data-ttu-id="a09ee-138">说明</span><span class="sxs-lookup"><span data-stu-id="a09ee-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a09ee-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="a09ee-139">aboutMe</span></span>|<span data-ttu-id="a09ee-140">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-140">String</span></span>|<span data-ttu-id="a09ee-141">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="a09ee-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="a09ee-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="a09ee-142">accountEnabled</span></span>|<span data-ttu-id="a09ee-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a09ee-143">Boolean</span></span>| <span data-ttu-id="a09ee-144">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="a09ee-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="a09ee-145">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="a09ee-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="a09ee-146">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="a09ee-146">assignedLicenses</span></span>|<span data-ttu-id="a09ee-147">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="a09ee-147">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="a09ee-p107">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="a09ee-150">birthday</span><span class="sxs-lookup"><span data-stu-id="a09ee-150">birthday</span></span>|<span data-ttu-id="a09ee-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a09ee-151">DateTimeOffset</span></span>|<span data-ttu-id="a09ee-p108">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a09ee-p108">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a09ee-155">businessPhones</span><span class="sxs-lookup"><span data-stu-id="a09ee-155">businessPhones</span></span>| <span data-ttu-id="a09ee-156">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a09ee-156">String collection</span></span> | <span data-ttu-id="a09ee-p109">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="a09ee-159">城市</span><span class="sxs-lookup"><span data-stu-id="a09ee-159">city</span></span>|<span data-ttu-id="a09ee-160">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-160">String</span></span>|<span data-ttu-id="a09ee-161">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="a09ee-161">The city in which the user is located.</span></span>|
|<span data-ttu-id="a09ee-162">country</span><span class="sxs-lookup"><span data-stu-id="a09ee-162">country</span></span>|<span data-ttu-id="a09ee-163">字符串</span><span class="sxs-lookup"><span data-stu-id="a09ee-163">String</span></span>|<span data-ttu-id="a09ee-164">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="a09ee-164">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="a09ee-165">department</span><span class="sxs-lookup"><span data-stu-id="a09ee-165">department</span></span>|<span data-ttu-id="a09ee-166">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-166">String</span></span>|<span data-ttu-id="a09ee-167">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="a09ee-167">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="a09ee-168">displayName</span><span class="sxs-lookup"><span data-stu-id="a09ee-168">displayName</span></span>|<span data-ttu-id="a09ee-169">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-169">String</span></span>|<span data-ttu-id="a09ee-p110">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="a09ee-174">employeeId</span><span class="sxs-lookup"><span data-stu-id="a09ee-174">employeeId</span></span>|<span data-ttu-id="a09ee-175">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-175">String</span></span>|<span data-ttu-id="a09ee-176">由组织分配给该用户的员工标识符。</span><span class="sxs-lookup"><span data-stu-id="a09ee-176">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="a09ee-177">givenName</span><span class="sxs-lookup"><span data-stu-id="a09ee-177">givenName</span></span>|<span data-ttu-id="a09ee-178">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-178">String</span></span>|<span data-ttu-id="a09ee-179">用户的名。</span><span class="sxs-lookup"><span data-stu-id="a09ee-179">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="a09ee-180">hireDate</span><span class="sxs-lookup"><span data-stu-id="a09ee-180">hireDate</span></span>|<span data-ttu-id="a09ee-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a09ee-181">DateTimeOffset</span></span>|<span data-ttu-id="a09ee-p111">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a09ee-p111">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a09ee-185">identities</span><span class="sxs-lookup"><span data-stu-id="a09ee-185">identities</span></span>|<span data-ttu-id="a09ee-186">[objectIdentity](../resources/objectidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a09ee-186">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="a09ee-187">表示可用于登录此用户帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="a09ee-187">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="a09ee-188">标识可由 Microsoft、组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供，并绑定到用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a09ee-188">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="a09ee-189">对**标识**的任何更新都将替换整个集合，并且您必须在集合中提供 userPrincipalName **signInType**标识。</span><span class="sxs-lookup"><span data-stu-id="a09ee-189">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="a09ee-190">interests</span><span class="sxs-lookup"><span data-stu-id="a09ee-190">interests</span></span>|<span data-ttu-id="a09ee-191">String collection</span><span class="sxs-lookup"><span data-stu-id="a09ee-191">String collection</span></span>|<span data-ttu-id="a09ee-192">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="a09ee-192">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="a09ee-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a09ee-193">jobTitle</span></span>|<span data-ttu-id="a09ee-194">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-194">String</span></span>|<span data-ttu-id="a09ee-195">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="a09ee-195">The user’s job title.</span></span>|
|<span data-ttu-id="a09ee-196">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a09ee-196">mailNickname</span></span>|<span data-ttu-id="a09ee-197">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-197">String</span></span>|<span data-ttu-id="a09ee-198">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="a09ee-198">The mail alias for the user.</span></span> <span data-ttu-id="a09ee-199">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="a09ee-199">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="a09ee-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="a09ee-200">mobilePhone</span></span>|<span data-ttu-id="a09ee-201">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-201">String</span></span>|<span data-ttu-id="a09ee-202">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="a09ee-202">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="a09ee-203">mySite</span><span class="sxs-lookup"><span data-stu-id="a09ee-203">mySite</span></span>|<span data-ttu-id="a09ee-204">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-204">String</span></span>|<span data-ttu-id="a09ee-205">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="a09ee-205">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="a09ee-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a09ee-206">officeLocation</span></span>|<span data-ttu-id="a09ee-207">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-207">String</span></span>|<span data-ttu-id="a09ee-208">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="a09ee-208">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="a09ee-209">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="a09ee-209">onPremisesImmutableId</span></span>|<span data-ttu-id="a09ee-210">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-210">String</span></span>|<span data-ttu-id="a09ee-211">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="a09ee-211">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="a09ee-212">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="a09ee-212">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="a09ee-213">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="a09ee-213">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="a09ee-214">otherMails</span><span class="sxs-lookup"><span data-stu-id="a09ee-214">otherMails</span></span>|<span data-ttu-id="a09ee-215">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-215">String</span></span> |<span data-ttu-id="a09ee-216">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="a09ee-216">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="a09ee-217">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="a09ee-217">passwordPolicies</span></span>|<span data-ttu-id="a09ee-218">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-218">String</span></span>|<span data-ttu-id="a09ee-p115">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p115">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="a09ee-223">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="a09ee-223">passwordProfile</span></span>|[<span data-ttu-id="a09ee-224">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="a09ee-224">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="a09ee-p116">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p116">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="a09ee-230">pastProjects</span><span class="sxs-lookup"><span data-stu-id="a09ee-230">pastProjects</span></span>|<span data-ttu-id="a09ee-231">String collection</span><span class="sxs-lookup"><span data-stu-id="a09ee-231">String collection</span></span>|<span data-ttu-id="a09ee-232">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="a09ee-232">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="a09ee-233">postalCode</span><span class="sxs-lookup"><span data-stu-id="a09ee-233">postalCode</span></span>|<span data-ttu-id="a09ee-234">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-234">String</span></span>|<span data-ttu-id="a09ee-p117">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p117">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="a09ee-238">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="a09ee-238">preferredLanguage</span></span>|<span data-ttu-id="a09ee-239">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-239">String</span></span>|<span data-ttu-id="a09ee-p118">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p118">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="a09ee-242">responsibilities</span><span class="sxs-lookup"><span data-stu-id="a09ee-242">responsibilities</span></span>|<span data-ttu-id="a09ee-243">String collection</span><span class="sxs-lookup"><span data-stu-id="a09ee-243">String collection</span></span>|<span data-ttu-id="a09ee-244">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="a09ee-244">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="a09ee-245">schools</span><span class="sxs-lookup"><span data-stu-id="a09ee-245">schools</span></span>|<span data-ttu-id="a09ee-246">String collection</span><span class="sxs-lookup"><span data-stu-id="a09ee-246">String collection</span></span>|<span data-ttu-id="a09ee-247">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="a09ee-247">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="a09ee-248">skills</span><span class="sxs-lookup"><span data-stu-id="a09ee-248">skills</span></span>|<span data-ttu-id="a09ee-249">String collection</span><span class="sxs-lookup"><span data-stu-id="a09ee-249">String collection</span></span>|<span data-ttu-id="a09ee-250">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="a09ee-250">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="a09ee-251">state</span><span class="sxs-lookup"><span data-stu-id="a09ee-251">state</span></span>|<span data-ttu-id="a09ee-252">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-252">String</span></span>|<span data-ttu-id="a09ee-253">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="a09ee-253">The state or province in the user's address.</span></span>|
|<span data-ttu-id="a09ee-254">streetAddress</span><span class="sxs-lookup"><span data-stu-id="a09ee-254">streetAddress</span></span>|<span data-ttu-id="a09ee-255">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-255">String</span></span>|<span data-ttu-id="a09ee-256">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="a09ee-256">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="a09ee-257">surname</span><span class="sxs-lookup"><span data-stu-id="a09ee-257">surname</span></span>|<span data-ttu-id="a09ee-258">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-258">String</span></span>|<span data-ttu-id="a09ee-259">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="a09ee-259">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="a09ee-260">usageLocation</span><span class="sxs-lookup"><span data-stu-id="a09ee-260">usageLocation</span></span>|<span data-ttu-id="a09ee-261">字符串</span><span class="sxs-lookup"><span data-stu-id="a09ee-261">String</span></span>|<span data-ttu-id="a09ee-262">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="a09ee-262">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="a09ee-263">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="a09ee-263">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="a09ee-264">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="a09ee-264">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="a09ee-265">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="a09ee-265">Not nullable.</span></span>|
|<span data-ttu-id="a09ee-266">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a09ee-266">userPrincipalName</span></span>|<span data-ttu-id="a09ee-267">字符串</span><span class="sxs-lookup"><span data-stu-id="a09ee-267">String</span></span>|<span data-ttu-id="a09ee-p120">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="a09ee-p120">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="a09ee-275">userType</span><span class="sxs-lookup"><span data-stu-id="a09ee-275">userType</span></span>|<span data-ttu-id="a09ee-276">String</span><span class="sxs-lookup"><span data-stu-id="a09ee-276">String</span></span>|<span data-ttu-id="a09ee-277">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="a09ee-277">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="a09ee-278">由于**用户**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用该`PATCH`操作在现有**用户**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="a09ee-278">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a09ee-279">响应</span><span class="sxs-lookup"><span data-stu-id="a09ee-279">Response</span></span>

<span data-ttu-id="a09ee-280">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a09ee-280">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a09ee-281">示例</span><span class="sxs-lookup"><span data-stu-id="a09ee-281">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="a09ee-282">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="a09ee-282">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="a09ee-283">请求</span><span class="sxs-lookup"><span data-stu-id="a09ee-283">Request</span></span>

<span data-ttu-id="a09ee-284">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="a09ee-284">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a09ee-285">HTTP</span><span class="sxs-lookup"><span data-stu-id="a09ee-285">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a09ee-286">C#</span><span class="sxs-lookup"><span data-stu-id="a09ee-286">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a09ee-287">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a09ee-287">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a09ee-288">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a09ee-288">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a09ee-289">响应</span><span class="sxs-lookup"><span data-stu-id="a09ee-289">Response</span></span>

<span data-ttu-id="a09ee-290">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a09ee-290">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="a09ee-291">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="a09ee-291">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="a09ee-292">请求</span><span class="sxs-lookup"><span data-stu-id="a09ee-292">Request</span></span>

<span data-ttu-id="a09ee-293">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="a09ee-293">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a09ee-294">HTTP</span><span class="sxs-lookup"><span data-stu-id="a09ee-294">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a09ee-295">C#</span><span class="sxs-lookup"><span data-stu-id="a09ee-295">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a09ee-296">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a09ee-296">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a09ee-297">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a09ee-297">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a09ee-298">响应</span><span class="sxs-lookup"><span data-stu-id="a09ee-298">Response</span></span>

<span data-ttu-id="a09ee-299">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a09ee-299">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a09ee-300">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a09ee-300">See also</span></span>

- [<span data-ttu-id="a09ee-301">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a09ee-301">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a09ee-302">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a09ee-302">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a09ee-303">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a09ee-303">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
