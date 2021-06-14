---
title: 更新用户
description: 更新 user 对象的属性。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 456361bf711419bec46967d9478c004a1ac624ad
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911352"
---
# <a name="update-user"></a><span data-ttu-id="38c9a-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="38c9a-103">Update user</span></span>

<span data-ttu-id="38c9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38c9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38c9a-105">更新 [user](../resources/user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38c9a-105">Update the properties of a [user](../resources/user.md) object.</span></span> <span data-ttu-id="38c9a-106">并非所有属性都可以在没有管理员角色的情况下由具有其默认权限的成员或来宾用户更新。</span><span class="sxs-lookup"><span data-stu-id="38c9a-106">Not all properties can be updated by Member or Guest users with their default permissions without Administrator roles.</span></span> <span data-ttu-id="38c9a-107">[比较成员和来宾默认](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) 权限，查看其可管理的属性。</span><span class="sxs-lookup"><span data-stu-id="38c9a-107">[Compare member and guest default permissions](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) to see properties they can manage.</span></span>

## <a name="permissions"></a><span data-ttu-id="38c9a-108">权限</span><span class="sxs-lookup"><span data-stu-id="38c9a-108">Permissions</span></span>
<span data-ttu-id="38c9a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38c9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38c9a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38c9a-111">Permission type</span></span>      | <span data-ttu-id="38c9a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38c9a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38c9a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38c9a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="38c9a-114">User.ReadWrite、User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38c9a-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38c9a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38c9a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38c9a-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38c9a-116">User.ReadWrite</span></span>    |
|<span data-ttu-id="38c9a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38c9a-117">Application</span></span> | <span data-ttu-id="38c9a-118">User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38c9a-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="38c9a-119">更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="38c9a-119">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="38c9a-120">如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。</span><span class="sxs-lookup"><span data-stu-id="38c9a-120">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="38c9a-121">有关详细信息，请参阅 [Azure AD 内置角色帮助人员（密码）](/azure/active-directory/roles/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38c9a-121">For more details, see Helpdesk (Password) Administrator in [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference).</span></span>  <span data-ttu-id="38c9a-122">这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。</span><span class="sxs-lookup"><span data-stu-id="38c9a-122">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>
> - <span data-ttu-id="38c9a-123">个人 Microsoft 帐户必须绑定到 AAD 租户，才能使用 User.ReadWrite 对个人 Microsoft 帐户的委派权限更新配置文件。</span><span class="sxs-lookup"><span data-stu-id="38c9a-123">Your personal Microsoft account must be tied to an AAD tenant to update your profile with the User.ReadWrite delegated permission on a personal Microsoft account.</span></span>
> - <span data-ttu-id="38c9a-124">更新 **identities** 属性需要 User.ManageIdentities.All 权限。</span><span class="sxs-lookup"><span data-stu-id="38c9a-124">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="38c9a-125">此外，不允许将 [B2C 本地帐户](../resources/objectidentity.md)添加到现有 **user** 对象，除非 **user** 对象已包含本地帐户标识。</span><span class="sxs-lookup"><span data-stu-id="38c9a-125">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="38c9a-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38c9a-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="38c9a-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="38c9a-127">Request headers</span></span>
| <span data-ttu-id="38c9a-128">标头</span><span class="sxs-lookup"><span data-stu-id="38c9a-128">Header</span></span>       | <span data-ttu-id="38c9a-129">值</span><span class="sxs-lookup"><span data-stu-id="38c9a-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="38c9a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="38c9a-130">Authorization</span></span>  | <span data-ttu-id="38c9a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38c9a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="38c9a-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38c9a-133">Content-Type</span></span>  | <span data-ttu-id="38c9a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="38c9a-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38c9a-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="38c9a-135">Request body</span></span>
<span data-ttu-id="38c9a-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="38c9a-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="38c9a-139">属性</span><span class="sxs-lookup"><span data-stu-id="38c9a-139">Property</span></span>     | <span data-ttu-id="38c9a-140">类型</span><span class="sxs-lookup"><span data-stu-id="38c9a-140">Type</span></span>   |<span data-ttu-id="38c9a-141">说明</span><span class="sxs-lookup"><span data-stu-id="38c9a-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38c9a-142">aboutMe</span><span class="sxs-lookup"><span data-stu-id="38c9a-142">aboutMe</span></span>|<span data-ttu-id="38c9a-143">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-143">String</span></span>|<span data-ttu-id="38c9a-144">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="38c9a-144">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="38c9a-145">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="38c9a-145">accountEnabled</span></span>|<span data-ttu-id="38c9a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="38c9a-146">Boolean</span></span>| <span data-ttu-id="38c9a-147">启用帐户时为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-147">`true` if the account is enabled; otherwise, `false`.</span></span> <span data-ttu-id="38c9a-148">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="38c9a-148">This property is required when a user is created.</span></span>    |
| <span data-ttu-id="38c9a-149">ageGroup</span><span class="sxs-lookup"><span data-stu-id="38c9a-149">ageGroup</span></span> | [<span data-ttu-id="38c9a-150">ageGroup</span><span class="sxs-lookup"><span data-stu-id="38c9a-150">ageGroup</span></span>](../resources/user.md#agegroup-values) | <span data-ttu-id="38c9a-151">设置用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="38c9a-151">Sets the age group of the user.</span></span> <span data-ttu-id="38c9a-152">允许的值：`null`、`minor`、`notAdult` 和 `adult`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-152">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="38c9a-153">请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="38c9a-153">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="38c9a-154">birthday</span><span class="sxs-lookup"><span data-stu-id="38c9a-154">birthday</span></span>|<span data-ttu-id="38c9a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38c9a-155">DateTimeOffset</span></span>|<span data-ttu-id="38c9a-156">用户的生日。</span><span class="sxs-lookup"><span data-stu-id="38c9a-156">The birthday of the user.</span></span> <span data-ttu-id="38c9a-157">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="38c9a-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38c9a-158">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="38c9a-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="38c9a-159">businessPhones</span><span class="sxs-lookup"><span data-stu-id="38c9a-159">businessPhones</span></span>| <span data-ttu-id="38c9a-160">String collection</span><span class="sxs-lookup"><span data-stu-id="38c9a-160">String collection</span></span> | <span data-ttu-id="38c9a-p110">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-p110">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="38c9a-163">城市</span><span class="sxs-lookup"><span data-stu-id="38c9a-163">city</span></span>|<span data-ttu-id="38c9a-164">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-164">String</span></span>|<span data-ttu-id="38c9a-165">用户所在的城市。</span><span class="sxs-lookup"><span data-stu-id="38c9a-165">The city in which the user is located.</span></span>|
| <span data-ttu-id="38c9a-166">companyName</span><span class="sxs-lookup"><span data-stu-id="38c9a-166">companyName</span></span> | <span data-ttu-id="38c9a-167">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-167">String</span></span> | <span data-ttu-id="38c9a-168">与用户关联的公司名称。</span><span class="sxs-lookup"><span data-stu-id="38c9a-168">The company name which the user is associated.</span></span> <span data-ttu-id="38c9a-169">此属性可用于描述外部用户所属的公司。</span><span class="sxs-lookup"><span data-stu-id="38c9a-169">This property can be useful for describing the company that an external user comes from.</span></span> <span data-ttu-id="38c9a-170">公司名称的最大长度为 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="38c9a-170">The maximum length of the company name is 64 characters.</span></span> |
| <span data-ttu-id="38c9a-171">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="38c9a-171">consentProvidedForMinor</span></span> | [<span data-ttu-id="38c9a-172">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="38c9a-172">consentProvidedForMinor</span></span>](../resources/user.md#consentprovidedforminor-values) | <span data-ttu-id="38c9a-173">设置是否已获得未成年人的同意。</span><span class="sxs-lookup"><span data-stu-id="38c9a-173">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="38c9a-174">允许的值：`null`、`granted`、`denied` 和 `notRequired`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-174">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="38c9a-175">请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="38c9a-175">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="38c9a-176">country</span><span class="sxs-lookup"><span data-stu-id="38c9a-176">country</span></span>|<span data-ttu-id="38c9a-177">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-177">String</span></span>|<span data-ttu-id="38c9a-178">用户所在的国家/地区;例如， `US` 或 `UK`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-178">The country/region in which the user is located; for example, `US` or `UK`.</span></span>|
|<span data-ttu-id="38c9a-179">department</span><span class="sxs-lookup"><span data-stu-id="38c9a-179">department</span></span>|<span data-ttu-id="38c9a-180">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-180">String</span></span>|<span data-ttu-id="38c9a-181">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="38c9a-181">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="38c9a-182">displayName</span><span class="sxs-lookup"><span data-stu-id="38c9a-182">displayName</span></span>|<span data-ttu-id="38c9a-183">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-183">String</span></span>|<span data-ttu-id="38c9a-184">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="38c9a-184">The name displayed in the address book for the user.</span></span> <span data-ttu-id="38c9a-185">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="38c9a-185">This is usually the combination of the user's first name, middle initial and last name.</span></span> <span data-ttu-id="38c9a-186">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="38c9a-186">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="38c9a-187">支持 `$filter` 和 `$orderby`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-187">Supports `$filter` and `$orderby`.</span></span>|
| <span data-ttu-id="38c9a-188">employeeId</span><span class="sxs-lookup"><span data-stu-id="38c9a-188">employeeId</span></span> | <span data-ttu-id="38c9a-189">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-189">String</span></span> | <span data-ttu-id="38c9a-190">由组织分配给该用户的员工标识符。</span><span class="sxs-lookup"><span data-stu-id="38c9a-190">The employee identifier assigned to the user by the organization.</span></span> |
| <span data-ttu-id="38c9a-191">employeeType</span><span class="sxs-lookup"><span data-stu-id="38c9a-191">employeeType</span></span> | <span data-ttu-id="38c9a-192">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-192">String</span></span> | <span data-ttu-id="38c9a-193">捕获企业员工类型。</span><span class="sxs-lookup"><span data-stu-id="38c9a-193">Captures enterprise worker type.</span></span> <span data-ttu-id="38c9a-194">例如，`Employee`、`Contractor`、`Consultant` 或 `Vendor`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-194">For example, `Employee`, `Contractor`, `Consultant`, or `Vendor`.</span></span> <span data-ttu-id="38c9a-195">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="38c9a-195">Returned only on `$select`.</span></span>|
|<span data-ttu-id="38c9a-196">givenName</span><span class="sxs-lookup"><span data-stu-id="38c9a-196">givenName</span></span>|<span data-ttu-id="38c9a-197">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-197">String</span></span>|<span data-ttu-id="38c9a-198">用户的名。</span><span class="sxs-lookup"><span data-stu-id="38c9a-198">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="38c9a-199">hireDate</span><span class="sxs-lookup"><span data-stu-id="38c9a-199">hireDate</span></span>|<span data-ttu-id="38c9a-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38c9a-200">DateTimeOffset</span></span>|<span data-ttu-id="38c9a-201">用户的雇佣日期。</span><span class="sxs-lookup"><span data-stu-id="38c9a-201">The hire date of the user.</span></span> <span data-ttu-id="38c9a-202">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="38c9a-202">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38c9a-203">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="38c9a-203">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="38c9a-204">interests</span><span class="sxs-lookup"><span data-stu-id="38c9a-204">interests</span></span>|<span data-ttu-id="38c9a-205">String collection</span><span class="sxs-lookup"><span data-stu-id="38c9a-205">String collection</span></span>|<span data-ttu-id="38c9a-206">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="38c9a-206">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="38c9a-207">jobTitle</span><span class="sxs-lookup"><span data-stu-id="38c9a-207">jobTitle</span></span>|<span data-ttu-id="38c9a-208">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-208">String</span></span>|<span data-ttu-id="38c9a-209">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="38c9a-209">The user’s job title.</span></span>|
|<span data-ttu-id="38c9a-210">mail</span><span class="sxs-lookup"><span data-stu-id="38c9a-210">mail</span></span>|<span data-ttu-id="38c9a-211">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-211">String</span></span>|<span data-ttu-id="38c9a-212">用户的 SMTP 地址，例如， `jeff@contoso.onmicrosoft.com`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-212">The SMTP address for the user, for example, `jeff@contoso.onmicrosoft.com`.</span></span> <span data-ttu-id="38c9a-213">对此属性的更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="38c9a-213">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span>|
|<span data-ttu-id="38c9a-214">mailNickname</span><span class="sxs-lookup"><span data-stu-id="38c9a-214">mailNickname</span></span>|<span data-ttu-id="38c9a-215">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-215">String</span></span>|<span data-ttu-id="38c9a-p117">用户的邮件别名。创建用户时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="38c9a-p117">The mail alias for the user. This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="38c9a-218">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="38c9a-218">mobilePhone</span></span>|<span data-ttu-id="38c9a-219">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-219">String</span></span>|<span data-ttu-id="38c9a-220">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-220">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="38c9a-221">mySite</span><span class="sxs-lookup"><span data-stu-id="38c9a-221">mySite</span></span>|<span data-ttu-id="38c9a-222">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-222">String</span></span>|<span data-ttu-id="38c9a-223">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="38c9a-223">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="38c9a-224">officeLocation</span><span class="sxs-lookup"><span data-stu-id="38c9a-224">officeLocation</span></span>|<span data-ttu-id="38c9a-225">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-225">String</span></span>|<span data-ttu-id="38c9a-226">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="38c9a-226">The office location in the user's place of business.</span></span>|
| <span data-ttu-id="38c9a-227">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="38c9a-227">onPremisesExtensionAttributes</span></span> | [<span data-ttu-id="38c9a-228">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="38c9a-228">onPremisesExtensionAttributes</span></span>](../resources/onpremisesextensionattributes.md) | <span data-ttu-id="38c9a-229">包含用户的 extensionAttributes 1-15。</span><span class="sxs-lookup"><span data-stu-id="38c9a-229">Contains extensionAttributes 1-15 for the user.</span></span> <span data-ttu-id="38c9a-230">请注意，单个扩展属性既不可选择，也不可筛选。</span><span class="sxs-lookup"><span data-stu-id="38c9a-230">Note that the individual extension attributes are neither selectable nor filterable.</span></span> <span data-ttu-id="38c9a-231">对于 `onPremisesSyncEnabled` 用户，这组属性集的授权来源是本地，并且为只读。</span><span class="sxs-lookup"><span data-stu-id="38c9a-231">For an `onPremisesSyncEnabled` user, the source of authority for this set of properties is the on-premises and is read-only and is read-only.</span></span> <span data-ttu-id="38c9a-232">这些扩展属性也称 Exchange 自定义属性 1-15。</span><span class="sxs-lookup"><span data-stu-id="38c9a-232">These extension attributes are also known as Exchange custom attributes 1-15.</span></span>|
|<span data-ttu-id="38c9a-233">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="38c9a-233">onPremisesImmutableId</span></span>|<span data-ttu-id="38c9a-234">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-234">String</span></span>|<span data-ttu-id="38c9a-235">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。</span><span class="sxs-lookup"><span data-stu-id="38c9a-235">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="38c9a-236">如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。</span><span class="sxs-lookup"><span data-stu-id="38c9a-236">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="38c9a-237">**重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。</span><span class="sxs-lookup"><span data-stu-id="38c9a-237">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="38c9a-238">otherMails</span><span class="sxs-lookup"><span data-stu-id="38c9a-238">otherMails</span></span>|<span data-ttu-id="38c9a-239">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-239">String</span></span> |<span data-ttu-id="38c9a-240">用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-240">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="38c9a-241">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="38c9a-241">passwordPolicies</span></span>|<span data-ttu-id="38c9a-242">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-242">String</span></span>|<span data-ttu-id="38c9a-243">指定用户的密码策略。</span><span class="sxs-lookup"><span data-stu-id="38c9a-243">Specifies password policies for the user.</span></span> <span data-ttu-id="38c9a-244">此值表示枚举，其中一个可能 `DisableStrongPassword`为枚举值，允许指定超过默认策略的密码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-244">This value is an enumeration with one possible value being `DisableStrongPassword`, which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="38c9a-245">`DisablePasswordExpiration` 也可以指定 。</span><span class="sxs-lookup"><span data-stu-id="38c9a-245">`DisablePasswordExpiration` can also be specified.</span></span> <span data-ttu-id="38c9a-246">可同时指定两者;例如： `DisablePasswordExpiration, DisableStrongPassword`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-246">The two may be specified together; for example: `DisablePasswordExpiration, DisableStrongPassword`.</span></span>|
|<span data-ttu-id="38c9a-247">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="38c9a-247">passwordProfile</span></span>|[<span data-ttu-id="38c9a-248">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="38c9a-248">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="38c9a-249">指定用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="38c9a-249">Specifies the password profile for the user.</span></span> <span data-ttu-id="38c9a-250">配置文件包含用户的密码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-250">The profile contains the user’s password.</span></span> <span data-ttu-id="38c9a-251">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="38c9a-251">This property is required when a user is created.</span></span> <span data-ttu-id="38c9a-252">配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。</span><span class="sxs-lookup"><span data-stu-id="38c9a-252">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="38c9a-253">默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-253">By default, a strong password is required.</span></span> <span data-ttu-id="38c9a-254">这不能用于联合用户。</span><span class="sxs-lookup"><span data-stu-id="38c9a-254">This cannot be used for federated users.</span></span>|
|<span data-ttu-id="38c9a-255">pastProjects</span><span class="sxs-lookup"><span data-stu-id="38c9a-255">pastProjects</span></span>|<span data-ttu-id="38c9a-256">String collection</span><span class="sxs-lookup"><span data-stu-id="38c9a-256">String collection</span></span>|<span data-ttu-id="38c9a-257">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="38c9a-257">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="38c9a-258">postalCode</span><span class="sxs-lookup"><span data-stu-id="38c9a-258">postalCode</span></span>|<span data-ttu-id="38c9a-259">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-259">String</span></span>|<span data-ttu-id="38c9a-p122">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-p122">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="38c9a-263">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="38c9a-263">preferredLanguage</span></span>|<span data-ttu-id="38c9a-264">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-264">String</span></span>|<span data-ttu-id="38c9a-265">用户的首选语言。</span><span class="sxs-lookup"><span data-stu-id="38c9a-265">The preferred language for the user.</span></span> <span data-ttu-id="38c9a-266">应遵循 ISO 639-1 代码;例如， `en-US`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-266">Should follow ISO 639-1 Code; for example `en-US`.</span></span>|
|<span data-ttu-id="38c9a-267">responsibilities</span><span class="sxs-lookup"><span data-stu-id="38c9a-267">responsibilities</span></span>|<span data-ttu-id="38c9a-268">String collection</span><span class="sxs-lookup"><span data-stu-id="38c9a-268">String collection</span></span>|<span data-ttu-id="38c9a-269">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="38c9a-269">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="38c9a-270">schools</span><span class="sxs-lookup"><span data-stu-id="38c9a-270">schools</span></span>|<span data-ttu-id="38c9a-271">String collection</span><span class="sxs-lookup"><span data-stu-id="38c9a-271">String collection</span></span>|<span data-ttu-id="38c9a-272">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="38c9a-272">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="38c9a-273">skills</span><span class="sxs-lookup"><span data-stu-id="38c9a-273">skills</span></span>|<span data-ttu-id="38c9a-274">String collection</span><span class="sxs-lookup"><span data-stu-id="38c9a-274">String collection</span></span>|<span data-ttu-id="38c9a-275">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="38c9a-275">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="38c9a-276">state</span><span class="sxs-lookup"><span data-stu-id="38c9a-276">state</span></span>|<span data-ttu-id="38c9a-277">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-277">String</span></span>|<span data-ttu-id="38c9a-278">用户地址中的省/市/自治区或省。</span><span class="sxs-lookup"><span data-stu-id="38c9a-278">The state or province in the user's address.</span></span>|
|<span data-ttu-id="38c9a-279">streetAddress</span><span class="sxs-lookup"><span data-stu-id="38c9a-279">streetAddress</span></span>|<span data-ttu-id="38c9a-280">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-280">String</span></span>|<span data-ttu-id="38c9a-281">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="38c9a-281">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="38c9a-282">surname</span><span class="sxs-lookup"><span data-stu-id="38c9a-282">surname</span></span>|<span data-ttu-id="38c9a-283">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-283">String</span></span>|<span data-ttu-id="38c9a-284">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="38c9a-284">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="38c9a-285">usageLocation</span><span class="sxs-lookup"><span data-stu-id="38c9a-285">usageLocation</span></span>|<span data-ttu-id="38c9a-286">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-286">String</span></span>|<span data-ttu-id="38c9a-287">两个字母的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="38c9a-287">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="38c9a-288">为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="38c9a-288">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="38c9a-289">示例包括： `US`、 `JP`和 `GB`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-289">Examples include: `US`, `JP`, and `GB`.</span></span> <span data-ttu-id="38c9a-290">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="38c9a-290">Not nullable.</span></span>|
|<span data-ttu-id="38c9a-291">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38c9a-291">userPrincipalName</span></span>|<span data-ttu-id="38c9a-292">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-292">String</span></span>|<span data-ttu-id="38c9a-293">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="38c9a-293">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="38c9a-294">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="38c9a-294">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="38c9a-295">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="38c9a-295">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="38c9a-296">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="38c9a-296">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="38c9a-297">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="38c9a-297">This property is required when a user is created.</span></span> <span data-ttu-id="38c9a-298">可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。</span><span class="sxs-lookup"><span data-stu-id="38c9a-298">The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md).</span></span> <span data-ttu-id="38c9a-299">支持 `$filter` 和 `$orderby`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-299">Supports `$filter` and `$orderby`.</span></span>
|<span data-ttu-id="38c9a-300">userType</span><span class="sxs-lookup"><span data-stu-id="38c9a-300">userType</span></span>|<span data-ttu-id="38c9a-301">String</span><span class="sxs-lookup"><span data-stu-id="38c9a-301">String</span></span>|<span data-ttu-id="38c9a-302">可用于对目录中的用户类型进行分类的字符串值，例如`Member``Guest`。</span><span class="sxs-lookup"><span data-stu-id="38c9a-302">A string value that can be used to classify user types in your directory, such as `Member` and `Guest`.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="38c9a-303">以下属性无法使用仅限应用程序上下文进行更新：**aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**。</span><span class="sxs-lookup"><span data-stu-id="38c9a-303">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="38c9a-304">响应</span><span class="sxs-lookup"><span data-stu-id="38c9a-304">Response</span></span>

<span data-ttu-id="38c9a-305">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="38c9a-305">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="38c9a-306">示例</span><span class="sxs-lookup"><span data-stu-id="38c9a-306">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="38c9a-307">示例 1：更新已登录用户的属性</span><span class="sxs-lookup"><span data-stu-id="38c9a-307">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="38c9a-308">请求</span><span class="sxs-lookup"><span data-stu-id="38c9a-308">Request</span></span>

<span data-ttu-id="38c9a-309">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="38c9a-309">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38c9a-310">HTTP</span><span class="sxs-lookup"><span data-stu-id="38c9a-310">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="38c9a-311">C#</span><span class="sxs-lookup"><span data-stu-id="38c9a-311">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38c9a-312">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38c9a-312">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38c9a-313">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38c9a-313">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38c9a-314">Java</span><span class="sxs-lookup"><span data-stu-id="38c9a-314">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="38c9a-315">响应</span><span class="sxs-lookup"><span data-stu-id="38c9a-315">Response</span></span>
<span data-ttu-id="38c9a-316">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="38c9a-316">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="38c9a-317">示例 2：更新指定用户的属性</span><span class="sxs-lookup"><span data-stu-id="38c9a-317">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="38c9a-318">请求</span><span class="sxs-lookup"><span data-stu-id="38c9a-318">Request</span></span>

<span data-ttu-id="38c9a-319">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="38c9a-319">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="38c9a-320">HTTP</span><span class="sxs-lookup"><span data-stu-id="38c9a-320">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="38c9a-321">C#</span><span class="sxs-lookup"><span data-stu-id="38c9a-321">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38c9a-322">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38c9a-322">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38c9a-323">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38c9a-323">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38c9a-324">Java</span><span class="sxs-lookup"><span data-stu-id="38c9a-324">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38c9a-325">响应</span><span class="sxs-lookup"><span data-stu-id="38c9a-325">Response</span></span>

<span data-ttu-id="38c9a-326">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="38c9a-326">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
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
