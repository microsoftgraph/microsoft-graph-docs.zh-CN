---
title: 更新联系人
description: 更新联系人对象的属性。
ms.openlocfilehash: 2fbf597ebc8a6c65141c64ae42ae42266f14cbde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043970"
---
# <a name="update-contact"></a><span data-ttu-id="b461c-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="b461c-103">Update contact</span></span>

> <span data-ttu-id="b461c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b461c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b461c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b461c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b461c-106">更新联系人对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b461c-106">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b461c-107">权限</span><span class="sxs-lookup"><span data-stu-id="b461c-107">Permissions</span></span>
<span data-ttu-id="b461c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b461c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b461c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b461c-110">Permission type</span></span>      | <span data-ttu-id="b461c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b461c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b461c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b461c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b461c-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b461c-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b461c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b461c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b461c-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b461c-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b461c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b461c-116">Application</span></span> | <span data-ttu-id="b461c-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b461c-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b461c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b461c-118">HTTP request</span></span>
<span data-ttu-id="b461c-119"><!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)从用户的默认[contactFolder](../resources/contactfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="b461c-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="b461c-120">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="b461c-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="b461c-121">[联系人](../resources/contact.md) [contactFolder](../resources/mailfolder.md)子文件夹中包含。</span><span class="sxs-lookup"><span data-stu-id="b461c-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="b461c-122">下面的示例演示一个级别的嵌套，但联系人可以位于子级的子级，依此类推。</span><span class="sxs-lookup"><span data-stu-id="b461c-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b461c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b461c-123">Request headers</span></span>
| <span data-ttu-id="b461c-124">标头</span><span class="sxs-lookup"><span data-stu-id="b461c-124">Header</span></span>       | <span data-ttu-id="b461c-125">值</span><span class="sxs-lookup"><span data-stu-id="b461c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b461c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b461c-126">Authorization</span></span>  | <span data-ttu-id="b461c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b461c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b461c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b461c-129">Content-Type</span></span>  | <span data-ttu-id="b461c-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b461c-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b461c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b461c-132">Request body</span></span>
<span data-ttu-id="b461c-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b461c-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b461c-136">属性</span><span class="sxs-lookup"><span data-stu-id="b461c-136">Property</span></span>     | <span data-ttu-id="b461c-137">类型</span><span class="sxs-lookup"><span data-stu-id="b461c-137">Type</span></span>   |<span data-ttu-id="b461c-138">说明</span><span class="sxs-lookup"><span data-stu-id="b461c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b461c-139">assistantName</span><span class="sxs-lookup"><span data-stu-id="b461c-139">assistantName</span></span>|<span data-ttu-id="b461c-140">String</span><span class="sxs-lookup"><span data-stu-id="b461c-140">String</span></span>|<span data-ttu-id="b461c-141">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="b461c-141">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="b461c-142">birthday</span><span class="sxs-lookup"><span data-stu-id="b461c-142">birthday</span></span>|<span data-ttu-id="b461c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b461c-143">DateTimeOffset</span></span>|<span data-ttu-id="b461c-144">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="b461c-144">The contact's birthday.</span></span>|
|<span data-ttu-id="b461c-145">categories</span><span class="sxs-lookup"><span data-stu-id="b461c-145">categories</span></span>|<span data-ttu-id="b461c-146">String</span><span class="sxs-lookup"><span data-stu-id="b461c-146">String</span></span>|<span data-ttu-id="b461c-147">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="b461c-147">The categories associated with the contact.</span></span>|
|<span data-ttu-id="b461c-148">children</span><span class="sxs-lookup"><span data-stu-id="b461c-148">children</span></span>|<span data-ttu-id="b461c-149">String</span><span class="sxs-lookup"><span data-stu-id="b461c-149">String</span></span>||
|<span data-ttu-id="b461c-150">companyName</span><span class="sxs-lookup"><span data-stu-id="b461c-150">companyName</span></span>|<span data-ttu-id="b461c-151">String</span><span class="sxs-lookup"><span data-stu-id="b461c-151">String</span></span>|<span data-ttu-id="b461c-152">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="b461c-152">The name of the contact's company.</span></span>|
|<span data-ttu-id="b461c-153">department</span><span class="sxs-lookup"><span data-stu-id="b461c-153">department</span></span>|<span data-ttu-id="b461c-154">String</span><span class="sxs-lookup"><span data-stu-id="b461c-154">String</span></span>|<span data-ttu-id="b461c-155">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="b461c-155">The contact's department.</span></span>|
|<span data-ttu-id="b461c-156">displayName</span><span class="sxs-lookup"><span data-stu-id="b461c-156">displayName</span></span>|<span data-ttu-id="b461c-157">String</span><span class="sxs-lookup"><span data-stu-id="b461c-157">String</span></span>|<span data-ttu-id="b461c-158">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b461c-158">The contact's display name.</span></span> <span data-ttu-id="b461c-159">请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。</span><span class="sxs-lookup"><span data-stu-id="b461c-159">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="b461c-160">若要保留现有的值，始终为在更新操作的 displayName 包括它。</span><span class="sxs-lookup"><span data-stu-id="b461c-160">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="b461c-161">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="b461c-161">emailAddresses</span></span>|<span data-ttu-id="b461c-162">[typedEmailAddress](../resources/typedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="b461c-162">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="b461c-163">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b461c-163">The contact's email addresses.</span></span>|
|<span data-ttu-id="b461c-164">fileAs</span><span class="sxs-lookup"><span data-stu-id="b461c-164">fileAs</span></span>|<span data-ttu-id="b461c-165">String</span><span class="sxs-lookup"><span data-stu-id="b461c-165">String</span></span>|<span data-ttu-id="b461c-166">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="b461c-166">The name the contact is filed under.</span></span>|
|<span data-ttu-id="b461c-167">gender</span><span class="sxs-lookup"><span data-stu-id="b461c-167">gender</span></span> |<span data-ttu-id="b461c-168">字符串</span><span class="sxs-lookup"><span data-stu-id="b461c-168">String</span></span> |<span data-ttu-id="b461c-169">联系人的性别。</span><span class="sxs-lookup"><span data-stu-id="b461c-169">The contact's gender.</span></span> |
|<span data-ttu-id="b461c-170">generation</span><span class="sxs-lookup"><span data-stu-id="b461c-170">generation</span></span>|<span data-ttu-id="b461c-171">String</span><span class="sxs-lookup"><span data-stu-id="b461c-171">String</span></span>|<span data-ttu-id="b461c-172">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="b461c-172">The contact's generation.</span></span>|
|<span data-ttu-id="b461c-173">givenName</span><span class="sxs-lookup"><span data-stu-id="b461c-173">givenName</span></span>|<span data-ttu-id="b461c-174">String</span><span class="sxs-lookup"><span data-stu-id="b461c-174">String</span></span>|<span data-ttu-id="b461c-175">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="b461c-175">The contact's given name.</span></span>|
|<span data-ttu-id="b461c-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="b461c-176">imAddresses</span></span>|<span data-ttu-id="b461c-177">String</span><span class="sxs-lookup"><span data-stu-id="b461c-177">String</span></span>|<span data-ttu-id="b461c-178">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="b461c-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="b461c-179">initials</span><span class="sxs-lookup"><span data-stu-id="b461c-179">initials</span></span>|<span data-ttu-id="b461c-180">String</span><span class="sxs-lookup"><span data-stu-id="b461c-180">String</span></span>|<span data-ttu-id="b461c-181">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="b461c-181">The contact's initials.</span></span>|
|<span data-ttu-id="b461c-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b461c-182">jobTitle</span></span>|<span data-ttu-id="b461c-183">String</span><span class="sxs-lookup"><span data-stu-id="b461c-183">String</span></span>|<span data-ttu-id="b461c-184">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="b461c-184">The contact’s job title.</span></span>|
|<span data-ttu-id="b461c-185">manager</span><span class="sxs-lookup"><span data-stu-id="b461c-185">manager</span></span>|<span data-ttu-id="b461c-186">String</span><span class="sxs-lookup"><span data-stu-id="b461c-186">String</span></span>|<span data-ttu-id="b461c-187">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="b461c-187">The name of the contact's manager.</span></span>
|<span data-ttu-id="b461c-188">middleName</span><span class="sxs-lookup"><span data-stu-id="b461c-188">middleName</span></span>|<span data-ttu-id="b461c-189">String</span><span class="sxs-lookup"><span data-stu-id="b461c-189">String</span></span>|<span data-ttu-id="b461c-190">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="b461c-190">The contact's middle name.</span></span>|
|<span data-ttu-id="b461c-191">nickName</span><span class="sxs-lookup"><span data-stu-id="b461c-191">nickName</span></span>|<span data-ttu-id="b461c-192">String</span><span class="sxs-lookup"><span data-stu-id="b461c-192">String</span></span>|<span data-ttu-id="b461c-193">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="b461c-193">The contact's nickname.</span></span>|
|<span data-ttu-id="b461c-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b461c-194">officeLocation</span></span>|<span data-ttu-id="b461c-195">String</span><span class="sxs-lookup"><span data-stu-id="b461c-195">String</span></span>|<span data-ttu-id="b461c-196">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="b461c-196">The location of the contact's office.</span></span>|
|<span data-ttu-id="b461c-197">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b461c-197">parentFolderId</span></span>|<span data-ttu-id="b461c-198">String</span><span class="sxs-lookup"><span data-stu-id="b461c-198">String</span></span>|<span data-ttu-id="b461c-199">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="b461c-199">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="b461c-200">personalNotes</span><span class="sxs-lookup"><span data-stu-id="b461c-200">personalNotes</span></span>|<span data-ttu-id="b461c-201">String</span><span class="sxs-lookup"><span data-stu-id="b461c-201">String</span></span>|<span data-ttu-id="b461c-202">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="b461c-202">The user's notes about the contact.</span></span>|
|<span data-ttu-id="b461c-203">phones</span><span class="sxs-lookup"><span data-stu-id="b461c-203">phones</span></span> |<span data-ttu-id="b461c-204">[phone](../resources/phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="b461c-204">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="b461c-205">例如，家庭电话、 移动电话和商务电话与该联系人，关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b461c-205">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="b461c-206">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="b461c-206">postalAddresses</span></span> |<span data-ttu-id="b461c-207">[physicalAddress](../resources/physicaladdress.md)集合</span><span class="sxs-lookup"><span data-stu-id="b461c-207">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="b461c-208">解决与该联系人，例如家庭地址和业务地址。</span><span class="sxs-lookup"><span data-stu-id="b461c-208">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="b461c-209">profession</span><span class="sxs-lookup"><span data-stu-id="b461c-209">profession</span></span>|<span data-ttu-id="b461c-210">String</span><span class="sxs-lookup"><span data-stu-id="b461c-210">String</span></span>|<span data-ttu-id="b461c-211">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="b461c-211">The contact's profession.</span></span>|
|<span data-ttu-id="b461c-212">spouseName</span><span class="sxs-lookup"><span data-stu-id="b461c-212">spouseName</span></span>|<span data-ttu-id="b461c-213">String</span><span class="sxs-lookup"><span data-stu-id="b461c-213">String</span></span>|<span data-ttu-id="b461c-214">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="b461c-214">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="b461c-215">surname</span><span class="sxs-lookup"><span data-stu-id="b461c-215">surname</span></span>|<span data-ttu-id="b461c-216">String</span><span class="sxs-lookup"><span data-stu-id="b461c-216">String</span></span>|<span data-ttu-id="b461c-217">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="b461c-217">The contact's surname.</span></span>|
|<span data-ttu-id="b461c-218">title</span><span class="sxs-lookup"><span data-stu-id="b461c-218">title</span></span>|<span data-ttu-id="b461c-219">String</span><span class="sxs-lookup"><span data-stu-id="b461c-219">String</span></span>|<span data-ttu-id="b461c-220">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="b461c-220">The contact's title.</span></span>|
|<span data-ttu-id="b461c-221">websites</span><span class="sxs-lookup"><span data-stu-id="b461c-221">websites</span></span> |<span data-ttu-id="b461c-222">[website](../resources/website.md) collection</span><span class="sxs-lookup"><span data-stu-id="b461c-222">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="b461c-223">与联系人关联的网站。</span><span class="sxs-lookup"><span data-stu-id="b461c-223">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="b461c-224">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="b461c-224">weddingAnniversary</span></span> |<span data-ttu-id="b461c-225">日期</span><span class="sxs-lookup"><span data-stu-id="b461c-225">Date</span></span> |<span data-ttu-id="b461c-226">联系人的婚礼周年日。</span><span class="sxs-lookup"><span data-stu-id="b461c-226">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="b461c-227">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="b461c-227">yomiCompanyName</span></span>|<span data-ttu-id="b461c-228">字符串</span><span class="sxs-lookup"><span data-stu-id="b461c-228">String</span></span>|<span data-ttu-id="b461c-p108">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="b461c-p108">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="b461c-231">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="b461c-231">yomiGivenName</span></span>|<span data-ttu-id="b461c-232">字符串</span><span class="sxs-lookup"><span data-stu-id="b461c-232">String</span></span>|<span data-ttu-id="b461c-p109">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="b461c-p109">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="b461c-235">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="b461c-235">yomiSurname</span></span>|<span data-ttu-id="b461c-236">字符串</span><span class="sxs-lookup"><span data-stu-id="b461c-236">String</span></span>|<span data-ttu-id="b461c-p110">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="b461c-p110">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="b461c-239">由于**联系人**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**联系人**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="b461c-239">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b461c-240">响应</span><span class="sxs-lookup"><span data-stu-id="b461c-240">Response</span></span>

<span data-ttu-id="b461c-241">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新[联系人](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b461c-241">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b461c-242">示例</span><span class="sxs-lookup"><span data-stu-id="b461c-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b461c-243">请求</span><span class="sxs-lookup"><span data-stu-id="b461c-243">Request</span></span>
<span data-ttu-id="b461c-244">下面的示例将更新指定的联系人的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b461c-244">The following example updates the personal email address of the specified contact.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="b461c-245">响应</span><span class="sxs-lookup"><span data-stu-id="b461c-245">Response</span></span>
<span data-ttu-id="b461c-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b461c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="b461c-249">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b461c-249">See also</span></span>

- [<span data-ttu-id="b461c-250">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b461c-250">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b461c-251">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="b461c-251">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->