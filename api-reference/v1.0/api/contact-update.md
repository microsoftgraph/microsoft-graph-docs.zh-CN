---
title: 更新联系人
description: 更新 contact 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 214f9d019a1b3fcf7813c29ebcce2244bc7de98e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003229"
---
# <a name="update-contact"></a><span data-ttu-id="79d2f-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="79d2f-103">Update contact</span></span>

<span data-ttu-id="79d2f-104">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="79d2f-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79d2f-105">权限</span><span class="sxs-lookup"><span data-stu-id="79d2f-105">Permissions</span></span>
<span data-ttu-id="79d2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79d2f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="79d2f-108">Permission type</span></span>      | <span data-ttu-id="79d2f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79d2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79d2f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79d2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79d2f-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79d2f-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="79d2f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79d2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79d2f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79d2f-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="79d2f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="79d2f-114">Application</span></span> | <span data-ttu-id="79d2f-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79d2f-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79d2f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79d2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="79d2f-117">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="79d2f-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="79d2f-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="79d2f-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="79d2f-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79d2f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="79d2f-121">Request headers</span></span>
| <span data-ttu-id="79d2f-122">标头</span><span class="sxs-lookup"><span data-stu-id="79d2f-122">Header</span></span>       | <span data-ttu-id="79d2f-123">值</span><span class="sxs-lookup"><span data-stu-id="79d2f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79d2f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79d2f-124">Authorization</span></span>  | <span data-ttu-id="79d2f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79d2f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79d2f-127">Content-Type</span></span>  | <span data-ttu-id="79d2f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="79d2f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79d2f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="79d2f-130">Request body</span></span>
<span data-ttu-id="79d2f-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79d2f-134">属性</span><span class="sxs-lookup"><span data-stu-id="79d2f-134">Property</span></span>     | <span data-ttu-id="79d2f-135">类型</span><span class="sxs-lookup"><span data-stu-id="79d2f-135">Type</span></span>   |<span data-ttu-id="79d2f-136">说明</span><span class="sxs-lookup"><span data-stu-id="79d2f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79d2f-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="79d2f-137">assistantName</span></span>|<span data-ttu-id="79d2f-138">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-138">String</span></span>|<span data-ttu-id="79d2f-139">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="79d2f-140">birthday</span><span class="sxs-lookup"><span data-stu-id="79d2f-140">birthday</span></span>|<span data-ttu-id="79d2f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d2f-141">DateTimeOffset</span></span>|<span data-ttu-id="79d2f-142">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="79d2f-142">The contact's birthday.</span></span>|
|<span data-ttu-id="79d2f-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="79d2f-143">businessAddress</span></span>|[<span data-ttu-id="79d2f-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="79d2f-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="79d2f-145">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="79d2f-145">The contact's business address.</span></span>|
|<span data-ttu-id="79d2f-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="79d2f-146">businessHomePage</span></span>|<span data-ttu-id="79d2f-147">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-147">String</span></span>|<span data-ttu-id="79d2f-148">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="79d2f-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="79d2f-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="79d2f-149">businessPhones</span></span>|<span data-ttu-id="79d2f-150">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-150">String</span></span>|<span data-ttu-id="79d2f-151">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="79d2f-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="79d2f-152">categories</span><span class="sxs-lookup"><span data-stu-id="79d2f-152">categories</span></span>|<span data-ttu-id="79d2f-153">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-153">String</span></span>|<span data-ttu-id="79d2f-154">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="79d2f-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="79d2f-155">children</span><span class="sxs-lookup"><span data-stu-id="79d2f-155">children</span></span>|<span data-ttu-id="79d2f-156">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-156">String</span></span>|<span data-ttu-id="79d2f-157">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="79d2f-158">companyName</span><span class="sxs-lookup"><span data-stu-id="79d2f-158">companyName</span></span>|<span data-ttu-id="79d2f-159">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-159">String</span></span>|<span data-ttu-id="79d2f-160">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="79d2f-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="79d2f-161">department</span><span class="sxs-lookup"><span data-stu-id="79d2f-161">department</span></span>|<span data-ttu-id="79d2f-162">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-162">String</span></span>|<span data-ttu-id="79d2f-163">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="79d2f-163">The contact's department.</span></span>|
|<span data-ttu-id="79d2f-164">displayName</span><span class="sxs-lookup"><span data-stu-id="79d2f-164">displayName</span></span>|<span data-ttu-id="79d2f-165">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-165">String</span></span>|<span data-ttu-id="79d2f-166">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="79d2f-166">The contact's display name.</span></span> <span data-ttu-id="79d2f-167">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="79d2f-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="79d2f-168">若要保留预先存在的值，请始终在更新操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="79d2f-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="79d2f-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="79d2f-169">emailAddresses</span></span>|<span data-ttu-id="79d2f-170">[EmailAddress](../resources/emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79d2f-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="79d2f-171">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="79d2f-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="79d2f-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="79d2f-172">fileAs</span></span>|<span data-ttu-id="79d2f-173">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-173">String</span></span>|<span data-ttu-id="79d2f-174">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="79d2f-175">generation</span><span class="sxs-lookup"><span data-stu-id="79d2f-175">generation</span></span>|<span data-ttu-id="79d2f-176">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-176">String</span></span>|<span data-ttu-id="79d2f-177">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="79d2f-177">The contact's generation.</span></span>|
|<span data-ttu-id="79d2f-178">givenName</span><span class="sxs-lookup"><span data-stu-id="79d2f-178">givenName</span></span>|<span data-ttu-id="79d2f-179">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-179">String</span></span>|<span data-ttu-id="79d2f-180">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-180">The contact's given name.</span></span>|
|<span data-ttu-id="79d2f-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="79d2f-181">homeAddress</span></span>|[<span data-ttu-id="79d2f-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="79d2f-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="79d2f-183">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="79d2f-183">The contact's home address.</span></span>|
|<span data-ttu-id="79d2f-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="79d2f-184">homePhones</span></span>|<span data-ttu-id="79d2f-185">String collection</span><span class="sxs-lookup"><span data-stu-id="79d2f-185">String collection</span></span>|<span data-ttu-id="79d2f-186">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="79d2f-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="79d2f-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="79d2f-187">imAddresses</span></span>|<span data-ttu-id="79d2f-188">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-188">String</span></span>|<span data-ttu-id="79d2f-189">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="79d2f-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="79d2f-190">initials</span><span class="sxs-lookup"><span data-stu-id="79d2f-190">initials</span></span>|<span data-ttu-id="79d2f-191">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-191">String</span></span>|<span data-ttu-id="79d2f-192">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="79d2f-192">The contact's initials.</span></span>|
|<span data-ttu-id="79d2f-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="79d2f-193">jobTitle</span></span>|<span data-ttu-id="79d2f-194">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-194">String</span></span>|<span data-ttu-id="79d2f-195">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="79d2f-195">The contact’s job title.</span></span>|
|<span data-ttu-id="79d2f-196">manager</span><span class="sxs-lookup"><span data-stu-id="79d2f-196">manager</span></span>|<span data-ttu-id="79d2f-197">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-197">String</span></span>|<span data-ttu-id="79d2f-198">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="79d2f-199">middleName</span><span class="sxs-lookup"><span data-stu-id="79d2f-199">middleName</span></span>|<span data-ttu-id="79d2f-200">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-200">String</span></span>|<span data-ttu-id="79d2f-201">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-201">The contact's middle name.</span></span>|
|<span data-ttu-id="79d2f-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="79d2f-202">mobilePhone</span></span>|<span data-ttu-id="79d2f-203">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-203">String</span></span>|<span data-ttu-id="79d2f-204">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="79d2f-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="79d2f-205">nickName</span><span class="sxs-lookup"><span data-stu-id="79d2f-205">nickName</span></span>|<span data-ttu-id="79d2f-206">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-206">String</span></span>|<span data-ttu-id="79d2f-207">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="79d2f-207">The contact's nickname.</span></span>|
|<span data-ttu-id="79d2f-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="79d2f-208">officeLocation</span></span>|<span data-ttu-id="79d2f-209">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-209">String</span></span>|<span data-ttu-id="79d2f-210">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="79d2f-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="79d2f-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="79d2f-211">otherAddress</span></span>|[<span data-ttu-id="79d2f-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="79d2f-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="79d2f-213">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="79d2f-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="79d2f-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="79d2f-214">parentFolderId</span></span>|<span data-ttu-id="79d2f-215">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-215">String</span></span>|<span data-ttu-id="79d2f-216">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="79d2f-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="79d2f-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="79d2f-217">personalNotes</span></span>|<span data-ttu-id="79d2f-218">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-218">String</span></span>|<span data-ttu-id="79d2f-219">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="79d2f-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="79d2f-220">profession</span><span class="sxs-lookup"><span data-stu-id="79d2f-220">profession</span></span>|<span data-ttu-id="79d2f-221">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-221">String</span></span>|<span data-ttu-id="79d2f-222">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="79d2f-222">The contact's profession.</span></span>|
|<span data-ttu-id="79d2f-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="79d2f-223">spouseName</span></span>|<span data-ttu-id="79d2f-224">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-224">String</span></span>|<span data-ttu-id="79d2f-225">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="79d2f-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="79d2f-226">surname</span><span class="sxs-lookup"><span data-stu-id="79d2f-226">surname</span></span>|<span data-ttu-id="79d2f-227">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-227">String</span></span>|<span data-ttu-id="79d2f-228">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="79d2f-228">The contact's surname.</span></span>|
|<span data-ttu-id="79d2f-229">title</span><span class="sxs-lookup"><span data-stu-id="79d2f-229">title</span></span>|<span data-ttu-id="79d2f-230">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-230">String</span></span>|<span data-ttu-id="79d2f-231">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="79d2f-231">The contact's title.</span></span>|
|<span data-ttu-id="79d2f-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="79d2f-232">yomiCompanyName</span></span>|<span data-ttu-id="79d2f-233">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-233">String</span></span>|<span data-ttu-id="79d2f-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="79d2f-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="79d2f-236">yomiGivenName</span></span>|<span data-ttu-id="79d2f-237">字符串</span><span class="sxs-lookup"><span data-stu-id="79d2f-237">String</span></span>|<span data-ttu-id="79d2f-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="79d2f-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="79d2f-240">yomiSurname</span></span>|<span data-ttu-id="79d2f-241">String</span><span class="sxs-lookup"><span data-stu-id="79d2f-241">String</span></span>|<span data-ttu-id="79d2f-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="79d2f-244">响应</span><span class="sxs-lookup"><span data-stu-id="79d2f-244">Response</span></span>

<span data-ttu-id="79d2f-245">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79d2f-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79d2f-246">示例</span><span class="sxs-lookup"><span data-stu-id="79d2f-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79d2f-247">请求</span><span class="sxs-lookup"><span data-stu-id="79d2f-247">Request</span></span>
<span data-ttu-id="79d2f-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79d2f-248">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79d2f-249">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="79d2f-249">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79d2f-250">C#</span><span class="sxs-lookup"><span data-stu-id="79d2f-250">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79d2f-251">Javascript</span><span class="sxs-lookup"><span data-stu-id="79d2f-251">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79d2f-252">目标-C</span><span class="sxs-lookup"><span data-stu-id="79d2f-252">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79d2f-253">Java</span><span class="sxs-lookup"><span data-stu-id="79d2f-253">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79d2f-254">响应</span><span class="sxs-lookup"><span data-stu-id="79d2f-254">Response</span></span>
<span data-ttu-id="79d2f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79d2f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
