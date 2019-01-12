---
title: 更新用户
description: 更新 user 对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00efdeed6fdb85aeccde5fae63e813b8b5e65961
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939110"
---
# <a name="update-user"></a><span data-ttu-id="bca06-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="bca06-103">Update user</span></span>

> <span data-ttu-id="bca06-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bca06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bca06-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bca06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bca06-106">更新 user 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bca06-106">Update the properties of a user object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bca06-107">权限</span><span class="sxs-lookup"><span data-stu-id="bca06-107">Permissions</span></span>
<span data-ttu-id="bca06-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bca06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca06-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bca06-110">Permission type</span></span>      | <span data-ttu-id="bca06-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bca06-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bca06-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bca06-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bca06-113">User.ReadWrite，User.ReadWrite.All，Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca06-113">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="bca06-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bca06-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bca06-115">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bca06-115">User.ReadWrite</span></span>    |
|<span data-ttu-id="bca06-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bca06-116">Application</span></span> | <span data-ttu-id="bca06-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca06-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bca06-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bca06-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```
## <a name="request-headers"></a><span data-ttu-id="bca06-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bca06-119">Request headers</span></span>
| <span data-ttu-id="bca06-120">标头</span><span class="sxs-lookup"><span data-stu-id="bca06-120">Header</span></span>       | <span data-ttu-id="bca06-121">值</span><span class="sxs-lookup"><span data-stu-id="bca06-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="bca06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bca06-122">Authorization</span></span>  | <span data-ttu-id="bca06-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bca06-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bca06-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bca06-125">Content-Type</span></span>  | <span data-ttu-id="bca06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bca06-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bca06-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bca06-127">Request body</span></span>
<span data-ttu-id="bca06-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bca06-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bca06-131">属性</span><span class="sxs-lookup"><span data-stu-id="bca06-131">Property</span></span>     | <span data-ttu-id="bca06-132">类型</span><span class="sxs-lookup"><span data-stu-id="bca06-132">Type</span></span>   |<span data-ttu-id="bca06-133">说明</span><span class="sxs-lookup"><span data-stu-id="bca06-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bca06-134">aboutMe</span><span class="sxs-lookup"><span data-stu-id="bca06-134">aboutMe</span></span>|<span data-ttu-id="bca06-135">String</span><span class="sxs-lookup"><span data-stu-id="bca06-135">String</span></span>|<span data-ttu-id="bca06-136">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="bca06-136">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="bca06-137">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="bca06-137">accountEnabled</span></span>|<span data-ttu-id="bca06-138">布尔</span><span class="sxs-lookup"><span data-stu-id="bca06-138">Boolean</span></span>| <span data-ttu-id="bca06-p105">启用帐户时为 **true**，否则为 **false**。创建用户时此属性是必需的。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p105">**true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.</span></span>    |
|<span data-ttu-id="bca06-142">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="bca06-142">assignedLicenses</span></span>|<span data-ttu-id="bca06-143">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="bca06-143">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="bca06-p106">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="bca06-p106">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="bca06-146">birthday</span><span class="sxs-lookup"><span data-stu-id="bca06-146">birthday</span></span>|<span data-ttu-id="bca06-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca06-147">DateTimeOffset</span></span>|<span data-ttu-id="bca06-p107">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bca06-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bca06-151">city</span><span class="sxs-lookup"><span data-stu-id="bca06-151">city</span></span>|<span data-ttu-id="bca06-152">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-152">String</span></span>|<span data-ttu-id="bca06-p108">用户所在的城市。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p108">The city in which the user is located. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-155">country</span><span class="sxs-lookup"><span data-stu-id="bca06-155">country</span></span>|<span data-ttu-id="bca06-156">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-156">String</span></span>|<span data-ttu-id="bca06-p109">用户所在的国家/地区；例如，“美国”或“英国”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p109">The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-159">department</span><span class="sxs-lookup"><span data-stu-id="bca06-159">department</span></span>|<span data-ttu-id="bca06-160">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-160">String</span></span>|<span data-ttu-id="bca06-p110">用户工作部门的名称。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p110">The name for the department in which the user works. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-163">displayName</span><span class="sxs-lookup"><span data-stu-id="bca06-163">displayName</span></span>|<span data-ttu-id="bca06-164">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-164">String</span></span>|<span data-ttu-id="bca06-p111">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="bca06-p111">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="bca06-169">雇员 id</span><span class="sxs-lookup"><span data-stu-id="bca06-169">employeeId</span></span>|<span data-ttu-id="bca06-170">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-170">String</span></span>|<span data-ttu-id="bca06-171">分配给用户组织的员工标识符。</span><span class="sxs-lookup"><span data-stu-id="bca06-171">The employee identifier assigned to the user by the organization.</span></span> <span data-ttu-id="bca06-172">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-172">Supports $filter.</span></span>|
|<span data-ttu-id="bca06-173">givenName</span><span class="sxs-lookup"><span data-stu-id="bca06-173">givenName</span></span>|<span data-ttu-id="bca06-174">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-174">String</span></span>|<span data-ttu-id="bca06-p113">用户的名。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p113">The given name (first name) of the user. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-177">hireDate</span><span class="sxs-lookup"><span data-stu-id="bca06-177">hireDate</span></span>|<span data-ttu-id="bca06-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca06-178">DateTimeOffset</span></span>|<span data-ttu-id="bca06-p114">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bca06-p114">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bca06-182">interests</span><span class="sxs-lookup"><span data-stu-id="bca06-182">interests</span></span>|<span data-ttu-id="bca06-183">String collection</span><span class="sxs-lookup"><span data-stu-id="bca06-183">String collection</span></span>|<span data-ttu-id="bca06-184">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="bca06-184">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="bca06-185">jobTitle</span><span class="sxs-lookup"><span data-stu-id="bca06-185">jobTitle</span></span>|<span data-ttu-id="bca06-186">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-186">String</span></span>|<span data-ttu-id="bca06-p115">用户的职务。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p115">The user’s job title. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-189">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bca06-189">mailNickname</span></span>|<span data-ttu-id="bca06-190">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-190">String</span></span>|<span data-ttu-id="bca06-p116">用户的邮件别名。创建用户时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p116">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-194">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="bca06-194">mobilePhone</span></span>|<span data-ttu-id="bca06-195">String</span><span class="sxs-lookup"><span data-stu-id="bca06-195">String</span></span>|<span data-ttu-id="bca06-196">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="bca06-196">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="bca06-197">mySite</span><span class="sxs-lookup"><span data-stu-id="bca06-197">mySite</span></span>|<span data-ttu-id="bca06-198">String</span><span class="sxs-lookup"><span data-stu-id="bca06-198">String</span></span>|<span data-ttu-id="bca06-199">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="bca06-199">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="bca06-200">officeLocation</span><span class="sxs-lookup"><span data-stu-id="bca06-200">officeLocation</span></span>|<span data-ttu-id="bca06-201">String</span><span class="sxs-lookup"><span data-stu-id="bca06-201">String</span></span>|<span data-ttu-id="bca06-202">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="bca06-202">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="bca06-203">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="bca06-203">onPremisesImmutableId</span></span>|<span data-ttu-id="bca06-204">String</span><span class="sxs-lookup"><span data-stu-id="bca06-204">String</span></span>|<span data-ttu-id="bca06-p117">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。**重要说明：** 指定该属性时不能使用 **$** 和 **_** 字符。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p117">This property is used to associate an on-premises Active Directory user account to their Azure AD user object. This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property. **Important:** The **$** and **_** characters cannot be used when specifying this property. Supports $filter.</span></span>                            |
|<span data-ttu-id="bca06-209">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="bca06-209">passwordPolicies</span></span>|<span data-ttu-id="bca06-210">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-210">String</span></span>|<span data-ttu-id="bca06-p118">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="bca06-p118">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="bca06-215">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="bca06-215">passwordProfile</span></span>|[<span data-ttu-id="bca06-216">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="bca06-216">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="bca06-p119">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="bca06-p119">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="bca06-222">pastProjects</span><span class="sxs-lookup"><span data-stu-id="bca06-222">pastProjects</span></span>|<span data-ttu-id="bca06-223">String collection</span><span class="sxs-lookup"><span data-stu-id="bca06-223">String collection</span></span>|<span data-ttu-id="bca06-224">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="bca06-224">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="bca06-225">postalCode</span><span class="sxs-lookup"><span data-stu-id="bca06-225">postalCode</span></span>|<span data-ttu-id="bca06-226">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-226">String</span></span>|<span data-ttu-id="bca06-p120">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="bca06-p120">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="bca06-230">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="bca06-230">preferredLanguage</span></span>|<span data-ttu-id="bca06-231">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-231">String</span></span>|<span data-ttu-id="bca06-p121">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="bca06-p121">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="bca06-234">preferredName</span><span class="sxs-lookup"><span data-stu-id="bca06-234">preferredName</span></span>|<span data-ttu-id="bca06-235">String</span><span class="sxs-lookup"><span data-stu-id="bca06-235">String</span></span>|<span data-ttu-id="bca06-236">用户的首选名称。</span><span class="sxs-lookup"><span data-stu-id="bca06-236">The preferred name for the user.</span></span>|
|<span data-ttu-id="bca06-237">responsibilities</span><span class="sxs-lookup"><span data-stu-id="bca06-237">responsibilities</span></span>|<span data-ttu-id="bca06-238">String collection</span><span class="sxs-lookup"><span data-stu-id="bca06-238">String collection</span></span>|<span data-ttu-id="bca06-239">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="bca06-239">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="bca06-240">schools</span><span class="sxs-lookup"><span data-stu-id="bca06-240">schools</span></span>|<span data-ttu-id="bca06-241">String collection</span><span class="sxs-lookup"><span data-stu-id="bca06-241">String collection</span></span>|<span data-ttu-id="bca06-242">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="bca06-242">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="bca06-243">skills</span><span class="sxs-lookup"><span data-stu-id="bca06-243">skills</span></span>|<span data-ttu-id="bca06-244">String collection</span><span class="sxs-lookup"><span data-stu-id="bca06-244">String collection</span></span>|<span data-ttu-id="bca06-245">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="bca06-245">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="bca06-246">state</span><span class="sxs-lookup"><span data-stu-id="bca06-246">state</span></span>|<span data-ttu-id="bca06-247">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-247">String</span></span>|<span data-ttu-id="bca06-p122">用户地址中的省/市/自治区或省。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p122">The state or province in the user's address. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-250">streetAddress</span><span class="sxs-lookup"><span data-stu-id="bca06-250">streetAddress</span></span>|<span data-ttu-id="bca06-251">String</span><span class="sxs-lookup"><span data-stu-id="bca06-251">String</span></span>|<span data-ttu-id="bca06-252">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="bca06-252">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="bca06-253">surname</span><span class="sxs-lookup"><span data-stu-id="bca06-253">surname</span></span>|<span data-ttu-id="bca06-254">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-254">String</span></span>|<span data-ttu-id="bca06-p123">用户的姓氏。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p123">The user's surname (family name or last name). Supports $filter.</span></span>|
|<span data-ttu-id="bca06-257">usageLocation</span><span class="sxs-lookup"><span data-stu-id="bca06-257">usageLocation</span></span>|<span data-ttu-id="bca06-258">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-258">String</span></span>|<span data-ttu-id="bca06-p124">两个字母的国家/地区代码（ISO 标准 3166）。为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。示例包括：“US”、“JP”和“GB”。不可为 null。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p124">A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.</span></span>|
|<span data-ttu-id="bca06-264">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bca06-264">userPrincipalName</span></span>|<span data-ttu-id="bca06-265">String</span><span class="sxs-lookup"><span data-stu-id="bca06-265">String</span></span>|<span data-ttu-id="bca06-p125">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="bca06-p125">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="bca06-273">userType</span><span class="sxs-lookup"><span data-stu-id="bca06-273">userType</span></span>|<span data-ttu-id="bca06-274">字符串</span><span class="sxs-lookup"><span data-stu-id="bca06-274">String</span></span>|<span data-ttu-id="bca06-p126">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="bca06-p126">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>          |

<span data-ttu-id="bca06-277">由于**用户**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**用户**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="bca06-277">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="bca06-278">响应</span><span class="sxs-lookup"><span data-stu-id="bca06-278">Response</span></span>

<span data-ttu-id="bca06-279">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bca06-279">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="bca06-280">示例</span><span class="sxs-lookup"><span data-stu-id="bca06-280">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bca06-281">请求</span><span class="sxs-lookup"><span data-stu-id="bca06-281">Request</span></span>
<span data-ttu-id="bca06-282">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bca06-282">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bca06-283">响应</span><span class="sxs-lookup"><span data-stu-id="bca06-283">Response</span></span>
<span data-ttu-id="bca06-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bca06-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="bca06-287">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bca06-287">See also</span></span>

- [<span data-ttu-id="bca06-288">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bca06-288">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bca06-289">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="bca06-289">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bca06-290">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="bca06-290">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
