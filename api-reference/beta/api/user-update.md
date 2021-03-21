---
title: 更新用户
description: 更新 user 对象的属性。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 085bd1e6037b6269ed573d4f684b51220b7ce775
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955349"
---
# <a name="update-user"></a><span data-ttu-id="0e915-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="0e915-103">Update user</span></span>

<span data-ttu-id="0e915-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e915-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e915-105">更新 [user](../resources/user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e915-105">Update the properties of a [user](../resources/user.md) object.</span></span> <span data-ttu-id="0e915-106">并非所有属性都可以由具有默认权限（没有管理员角色）的"成员"或"来宾"用户进行更新。</span><span class="sxs-lookup"><span data-stu-id="0e915-106">Not all properties can be updated by Member or Guest users with their default permissions without Administrator roles.</span></span> <span data-ttu-id="0e915-107">[比较成员和来宾默认权限](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) 以查看他们可以管理的属性。</span><span class="sxs-lookup"><span data-stu-id="0e915-107">[Compare member and guest default permissions](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) to see properties they can manage.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e915-108">权限</span><span class="sxs-lookup"><span data-stu-id="0e915-108">Permissions</span></span>
<span data-ttu-id="0e915-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e915-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e915-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e915-111">Permission type</span></span>      | <span data-ttu-id="0e915-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e915-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e915-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e915-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0e915-114">User.ReadWrite、User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e915-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e915-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e915-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e915-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e915-116">User.ReadWrite</span></span>    |
|<span data-ttu-id="0e915-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e915-117">Application</span></span> | <span data-ttu-id="0e915-118">User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e915-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="0e915-119">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="0e915-119">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="0e915-120">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="0e915-120">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="0e915-121">有关详细信息，请参阅 Azure AD (角色中的) 密码[管理员"。](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="0e915-121">For more details, see Helpdesk (Password) Administrator in [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference).</span></span>  <span data-ttu-id="0e915-122">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="0e915-122">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>
> - <span data-ttu-id="0e915-123">必须使用个人 Microsoft 帐户的 User.ReadWrite 委派权限将你的个人 Microsoft 帐户绑定到 AAD 租户才能更新你的配置文件。</span><span class="sxs-lookup"><span data-stu-id="0e915-123">Your personal Microsoft account must be tied to an AAD tenant to update your profile with the User.ReadWrite delegated permission on a personal Microsoft account.</span></span>
> - <span data-ttu-id="0e915-124">更新 **identities** 属性需要 User.ManageIdentities.All 权限。</span><span class="sxs-lookup"><span data-stu-id="0e915-124">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="0e915-125">此外，不允许将 [B2C 本地帐户](../resources/objectidentity.md)添加到现有 **user** 对象，除非 **user** 对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="0e915-125">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="0e915-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e915-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="0e915-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e915-127">Request headers</span></span>
| <span data-ttu-id="0e915-128">标头</span><span class="sxs-lookup"><span data-stu-id="0e915-128">Header</span></span>       | <span data-ttu-id="0e915-129">值</span><span class="sxs-lookup"><span data-stu-id="0e915-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0e915-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e915-130">Authorization</span></span>  | <span data-ttu-id="0e915-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e915-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0e915-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e915-133">Content-Type</span></span>  | <span data-ttu-id="0e915-134">application/json</span><span class="sxs-lookup"><span data-stu-id="0e915-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e915-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e915-135">Request body</span></span>
<span data-ttu-id="0e915-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0e915-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e915-139">属性</span><span class="sxs-lookup"><span data-stu-id="0e915-139">Property</span></span>     | <span data-ttu-id="0e915-140">类型</span><span class="sxs-lookup"><span data-stu-id="0e915-140">Type</span></span>   |<span data-ttu-id="0e915-141">说明</span><span class="sxs-lookup"><span data-stu-id="0e915-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e915-142">aboutMe</span><span class="sxs-lookup"><span data-stu-id="0e915-142">aboutMe</span></span>|<span data-ttu-id="0e915-143">String</span><span class="sxs-lookup"><span data-stu-id="0e915-143">String</span></span>|<span data-ttu-id="0e915-144">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="0e915-144">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="0e915-145">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="0e915-145">accountEnabled</span></span>|<span data-ttu-id="0e915-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e915-146">Boolean</span></span>| <span data-ttu-id="0e915-147">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="0e915-147">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="0e915-148">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="0e915-148">This property is required when a user is created.</span></span>    |
| <span data-ttu-id="0e915-149">ageGroup</span><span class="sxs-lookup"><span data-stu-id="0e915-149">ageGroup</span></span> | [<span data-ttu-id="0e915-150">ageGroup</span><span class="sxs-lookup"><span data-stu-id="0e915-150">ageGroup</span></span>](../resources/user.md#agegroup-values) | <span data-ttu-id="0e915-151">设置用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="0e915-151">Sets the age group of the user.</span></span> <span data-ttu-id="0e915-152">允许的值：`null`、`minor`、`notAdult` 和 `adult`。</span><span class="sxs-lookup"><span data-stu-id="0e915-152">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="0e915-153">请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e915-153">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="0e915-154">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="0e915-154">assignedLicenses</span></span>|<span data-ttu-id="0e915-155">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e915-155">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="0e915-p109">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0e915-p109">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="0e915-158">birthday</span><span class="sxs-lookup"><span data-stu-id="0e915-158">birthday</span></span>|<span data-ttu-id="0e915-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e915-159">DateTimeOffset</span></span>|<span data-ttu-id="0e915-160">用户的生日。</span><span class="sxs-lookup"><span data-stu-id="0e915-160">The birthday of the user.</span></span> <span data-ttu-id="0e915-161">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0e915-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e915-162">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="0e915-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="0e915-163">businessPhones</span><span class="sxs-lookup"><span data-stu-id="0e915-163">businessPhones</span></span>| <span data-ttu-id="0e915-164">String collection</span><span class="sxs-lookup"><span data-stu-id="0e915-164">String collection</span></span> | <span data-ttu-id="0e915-p111">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="0e915-p111">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="0e915-167">城市</span><span class="sxs-lookup"><span data-stu-id="0e915-167">city</span></span>|<span data-ttu-id="0e915-168">String</span><span class="sxs-lookup"><span data-stu-id="0e915-168">String</span></span>|<span data-ttu-id="0e915-169">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="0e915-169">The city in which the user is located.</span></span>|
| <span data-ttu-id="0e915-170">companyName</span><span class="sxs-lookup"><span data-stu-id="0e915-170">companyName</span></span> | <span data-ttu-id="0e915-171">String</span><span class="sxs-lookup"><span data-stu-id="0e915-171">String</span></span> | <span data-ttu-id="0e915-172">与用户关联的公司名称。</span><span class="sxs-lookup"><span data-stu-id="0e915-172">The company name which the user is associated.</span></span> <span data-ttu-id="0e915-173">此属性可用于描述外部用户所属的公司。</span><span class="sxs-lookup"><span data-stu-id="0e915-173">This property can be useful for describing the company that an external user comes from.</span></span> <span data-ttu-id="0e915-174">公司名称的最大长度为 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="0e915-174">The maximum length of the company name is 64 characters.</span></span> |
| <span data-ttu-id="0e915-175">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="0e915-175">consentProvidedForMinor</span></span> | [<span data-ttu-id="0e915-176">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="0e915-176">consentProvidedForMinor</span></span>](../resources/user.md#consentprovidedforminor-values) | <span data-ttu-id="0e915-177">设置是否已获得未成年人的同意。</span><span class="sxs-lookup"><span data-stu-id="0e915-177">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="0e915-178">允许的值：`null`、`granted`、`denied` 和 `notRequired`。</span><span class="sxs-lookup"><span data-stu-id="0e915-178">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="0e915-179">请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e915-179">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="0e915-180">country</span><span class="sxs-lookup"><span data-stu-id="0e915-180">country</span></span>|<span data-ttu-id="0e915-181">String</span><span class="sxs-lookup"><span data-stu-id="0e915-181">String</span></span>|<span data-ttu-id="0e915-182">用户所在的国家/地区；例如，“美国”或“英国”。</span><span class="sxs-lookup"><span data-stu-id="0e915-182">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="0e915-183">department</span><span class="sxs-lookup"><span data-stu-id="0e915-183">department</span></span>|<span data-ttu-id="0e915-184">String</span><span class="sxs-lookup"><span data-stu-id="0e915-184">String</span></span>|<span data-ttu-id="0e915-185">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="0e915-185">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="0e915-186">displayName</span><span class="sxs-lookup"><span data-stu-id="0e915-186">displayName</span></span>|<span data-ttu-id="0e915-187">String</span><span class="sxs-lookup"><span data-stu-id="0e915-187">String</span></span>|<span data-ttu-id="0e915-188">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="0e915-188">The name displayed in the address book for the user.</span></span> <span data-ttu-id="0e915-189">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="0e915-189">This is usually the combination of the user's first name, middle initial and last name.</span></span> <span data-ttu-id="0e915-190">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="0e915-190">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="0e915-191">支持 `$filter` 和 `$orderby`。</span><span class="sxs-lookup"><span data-stu-id="0e915-191">Supports `$filter` and `$orderby`.</span></span>|
|<span data-ttu-id="0e915-192">employeeId</span><span class="sxs-lookup"><span data-stu-id="0e915-192">employeeId</span></span>|<span data-ttu-id="0e915-193">String</span><span class="sxs-lookup"><span data-stu-id="0e915-193">String</span></span>|<span data-ttu-id="0e915-194">由组织分配给该用户的员工标识符。</span><span class="sxs-lookup"><span data-stu-id="0e915-194">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="0e915-195">givenName</span><span class="sxs-lookup"><span data-stu-id="0e915-195">givenName</span></span>|<span data-ttu-id="0e915-196">String</span><span class="sxs-lookup"><span data-stu-id="0e915-196">String</span></span>|<span data-ttu-id="0e915-197">用户的名。</span><span class="sxs-lookup"><span data-stu-id="0e915-197">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="0e915-198">hireDate</span><span class="sxs-lookup"><span data-stu-id="0e915-198">hireDate</span></span>|<span data-ttu-id="0e915-199">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e915-199">DateTimeOffset</span></span>|<span data-ttu-id="0e915-200">用户的雇佣日期。</span><span class="sxs-lookup"><span data-stu-id="0e915-200">The hire date of the user.</span></span> <span data-ttu-id="0e915-201">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0e915-201">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0e915-202">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="0e915-202">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="0e915-203">identities</span><span class="sxs-lookup"><span data-stu-id="0e915-203">identities</span></span>|<span data-ttu-id="0e915-204">[objectIdentity](../resources/objectidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e915-204">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="0e915-205">表示可用于登录此用户帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="0e915-205">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="0e915-206">标识可由 Microsoft、组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供，并绑定到用户帐户。</span><span class="sxs-lookup"><span data-stu-id="0e915-206">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="0e915-207">对标识 **的任何** 更新都将替换整个集合，并且必须在集合中提供 userPrincipalName **signInType** 标识。</span><span class="sxs-lookup"><span data-stu-id="0e915-207">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="0e915-208">interests</span><span class="sxs-lookup"><span data-stu-id="0e915-208">interests</span></span>|<span data-ttu-id="0e915-209">String collection</span><span class="sxs-lookup"><span data-stu-id="0e915-209">String collection</span></span>|<span data-ttu-id="0e915-210">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="0e915-210">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="0e915-211">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0e915-211">jobTitle</span></span>|<span data-ttu-id="0e915-212">String</span><span class="sxs-lookup"><span data-stu-id="0e915-212">String</span></span>|<span data-ttu-id="0e915-213">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="0e915-213">The user’s job title.</span></span>|
|<span data-ttu-id="0e915-214">mail</span><span class="sxs-lookup"><span data-stu-id="0e915-214">mail</span></span>|<span data-ttu-id="0e915-215">String</span><span class="sxs-lookup"><span data-stu-id="0e915-215">String</span></span>|<span data-ttu-id="0e915-216">用户的 SMTP 地址，例如 `jeff@contoso.onmicrosoft.com` ， 。</span><span class="sxs-lookup"><span data-stu-id="0e915-216">The SMTP address for the user, for example, `jeff@contoso.onmicrosoft.com`.</span></span> <span data-ttu-id="0e915-217">对此属性的更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="0e915-217">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="0e915-218">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="0e915-218">Returned by default.</span></span> <span data-ttu-id="0e915-219">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="0e915-219">Supports `$filter`.</span></span>|
|<span data-ttu-id="0e915-220">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0e915-220">mailNickname</span></span>|<span data-ttu-id="0e915-221">String</span><span class="sxs-lookup"><span data-stu-id="0e915-221">String</span></span>|<span data-ttu-id="0e915-222">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="0e915-222">The mail alias for the user.</span></span> <span data-ttu-id="0e915-223">创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="0e915-223">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="0e915-224">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0e915-224">mobilePhone</span></span>|<span data-ttu-id="0e915-225">String</span><span class="sxs-lookup"><span data-stu-id="0e915-225">String</span></span>|<span data-ttu-id="0e915-226">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="0e915-226">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="0e915-227">mySite</span><span class="sxs-lookup"><span data-stu-id="0e915-227">mySite</span></span>|<span data-ttu-id="0e915-228">String</span><span class="sxs-lookup"><span data-stu-id="0e915-228">String</span></span>|<span data-ttu-id="0e915-229">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="0e915-229">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="0e915-230">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0e915-230">officeLocation</span></span>|<span data-ttu-id="0e915-231">String</span><span class="sxs-lookup"><span data-stu-id="0e915-231">String</span></span>|<span data-ttu-id="0e915-232">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="0e915-232">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="0e915-233">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="0e915-233">onPremisesImmutableId</span></span>|<span data-ttu-id="0e915-234">String</span><span class="sxs-lookup"><span data-stu-id="0e915-234">String</span></span>|<span data-ttu-id="0e915-235">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="0e915-235">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="0e915-236">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="0e915-236">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="0e915-237">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="0e915-237">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="0e915-238">otherMails</span><span class="sxs-lookup"><span data-stu-id="0e915-238">otherMails</span></span>|<span data-ttu-id="0e915-239">String</span><span class="sxs-lookup"><span data-stu-id="0e915-239">String</span></span> |<span data-ttu-id="0e915-240">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="0e915-240">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="0e915-241">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="0e915-241">passwordPolicies</span></span>|<span data-ttu-id="0e915-242">String</span><span class="sxs-lookup"><span data-stu-id="0e915-242">String</span></span>|<span data-ttu-id="0e915-243">指定用户的密码策略。</span><span class="sxs-lookup"><span data-stu-id="0e915-243">Specifies password policies for the user.</span></span> <span data-ttu-id="0e915-244">此值是一个枚举，其中一个可能的值是 ，这允许指定比 `DisableStrongPassword` 默认策略弱的密码。</span><span class="sxs-lookup"><span data-stu-id="0e915-244">This value is an enumeration with one possible value being `DisableStrongPassword`, which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="0e915-245">`DisablePasswordExpiration` 也可以指定 。</span><span class="sxs-lookup"><span data-stu-id="0e915-245">`DisablePasswordExpiration` can also be specified.</span></span> <span data-ttu-id="0e915-246">可以同时指定这两者;例如 `DisablePasswordExpiration, DisableStrongPassword` ：。</span><span class="sxs-lookup"><span data-stu-id="0e915-246">The two may be specified together; for example: `DisablePasswordExpiration, DisableStrongPassword`.</span></span>|
|<span data-ttu-id="0e915-247">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="0e915-247">passwordProfile</span></span>|[<span data-ttu-id="0e915-248">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="0e915-248">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="0e915-p122">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="0e915-p122">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="0e915-254">pastProjects</span><span class="sxs-lookup"><span data-stu-id="0e915-254">pastProjects</span></span>|<span data-ttu-id="0e915-255">String collection</span><span class="sxs-lookup"><span data-stu-id="0e915-255">String collection</span></span>|<span data-ttu-id="0e915-256">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="0e915-256">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="0e915-257">postalCode</span><span class="sxs-lookup"><span data-stu-id="0e915-257">postalCode</span></span>|<span data-ttu-id="0e915-258">String</span><span class="sxs-lookup"><span data-stu-id="0e915-258">String</span></span>|<span data-ttu-id="0e915-p123">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="0e915-p123">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="0e915-262">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="0e915-262">preferredLanguage</span></span>|<span data-ttu-id="0e915-263">String</span><span class="sxs-lookup"><span data-stu-id="0e915-263">String</span></span>|<span data-ttu-id="0e915-264">用户的首选语言。</span><span class="sxs-lookup"><span data-stu-id="0e915-264">The preferred language for the user.</span></span> <span data-ttu-id="0e915-265">应遵循 ISO 639-1 代码;例如 `en-US` 。</span><span class="sxs-lookup"><span data-stu-id="0e915-265">Should follow ISO 639-1 Code; for example `en-US`.</span></span>|
|<span data-ttu-id="0e915-266">responsibilities</span><span class="sxs-lookup"><span data-stu-id="0e915-266">responsibilities</span></span>|<span data-ttu-id="0e915-267">String collection</span><span class="sxs-lookup"><span data-stu-id="0e915-267">String collection</span></span>|<span data-ttu-id="0e915-268">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="0e915-268">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="0e915-269">schools</span><span class="sxs-lookup"><span data-stu-id="0e915-269">schools</span></span>|<span data-ttu-id="0e915-270">String collection</span><span class="sxs-lookup"><span data-stu-id="0e915-270">String collection</span></span>|<span data-ttu-id="0e915-271">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="0e915-271">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="0e915-272">skills</span><span class="sxs-lookup"><span data-stu-id="0e915-272">skills</span></span>|<span data-ttu-id="0e915-273">String collection</span><span class="sxs-lookup"><span data-stu-id="0e915-273">String collection</span></span>|<span data-ttu-id="0e915-274">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="0e915-274">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="0e915-275">state</span><span class="sxs-lookup"><span data-stu-id="0e915-275">state</span></span>|<span data-ttu-id="0e915-276">String</span><span class="sxs-lookup"><span data-stu-id="0e915-276">String</span></span>|<span data-ttu-id="0e915-277">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="0e915-277">The state or province in the user's address.</span></span>|
|<span data-ttu-id="0e915-278">streetAddress</span><span class="sxs-lookup"><span data-stu-id="0e915-278">streetAddress</span></span>|<span data-ttu-id="0e915-279">String</span><span class="sxs-lookup"><span data-stu-id="0e915-279">String</span></span>|<span data-ttu-id="0e915-280">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="0e915-280">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="0e915-281">surname</span><span class="sxs-lookup"><span data-stu-id="0e915-281">surname</span></span>|<span data-ttu-id="0e915-282">String</span><span class="sxs-lookup"><span data-stu-id="0e915-282">String</span></span>|<span data-ttu-id="0e915-283">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="0e915-283">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="0e915-284">usageLocation</span><span class="sxs-lookup"><span data-stu-id="0e915-284">usageLocation</span></span>|<span data-ttu-id="0e915-285">String</span><span class="sxs-lookup"><span data-stu-id="0e915-285">String</span></span>|<span data-ttu-id="0e915-286">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="0e915-286">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="0e915-287">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="0e915-287">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="0e915-288">示例包括 `US` ：、 `JP` 和 `GB` 。</span><span class="sxs-lookup"><span data-stu-id="0e915-288">Examples include: `US`, `JP`, and `GB`.</span></span> <span data-ttu-id="0e915-289">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0e915-289">Not nullable.</span></span>|
|<span data-ttu-id="0e915-290">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e915-290">userPrincipalName</span></span>|<span data-ttu-id="0e915-291">String</span><span class="sxs-lookup"><span data-stu-id="0e915-291">String</span></span>|<span data-ttu-id="0e915-p126">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="0e915-p126">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="0e915-299">userType</span><span class="sxs-lookup"><span data-stu-id="0e915-299">userType</span></span>|<span data-ttu-id="0e915-300">String</span><span class="sxs-lookup"><span data-stu-id="0e915-300">String</span></span>|<span data-ttu-id="0e915-301">可用于对目录中的用户类型进行分类的字符串值，例如 `Member` 和 `Guest` 。</span><span class="sxs-lookup"><span data-stu-id="0e915-301">A string value that can be used to classify user types in your directory, such as `Member` and `Guest`.</span></span>          |

<span data-ttu-id="0e915-302">由于 **用户** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作在现有用户实例的扩展的自定义属性中添加、更新或删除你自己的特定于 `PATCH` **应用** 的数据。</span><span class="sxs-lookup"><span data-stu-id="0e915-302">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

> [!NOTE] 
> <span data-ttu-id="0e915-303">以下属性无法使用仅限应用程序上下文进行更新：**aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**。</span><span class="sxs-lookup"><span data-stu-id="0e915-303">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="0e915-304">响应</span><span class="sxs-lookup"><span data-stu-id="0e915-304">Response</span></span>

<span data-ttu-id="0e915-305">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e915-305">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e915-306">示例</span><span class="sxs-lookup"><span data-stu-id="0e915-306">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="0e915-307">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="0e915-307">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="0e915-308">请求</span><span class="sxs-lookup"><span data-stu-id="0e915-308">Request</span></span>

<span data-ttu-id="0e915-309">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="0e915-309">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e915-310">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e915-310">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="0e915-311">C#</span><span class="sxs-lookup"><span data-stu-id="0e915-311">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e915-312">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e915-312">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e915-313">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e915-313">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e915-314">Java</span><span class="sxs-lookup"><span data-stu-id="0e915-314">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0e915-315">响应</span><span class="sxs-lookup"><span data-stu-id="0e915-315">Response</span></span>

<span data-ttu-id="0e915-316">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="0e915-316">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="0e915-317">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="0e915-317">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="0e915-318">请求</span><span class="sxs-lookup"><span data-stu-id="0e915-318">Request</span></span>

<span data-ttu-id="0e915-319">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="0e915-319">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e915-320">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e915-320">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="0e915-321">C#</span><span class="sxs-lookup"><span data-stu-id="0e915-321">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e915-322">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e915-322">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e915-323">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e915-323">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e915-324">Java</span><span class="sxs-lookup"><span data-stu-id="0e915-324">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e915-325">响应</span><span class="sxs-lookup"><span data-stu-id="0e915-325">Response</span></span>

<span data-ttu-id="0e915-326">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="0e915-326">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="0e915-327">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0e915-327">See also</span></span>

- [<span data-ttu-id="0e915-328">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0e915-328">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0e915-329">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="0e915-329">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0e915-330">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="0e915-330">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
