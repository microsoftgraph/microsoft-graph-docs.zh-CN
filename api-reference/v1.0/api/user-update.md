---
title: 更新用户
description: 更新 user 对象的属性。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dddcccadb27efd4bf5b25a3479df56a3ef5e7049
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582063"
---
# <a name="update-user"></a><span data-ttu-id="9768b-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="9768b-103">Update user</span></span>

<span data-ttu-id="9768b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9768b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9768b-105">更新 user 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9768b-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9768b-106">权限</span><span class="sxs-lookup"><span data-stu-id="9768b-106">Permissions</span></span>
<span data-ttu-id="9768b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9768b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9768b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9768b-109">Permission type</span></span>      | <span data-ttu-id="9768b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9768b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9768b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9768b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9768b-112">User.ReadWrite、User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9768b-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9768b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9768b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9768b-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9768b-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="9768b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9768b-115">Application</span></span> | <span data-ttu-id="9768b-116">User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9768b-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="9768b-117">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="9768b-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="9768b-118">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="9768b-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="9768b-119">有关详细信息，请参阅 [Azure AD 可用角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。</span><span class="sxs-lookup"><span data-stu-id="9768b-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="9768b-120">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="9768b-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="9768b-121">更新 **identities** 属性需要 User.ManageIdentities.All 权限。</span><span class="sxs-lookup"><span data-stu-id="9768b-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="9768b-122">此外，不允许将 [B2C 本地帐户](../resources/objectidentity.md)添加到现有 **user** 对象，除非 **user** 对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="9768b-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="9768b-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9768b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="9768b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9768b-124">Request headers</span></span>
| <span data-ttu-id="9768b-125">标头</span><span class="sxs-lookup"><span data-stu-id="9768b-125">Header</span></span>       | <span data-ttu-id="9768b-126">值</span><span class="sxs-lookup"><span data-stu-id="9768b-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9768b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9768b-127">Authorization</span></span>  | <span data-ttu-id="9768b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9768b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9768b-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9768b-130">Content-Type</span></span>  | <span data-ttu-id="9768b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="9768b-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9768b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="9768b-132">Request body</span></span>
<span data-ttu-id="9768b-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9768b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9768b-136">属性</span><span class="sxs-lookup"><span data-stu-id="9768b-136">Property</span></span>     | <span data-ttu-id="9768b-137">类型</span><span class="sxs-lookup"><span data-stu-id="9768b-137">Type</span></span>   |<span data-ttu-id="9768b-138">说明</span><span class="sxs-lookup"><span data-stu-id="9768b-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9768b-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="9768b-139">aboutMe</span></span>|<span data-ttu-id="9768b-140">String</span><span class="sxs-lookup"><span data-stu-id="9768b-140">String</span></span>|<span data-ttu-id="9768b-141">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="9768b-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="9768b-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="9768b-142">accountEnabled</span></span>|<span data-ttu-id="9768b-143">布尔</span><span class="sxs-lookup"><span data-stu-id="9768b-143">Boolean</span></span>| <span data-ttu-id="9768b-144">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="9768b-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="9768b-145">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="9768b-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="9768b-146">birthday</span><span class="sxs-lookup"><span data-stu-id="9768b-146">birthday</span></span>|<span data-ttu-id="9768b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9768b-147">DateTimeOffset</span></span>|<span data-ttu-id="9768b-p107">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9768b-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9768b-151">businessPhones</span><span class="sxs-lookup"><span data-stu-id="9768b-151">businessPhones</span></span>| <span data-ttu-id="9768b-152">String collection</span><span class="sxs-lookup"><span data-stu-id="9768b-152">String collection</span></span> | <span data-ttu-id="9768b-p108">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="9768b-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="9768b-155">城市</span><span class="sxs-lookup"><span data-stu-id="9768b-155">city</span></span>|<span data-ttu-id="9768b-156">String</span><span class="sxs-lookup"><span data-stu-id="9768b-156">String</span></span>|<span data-ttu-id="9768b-157">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="9768b-157">The city in which the user is located.</span></span>|
|<span data-ttu-id="9768b-158">country</span><span class="sxs-lookup"><span data-stu-id="9768b-158">country</span></span>|<span data-ttu-id="9768b-159">String</span><span class="sxs-lookup"><span data-stu-id="9768b-159">String</span></span>|<span data-ttu-id="9768b-160">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="9768b-160">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="9768b-161">department</span><span class="sxs-lookup"><span data-stu-id="9768b-161">department</span></span>|<span data-ttu-id="9768b-162">String</span><span class="sxs-lookup"><span data-stu-id="9768b-162">String</span></span>|<span data-ttu-id="9768b-163">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="9768b-163">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="9768b-164">displayName</span><span class="sxs-lookup"><span data-stu-id="9768b-164">displayName</span></span>|<span data-ttu-id="9768b-165">String</span><span class="sxs-lookup"><span data-stu-id="9768b-165">String</span></span>|<span data-ttu-id="9768b-p109">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="9768b-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="9768b-170">givenName</span><span class="sxs-lookup"><span data-stu-id="9768b-170">givenName</span></span>|<span data-ttu-id="9768b-171">String</span><span class="sxs-lookup"><span data-stu-id="9768b-171">String</span></span>|<span data-ttu-id="9768b-172">用户的名。</span><span class="sxs-lookup"><span data-stu-id="9768b-172">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="9768b-173">hireDate</span><span class="sxs-lookup"><span data-stu-id="9768b-173">hireDate</span></span>|<span data-ttu-id="9768b-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9768b-174">DateTimeOffset</span></span>|<span data-ttu-id="9768b-p110">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9768b-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9768b-178">interests</span><span class="sxs-lookup"><span data-stu-id="9768b-178">interests</span></span>|<span data-ttu-id="9768b-179">String collection</span><span class="sxs-lookup"><span data-stu-id="9768b-179">String collection</span></span>|<span data-ttu-id="9768b-180">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="9768b-180">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="9768b-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="9768b-181">jobTitle</span></span>|<span data-ttu-id="9768b-182">String</span><span class="sxs-lookup"><span data-stu-id="9768b-182">String</span></span>|<span data-ttu-id="9768b-183">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="9768b-183">The user’s job title.</span></span>|
|<span data-ttu-id="9768b-184">mail</span><span class="sxs-lookup"><span data-stu-id="9768b-184">mail</span></span>|<span data-ttu-id="9768b-185">String</span><span class="sxs-lookup"><span data-stu-id="9768b-185">String</span></span>|<span data-ttu-id="9768b-186">用户的 SMTP 地址，例如，“jeff@contoso.onmicrosoft.com”。</span><span class="sxs-lookup"><span data-stu-id="9768b-186">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="9768b-187">对此属性的更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="9768b-187">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="9768b-188">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="9768b-188">Supports $filter.</span></span>|
|<span data-ttu-id="9768b-189">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9768b-189">mailNickname</span></span>|<span data-ttu-id="9768b-190">String</span><span class="sxs-lookup"><span data-stu-id="9768b-190">String</span></span>|<span data-ttu-id="9768b-191">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="9768b-191">The mail alias for the user.</span></span> <span data-ttu-id="9768b-192">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="9768b-192">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="9768b-193">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="9768b-193">mobilePhone</span></span>|<span data-ttu-id="9768b-194">String</span><span class="sxs-lookup"><span data-stu-id="9768b-194">String</span></span>|<span data-ttu-id="9768b-195">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="9768b-195">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="9768b-196">mySite</span><span class="sxs-lookup"><span data-stu-id="9768b-196">mySite</span></span>|<span data-ttu-id="9768b-197">String</span><span class="sxs-lookup"><span data-stu-id="9768b-197">String</span></span>|<span data-ttu-id="9768b-198">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="9768b-198">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="9768b-199">officeLocation</span><span class="sxs-lookup"><span data-stu-id="9768b-199">officeLocation</span></span>|<span data-ttu-id="9768b-200">String</span><span class="sxs-lookup"><span data-stu-id="9768b-200">String</span></span>|<span data-ttu-id="9768b-201">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="9768b-201">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="9768b-202">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="9768b-202">onPremisesImmutableId</span></span>|<span data-ttu-id="9768b-203">String</span><span class="sxs-lookup"><span data-stu-id="9768b-203">String</span></span>|<span data-ttu-id="9768b-204">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="9768b-204">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="9768b-205">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="9768b-205">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="9768b-206">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="9768b-206">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="9768b-207">otherMails</span><span class="sxs-lookup"><span data-stu-id="9768b-207">otherMails</span></span>|<span data-ttu-id="9768b-208">String</span><span class="sxs-lookup"><span data-stu-id="9768b-208">String</span></span> |<span data-ttu-id="9768b-209">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="9768b-209">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="9768b-210">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="9768b-210">passwordPolicies</span></span>|<span data-ttu-id="9768b-211">String</span><span class="sxs-lookup"><span data-stu-id="9768b-211">String</span></span>|<span data-ttu-id="9768b-p114">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="9768b-p114">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="9768b-216">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="9768b-216">passwordProfile</span></span>|[<span data-ttu-id="9768b-217">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="9768b-217">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="9768b-p115">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="9768b-p115">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="9768b-223">pastProjects</span><span class="sxs-lookup"><span data-stu-id="9768b-223">pastProjects</span></span>|<span data-ttu-id="9768b-224">String collection</span><span class="sxs-lookup"><span data-stu-id="9768b-224">String collection</span></span>|<span data-ttu-id="9768b-225">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="9768b-225">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="9768b-226">postalCode</span><span class="sxs-lookup"><span data-stu-id="9768b-226">postalCode</span></span>|<span data-ttu-id="9768b-227">String</span><span class="sxs-lookup"><span data-stu-id="9768b-227">String</span></span>|<span data-ttu-id="9768b-p116">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="9768b-p116">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="9768b-231">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="9768b-231">preferredLanguage</span></span>|<span data-ttu-id="9768b-232">String</span><span class="sxs-lookup"><span data-stu-id="9768b-232">String</span></span>|<span data-ttu-id="9768b-p117">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="9768b-p117">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="9768b-235">responsibilities</span><span class="sxs-lookup"><span data-stu-id="9768b-235">responsibilities</span></span>|<span data-ttu-id="9768b-236">String collection</span><span class="sxs-lookup"><span data-stu-id="9768b-236">String collection</span></span>|<span data-ttu-id="9768b-237">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="9768b-237">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="9768b-238">schools</span><span class="sxs-lookup"><span data-stu-id="9768b-238">schools</span></span>|<span data-ttu-id="9768b-239">String collection</span><span class="sxs-lookup"><span data-stu-id="9768b-239">String collection</span></span>|<span data-ttu-id="9768b-240">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="9768b-240">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="9768b-241">skills</span><span class="sxs-lookup"><span data-stu-id="9768b-241">skills</span></span>|<span data-ttu-id="9768b-242">String collection</span><span class="sxs-lookup"><span data-stu-id="9768b-242">String collection</span></span>|<span data-ttu-id="9768b-243">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="9768b-243">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="9768b-244">state</span><span class="sxs-lookup"><span data-stu-id="9768b-244">state</span></span>|<span data-ttu-id="9768b-245">String</span><span class="sxs-lookup"><span data-stu-id="9768b-245">String</span></span>|<span data-ttu-id="9768b-246">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="9768b-246">The state or province in the user's address.</span></span>|
|<span data-ttu-id="9768b-247">streetAddress</span><span class="sxs-lookup"><span data-stu-id="9768b-247">streetAddress</span></span>|<span data-ttu-id="9768b-248">String</span><span class="sxs-lookup"><span data-stu-id="9768b-248">String</span></span>|<span data-ttu-id="9768b-249">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="9768b-249">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="9768b-250">surname</span><span class="sxs-lookup"><span data-stu-id="9768b-250">surname</span></span>|<span data-ttu-id="9768b-251">String</span><span class="sxs-lookup"><span data-stu-id="9768b-251">String</span></span>|<span data-ttu-id="9768b-252">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="9768b-252">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="9768b-253">usageLocation</span><span class="sxs-lookup"><span data-stu-id="9768b-253">usageLocation</span></span>|<span data-ttu-id="9768b-254">String</span><span class="sxs-lookup"><span data-stu-id="9768b-254">String</span></span>|<span data-ttu-id="9768b-255">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="9768b-255">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="9768b-256">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="9768b-256">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="9768b-257">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="9768b-257">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="9768b-258">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9768b-258">Not nullable.</span></span>|
|<span data-ttu-id="9768b-259">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9768b-259">userPrincipalName</span></span>|<span data-ttu-id="9768b-260">String</span><span class="sxs-lookup"><span data-stu-id="9768b-260">String</span></span>|<span data-ttu-id="9768b-p119">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="9768b-p119">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="9768b-268">userType</span><span class="sxs-lookup"><span data-stu-id="9768b-268">userType</span></span>|<span data-ttu-id="9768b-269">String</span><span class="sxs-lookup"><span data-stu-id="9768b-269">String</span></span>|<span data-ttu-id="9768b-270">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。</span><span class="sxs-lookup"><span data-stu-id="9768b-270">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="9768b-271">以下属性无法使用仅限应用程序上下文进行更新：**aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**。</span><span class="sxs-lookup"><span data-stu-id="9768b-271">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="9768b-272">响应</span><span class="sxs-lookup"><span data-stu-id="9768b-272">Response</span></span>

<span data-ttu-id="9768b-273">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9768b-273">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9768b-274">示例</span><span class="sxs-lookup"><span data-stu-id="9768b-274">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="9768b-275">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="9768b-275">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="9768b-276">请求</span><span class="sxs-lookup"><span data-stu-id="9768b-276">Request</span></span>

<span data-ttu-id="9768b-277">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="9768b-277">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9768b-278">HTTP</span><span class="sxs-lookup"><span data-stu-id="9768b-278">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9768b-279">C#</span><span class="sxs-lookup"><span data-stu-id="9768b-279">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9768b-280">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9768b-280">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9768b-281">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9768b-281">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9768b-282">Java</span><span class="sxs-lookup"><span data-stu-id="9768b-282">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9768b-283">响应</span><span class="sxs-lookup"><span data-stu-id="9768b-283">Response</span></span>
<span data-ttu-id="9768b-284">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="9768b-284">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="9768b-285">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="9768b-285">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="9768b-286">请求</span><span class="sxs-lookup"><span data-stu-id="9768b-286">Request</span></span>

<span data-ttu-id="9768b-287">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="9768b-287">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9768b-288">HTTP</span><span class="sxs-lookup"><span data-stu-id="9768b-288">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9768b-289">C#</span><span class="sxs-lookup"><span data-stu-id="9768b-289">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9768b-290">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9768b-290">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9768b-291">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9768b-291">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9768b-292">Java</span><span class="sxs-lookup"><span data-stu-id="9768b-292">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9768b-293">响应</span><span class="sxs-lookup"><span data-stu-id="9768b-293">Response</span></span>

<span data-ttu-id="9768b-294">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="9768b-294">The following example shows the response.</span></span>
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