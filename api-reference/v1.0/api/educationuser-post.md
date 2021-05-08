---
title: 创建 educationUser
description: 创建新的 educationUser 对象。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b26e0530fd4beea6d2f604fa46f891e154fefa61
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232176"
---
# <a name="create-educationuser"></a><span data-ttu-id="40688-103">创建 educationUser</span><span class="sxs-lookup"><span data-stu-id="40688-103">Create educationUser</span></span>

<span data-ttu-id="40688-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40688-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40688-105">创建新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40688-105">Create a new [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40688-106">权限</span><span class="sxs-lookup"><span data-stu-id="40688-106">Permissions</span></span>

<span data-ttu-id="40688-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40688-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40688-109">Permission type</span></span>                        | <span data-ttu-id="40688-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40688-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="40688-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40688-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40688-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="40688-112">Not supported.</span></span>                              |
| <span data-ttu-id="40688-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40688-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40688-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40688-114">Not supported.</span></span>                              |
| <span data-ttu-id="40688-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40688-115">Application</span></span>                            | <span data-ttu-id="40688-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40688-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="40688-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40688-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/users
```

## <a name="request-headers"></a><span data-ttu-id="40688-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="40688-118">Request headers</span></span>

| <span data-ttu-id="40688-119">名称</span><span class="sxs-lookup"><span data-stu-id="40688-119">Name</span></span>          | <span data-ttu-id="40688-120">说明</span><span class="sxs-lookup"><span data-stu-id="40688-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="40688-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40688-121">Authorization</span></span> | <span data-ttu-id="40688-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40688-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="40688-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40688-124">Content-Type</span></span>  | <span data-ttu-id="40688-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="40688-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40688-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40688-127">Request body</span></span>

<span data-ttu-id="40688-128">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40688-128">In the request body, supply a JSON representation of the [educationUser](../resources/educationuser.md) object.</span></span>

<span data-ttu-id="40688-129">下表显示创建 [educationUser](../resources/educationuser.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40688-129">The following table shows the properties that are required when you create the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="40688-130">属性</span><span class="sxs-lookup"><span data-stu-id="40688-130">Property</span></span>             | <span data-ttu-id="40688-131">类型</span><span class="sxs-lookup"><span data-stu-id="40688-131">Type</span></span>                                                               | <span data-ttu-id="40688-132">说明</span><span class="sxs-lookup"><span data-stu-id="40688-132">Description</span></span>                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="40688-133">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="40688-133">accountEnabled</span></span>       | <span data-ttu-id="40688-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="40688-134">Boolean</span></span>                                                            | <span data-ttu-id="40688-135">如果帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="40688-135">**True** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="40688-136">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="40688-136">This property is required when a user is created.</span></span> <span data-ttu-id="40688-137">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-137">Supports $filter.</span></span>                                                                                                                                                                                                                               |
| <span data-ttu-id="40688-138">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="40688-138">assignedLicenses</span></span>     | <span data-ttu-id="40688-139">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="40688-139">[assignedLicense](../resources/assignedlicense.md) collection</span></span>      | <span data-ttu-id="40688-p105">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40688-p105">The licenses that are assigned to the user. Not nullable.</span></span>                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="40688-142">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="40688-142">assignedPlans</span></span>        | <span data-ttu-id="40688-143">[assignedPlan](../resources/assignedplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="40688-143">[assignedPlan](../resources/assignedplan.md) collection</span></span>            | <span data-ttu-id="40688-p106">分配给该用户的计划。只读。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40688-p106">The plans that are assigned to the user. Read-only. Not nullable.</span></span>                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="40688-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="40688-147">businessPhones</span></span>       | <span data-ttu-id="40688-148">String collection</span><span class="sxs-lookup"><span data-stu-id="40688-148">String collection</span></span>                                                  | <span data-ttu-id="40688-149">用户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="40688-149">The telephone numbers for the user.</span></span> <span data-ttu-id="40688-150">**注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="40688-150">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                                                                                                                                                           |
| <span data-ttu-id="40688-151">createdBy</span><span class="sxs-lookup"><span data-stu-id="40688-151">createdBy</span></span>            | [<span data-ttu-id="40688-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="40688-152">identitySet</span></span>](../resources/identityset.md)                         | <span data-ttu-id="40688-153">创建了用户的实体。</span><span class="sxs-lookup"><span data-stu-id="40688-153">Entity who created the user.</span></span>                                                                                                                                                                                                                                                                                                                                |
| <span data-ttu-id="40688-154">department</span><span class="sxs-lookup"><span data-stu-id="40688-154">department</span></span>           | <span data-ttu-id="40688-155">String</span><span class="sxs-lookup"><span data-stu-id="40688-155">String</span></span>                                                             | <span data-ttu-id="40688-p108">用户工作部门的名称。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-p108">The name for the department in which the user works. Supports $filter.</span></span>                                                                                                                                                                                                                                                                                      |
| <span data-ttu-id="40688-158">displayName</span><span class="sxs-lookup"><span data-stu-id="40688-158">displayName</span></span>          | <span data-ttu-id="40688-159">String</span><span class="sxs-lookup"><span data-stu-id="40688-159">String</span></span>                                                             | <span data-ttu-id="40688-160">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="40688-160">The name displayed in the address book for the user.</span></span> <span data-ttu-id="40688-161">这通常是用户名字、中间名首字母和姓氏的组合。</span><span class="sxs-lookup"><span data-stu-id="40688-161">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="40688-162">此属性在创建用户时是必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="40688-162">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="40688-163">支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="40688-163">Supports $filter and $orderby.</span></span>                                                                                      |
| <span data-ttu-id="40688-164">externalSource</span><span class="sxs-lookup"><span data-stu-id="40688-164">externalSource</span></span>       | <span data-ttu-id="40688-165">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="40688-165">educationExternalSource</span></span>                                            | <span data-ttu-id="40688-166">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="40688-166">Where this user was created from.</span></span> <span data-ttu-id="40688-167">可取值为：`sis`、`manual`。</span><span class="sxs-lookup"><span data-stu-id="40688-167">Possible values are: `sis`, `manual`.</span></span>                                                                                                                                                                                                                                                                                     |
| <span data-ttu-id="40688-168">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="40688-168">externalSourceDetail</span></span> | <span data-ttu-id="40688-169">String</span><span class="sxs-lookup"><span data-stu-id="40688-169">String</span></span>                                                             | <span data-ttu-id="40688-170">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="40688-170">The name of the external source this resources was generated from.</span></span>                                                                                                                                                                                                                                                                                          |
| <span data-ttu-id="40688-171">givenName</span><span class="sxs-lookup"><span data-stu-id="40688-171">givenName</span></span>            | <span data-ttu-id="40688-172">String</span><span class="sxs-lookup"><span data-stu-id="40688-172">String</span></span>                                                             | <span data-ttu-id="40688-p111">用户的名。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-p111">The given name (first name) of the user. Supports $filter.</span></span>                                                                                                                                                                                                                                                                                                  |
| <span data-ttu-id="40688-175">mail</span><span class="sxs-lookup"><span data-stu-id="40688-175">mail</span></span>                 | <span data-ttu-id="40688-176">String</span><span class="sxs-lookup"><span data-stu-id="40688-176">String</span></span>                                                             | <span data-ttu-id="40688-177">用户的 SMTP 地址；例如，“jeff@contoso.onmicrosoft.com”。</span><span class="sxs-lookup"><span data-stu-id="40688-177">The SMTP address for the user; for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="40688-178">只读。</span><span class="sxs-lookup"><span data-stu-id="40688-178">Read-Only.</span></span> <span data-ttu-id="40688-179">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-179">Supports $filter.</span></span>                                                                                                                                                                                                                                                    |
| <span data-ttu-id="40688-180">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="40688-180">mailingAddress</span></span>       | [<span data-ttu-id="40688-181">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="40688-181">physicalAddress</span></span>](../resources/physicaladdress.md)                 | <span data-ttu-id="40688-182">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="40688-182">Mail address of user.</span></span>                                                                                                                                                                                                                                                                                                                                       |
| <span data-ttu-id="40688-183">mailNickname</span><span class="sxs-lookup"><span data-stu-id="40688-183">mailNickname</span></span>         | <span data-ttu-id="40688-184">String</span><span class="sxs-lookup"><span data-stu-id="40688-184">String</span></span>                                                             | <span data-ttu-id="40688-p113">用户的邮件别名。创建用户时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-p113">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>                                                                                                                                                                                                                                                      |
| <span data-ttu-id="40688-188">middleName</span><span class="sxs-lookup"><span data-stu-id="40688-188">middleName</span></span>           | <span data-ttu-id="40688-189">String</span><span class="sxs-lookup"><span data-stu-id="40688-189">String</span></span>                                                             | <span data-ttu-id="40688-190">用户的中间名。</span><span class="sxs-lookup"><span data-stu-id="40688-190">The middle name of user.</span></span>                                                                                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="40688-191">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="40688-191">mobilePhone</span></span>          | <span data-ttu-id="40688-192">String</span><span class="sxs-lookup"><span data-stu-id="40688-192">String</span></span>                                                             | <span data-ttu-id="40688-193">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="40688-193">The primary cellular telephone number for the user.</span></span>                                                                                                                                                                                                                                                                                                         |
| <span data-ttu-id="40688-194">onPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="40688-194">onPremisesInfo</span></span>       | [<span data-ttu-id="40688-195">educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="40688-195">educationOnPremisesInfo</span></span>](../resources/educationonpremisesinfo.md) | <span data-ttu-id="40688-196">用于将 AAD 用户与它的 Active Directory 对应项关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="40688-196">Additional information used to associate the AAD user with it's Active Directory counterpart.</span></span>                                                                                                                                                                                                                                                               |
| <span data-ttu-id="40688-197">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="40688-197">passwordPolicies</span></span>     | <span data-ttu-id="40688-198">String</span><span class="sxs-lookup"><span data-stu-id="40688-198">String</span></span>                                                             | <span data-ttu-id="40688-199">指定用户的密码策略。</span><span class="sxs-lookup"><span data-stu-id="40688-199">Specifies password policies for the user.</span></span> <span data-ttu-id="40688-200">此值是一个枚举，具有一个可能值 “DisableStrongPassword”，允许指定比默认策略弱的密码。</span><span class="sxs-lookup"><span data-stu-id="40688-200">This value is an enumeration with one possible value being "DisableStrongPassword", which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="40688-201">还可以指定 “DisablePasswordExpiration”。</span><span class="sxs-lookup"><span data-stu-id="40688-201">"DisablePasswordExpiration" can also be specified.</span></span> <span data-ttu-id="40688-202">可以同时指定两个值；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="40688-202">The two can be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span> |
| <span data-ttu-id="40688-203">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="40688-203">passwordProfile</span></span>      | [<span data-ttu-id="40688-204">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="40688-204">passwordProfile</span></span>](../resources/passwordprofile.md)                 | <span data-ttu-id="40688-205">指定用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="40688-205">Specifies the password profile for the user.</span></span> <span data-ttu-id="40688-206">配置文件包含用户的密码。</span><span class="sxs-lookup"><span data-stu-id="40688-206">The profile contains the user's password.</span></span> <span data-ttu-id="40688-207">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="40688-207">This property is required when a user is created.</span></span> <span data-ttu-id="40688-208">配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。</span><span class="sxs-lookup"><span data-stu-id="40688-208">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="40688-209">默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="40688-209">By default, a strong password is required.</span></span>                                                        |
| <span data-ttu-id="40688-210">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="40688-210">preferredLanguage</span></span>    | <span data-ttu-id="40688-211">String</span><span class="sxs-lookup"><span data-stu-id="40688-211">String</span></span>                                                             | <span data-ttu-id="40688-212">用户的首选语言。</span><span class="sxs-lookup"><span data-stu-id="40688-212">The preferred language for the user.</span></span> <span data-ttu-id="40688-213">应遵循 ISO 639-1 代码；例如“en-US”。</span><span class="sxs-lookup"><span data-stu-id="40688-213">Should follow ISO 639-1 Code; for example, "en-US".</span></span>                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="40688-214">primaryRole</span><span class="sxs-lookup"><span data-stu-id="40688-214">primaryRole</span></span>          | <span data-ttu-id="40688-215">educationUserRole</span><span class="sxs-lookup"><span data-stu-id="40688-215">educationUserRole</span></span>                                                  | <span data-ttu-id="40688-216">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="40688-216">Default role for a user.</span></span> <span data-ttu-id="40688-217">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="40688-217">The user's role might be different in an individual class.</span></span> <span data-ttu-id="40688-218">可取值为：`student`、`teacher`、`none`。</span><span class="sxs-lookup"><span data-stu-id="40688-218">Possible values are: `student`, `teacher`, `none`.</span></span>                                                                                                                                                                                                                      |
| <span data-ttu-id="40688-219">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="40688-219">provisionedPlans</span></span>     | <span data-ttu-id="40688-220">[provisionedPlan](../resources/provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="40688-220">[provisionedPlan](../resources/provisionedplan.md) collection</span></span>      | <span data-ttu-id="40688-p118">为用户设置的计划。只读。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40688-p118">The plans that are provisioned for the user. Read-only. Not nullable.</span></span>                                                                                                                                                                                                                                                                                       |
| <span data-ttu-id="40688-224">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="40688-224">residenceAddress</span></span>     | [<span data-ttu-id="40688-225">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="40688-225">physicalAddress</span></span>](../resources/physicaladdress.md)                 | <span data-ttu-id="40688-226">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="40688-226">Address where user lives.</span></span>                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="40688-227">student</span><span class="sxs-lookup"><span data-stu-id="40688-227">student</span></span>              | [<span data-ttu-id="40688-228">educationStudent</span><span class="sxs-lookup"><span data-stu-id="40688-228">educationStudent</span></span>](../resources/educationstudent.md)               | <span data-ttu-id="40688-229">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="40688-229">If the primary role is student, this block will contain student specific data.</span></span>                                                                                                                                                                                                                                                                              |
| <span data-ttu-id="40688-230">surname</span><span class="sxs-lookup"><span data-stu-id="40688-230">surname</span></span>              | <span data-ttu-id="40688-231">String</span><span class="sxs-lookup"><span data-stu-id="40688-231">String</span></span>                                                             | <span data-ttu-id="40688-p119">用户的姓氏。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-p119">The user's surname (family name or last name). Supports $filter.</span></span>                                                                                                                                                                                                                                                                                            |
| <span data-ttu-id="40688-234">teacher</span><span class="sxs-lookup"><span data-stu-id="40688-234">teacher</span></span>              | [<span data-ttu-id="40688-235">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="40688-235">educationTeacher</span></span>](../resources/educationteacher.md)               | <span data-ttu-id="40688-236">如果主要角色是教师，则此块将包含特定于教师的数据。</span><span class="sxs-lookup"><span data-stu-id="40688-236">If the primary role is teacher, this block will contain teacher specific data.</span></span>                                                                                                                                                                                                                                                                              |
| <span data-ttu-id="40688-237">usageLocation</span><span class="sxs-lookup"><span data-stu-id="40688-237">usageLocation</span></span>        | <span data-ttu-id="40688-238">String</span><span class="sxs-lookup"><span data-stu-id="40688-238">String</span></span>                                                             | <span data-ttu-id="40688-239">两个字母组成的国家/地区代码（ISO 标准 3166）。</span><span class="sxs-lookup"><span data-stu-id="40688-239">A two-letter country code (ISO standard 3166).</span></span> <span data-ttu-id="40688-240">鉴于检查服务在国家/地区的可用性的法律要求，这对将分配许可证的用户而言是必需的。</span><span class="sxs-lookup"><span data-stu-id="40688-240">Required for users who will be assigned licenses due to a legal requirement to check for availability of services in countries or regions.</span></span> <span data-ttu-id="40688-241">示例包括：“US”、“JP”和“GB”。</span><span class="sxs-lookup"><span data-stu-id="40688-241">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="40688-242">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40688-242">Not nullable.</span></span> <span data-ttu-id="40688-243">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-243">Supports $filter.</span></span>                                                                                           |
| <span data-ttu-id="40688-244">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="40688-244">userPrincipalName</span></span>    | <span data-ttu-id="40688-245">String</span><span class="sxs-lookup"><span data-stu-id="40688-245">String</span></span>                                                             | <span data-ttu-id="40688-246">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="40688-246">The user principal name (UPN) of the user.</span></span>                                                                                                                                                                                                                                                                                                                  |
| <span data-ttu-id="40688-247">userType</span><span class="sxs-lookup"><span data-stu-id="40688-247">userType</span></span>             | <span data-ttu-id="40688-248">String</span><span class="sxs-lookup"><span data-stu-id="40688-248">String</span></span>                                                             | <span data-ttu-id="40688-p121">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="40688-p121">A string value that can be used to classify user types in your directory, such as "Member" and "Guest". Supports $filter.</span></span>                                                                                                                                                                                                                                   |

## <a name="response"></a><span data-ttu-id="40688-251">响应</span><span class="sxs-lookup"><span data-stu-id="40688-251">Response</span></span>

<span data-ttu-id="40688-252">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40688-252">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40688-253">示例</span><span class="sxs-lookup"><span data-stu-id="40688-253">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40688-254">请求</span><span class="sxs-lookup"><span data-stu-id="40688-254">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/users
Content-Type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.educationUser",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```

### <a name="response"></a><span data-ttu-id="40688-255">响应</span><span class="sxs-lookup"><span data-stu-id="40688-255">Response</span></span>

> <span data-ttu-id="40688-256">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="40688-256">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```
