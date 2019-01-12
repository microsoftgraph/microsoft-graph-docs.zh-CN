---
title: 更新联系人
description: 更新 contact 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 381aa191639e32677d4fccbf9e9f48c99f3d988f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927903"
---
# <a name="update-contact"></a><span data-ttu-id="c6bbf-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="c6bbf-103">Update contact</span></span>

<span data-ttu-id="c6bbf-104">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6bbf-105">权限</span><span class="sxs-lookup"><span data-stu-id="c6bbf-105">Permissions</span></span>
<span data-ttu-id="c6bbf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6bbf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6bbf-108">Permission type</span></span>      | <span data-ttu-id="c6bbf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6bbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6bbf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6bbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6bbf-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6bbf-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c6bbf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6bbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6bbf-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6bbf-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c6bbf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6bbf-114">Application</span></span> | <span data-ttu-id="c6bbf-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6bbf-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6bbf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6bbf-116">HTTP request</span></span>
<span data-ttu-id="c6bbf-117"><!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)从用户的默认[contactFolder](../resources/contactfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="c6bbf-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="c6bbf-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c6bbf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6bbf-121">Request headers</span></span>
| <span data-ttu-id="c6bbf-122">标头</span><span class="sxs-lookup"><span data-stu-id="c6bbf-122">Header</span></span>       | <span data-ttu-id="c6bbf-123">值</span><span class="sxs-lookup"><span data-stu-id="c6bbf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6bbf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6bbf-124">Authorization</span></span>  | <span data-ttu-id="c6bbf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6bbf-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6bbf-127">Content-Type</span></span>  | <span data-ttu-id="c6bbf-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6bbf-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6bbf-130">Request body</span></span>
<span data-ttu-id="c6bbf-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c6bbf-134">属性</span><span class="sxs-lookup"><span data-stu-id="c6bbf-134">Property</span></span>     | <span data-ttu-id="c6bbf-135">类型</span><span class="sxs-lookup"><span data-stu-id="c6bbf-135">Type</span></span>   |<span data-ttu-id="c6bbf-136">说明</span><span class="sxs-lookup"><span data-stu-id="c6bbf-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6bbf-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-137">assistantName</span></span>|<span data-ttu-id="c6bbf-138">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-138">String</span></span>|<span data-ttu-id="c6bbf-139">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="c6bbf-140">birthday</span><span class="sxs-lookup"><span data-stu-id="c6bbf-140">birthday</span></span>|<span data-ttu-id="c6bbf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6bbf-141">DateTimeOffset</span></span>|<span data-ttu-id="c6bbf-142">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-142">The contact's birthday.</span></span>|
|<span data-ttu-id="c6bbf-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="c6bbf-143">businessAddress</span></span>|[<span data-ttu-id="c6bbf-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6bbf-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c6bbf-145">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-145">The contact's business address.</span></span>|
|<span data-ttu-id="c6bbf-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="c6bbf-146">businessHomePage</span></span>|<span data-ttu-id="c6bbf-147">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-147">String</span></span>|<span data-ttu-id="c6bbf-148">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="c6bbf-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="c6bbf-149">businessPhones</span></span>|<span data-ttu-id="c6bbf-150">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-150">String</span></span>|<span data-ttu-id="c6bbf-151">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="c6bbf-152">categories</span><span class="sxs-lookup"><span data-stu-id="c6bbf-152">categories</span></span>|<span data-ttu-id="c6bbf-153">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-153">String</span></span>|<span data-ttu-id="c6bbf-154">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="c6bbf-155">children</span><span class="sxs-lookup"><span data-stu-id="c6bbf-155">children</span></span>|<span data-ttu-id="c6bbf-156">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-156">String</span></span>|<span data-ttu-id="c6bbf-157">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="c6bbf-158">companyName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-158">companyName</span></span>|<span data-ttu-id="c6bbf-159">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-159">String</span></span>|<span data-ttu-id="c6bbf-160">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="c6bbf-161">department</span><span class="sxs-lookup"><span data-stu-id="c6bbf-161">department</span></span>|<span data-ttu-id="c6bbf-162">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-162">String</span></span>|<span data-ttu-id="c6bbf-163">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-163">The contact's department.</span></span>|
|<span data-ttu-id="c6bbf-164">displayName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-164">displayName</span></span>|<span data-ttu-id="c6bbf-165">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-165">String</span></span>|<span data-ttu-id="c6bbf-166">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-166">The contact's display name.</span></span> <span data-ttu-id="c6bbf-167">请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="c6bbf-168">若要保留现有的值，始终为在更新操作的 displayName 包括它。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="c6bbf-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="c6bbf-169">emailAddresses</span></span>|<span data-ttu-id="c6bbf-170">[EmailAddress](../resources/emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6bbf-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="c6bbf-171">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="c6bbf-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="c6bbf-172">fileAs</span></span>|<span data-ttu-id="c6bbf-173">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-173">String</span></span>|<span data-ttu-id="c6bbf-174">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="c6bbf-175">generation</span><span class="sxs-lookup"><span data-stu-id="c6bbf-175">generation</span></span>|<span data-ttu-id="c6bbf-176">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-176">String</span></span>|<span data-ttu-id="c6bbf-177">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-177">The contact's generation.</span></span>|
|<span data-ttu-id="c6bbf-178">givenName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-178">givenName</span></span>|<span data-ttu-id="c6bbf-179">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-179">String</span></span>|<span data-ttu-id="c6bbf-180">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-180">The contact's given name.</span></span>|
|<span data-ttu-id="c6bbf-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="c6bbf-181">homeAddress</span></span>|[<span data-ttu-id="c6bbf-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6bbf-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c6bbf-183">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-183">The contact's home address.</span></span>|
|<span data-ttu-id="c6bbf-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="c6bbf-184">homePhones</span></span>|<span data-ttu-id="c6bbf-185">String collection</span><span class="sxs-lookup"><span data-stu-id="c6bbf-185">String collection</span></span>|<span data-ttu-id="c6bbf-186">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="c6bbf-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="c6bbf-187">imAddresses</span></span>|<span data-ttu-id="c6bbf-188">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-188">String</span></span>|<span data-ttu-id="c6bbf-189">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="c6bbf-190">initials</span><span class="sxs-lookup"><span data-stu-id="c6bbf-190">initials</span></span>|<span data-ttu-id="c6bbf-191">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-191">String</span></span>|<span data-ttu-id="c6bbf-192">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-192">The contact's initials.</span></span>|
|<span data-ttu-id="c6bbf-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c6bbf-193">jobTitle</span></span>|<span data-ttu-id="c6bbf-194">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-194">String</span></span>|<span data-ttu-id="c6bbf-195">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-195">The contact’s job title.</span></span>|
|<span data-ttu-id="c6bbf-196">manager</span><span class="sxs-lookup"><span data-stu-id="c6bbf-196">manager</span></span>|<span data-ttu-id="c6bbf-197">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-197">String</span></span>|<span data-ttu-id="c6bbf-198">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="c6bbf-199">middleName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-199">middleName</span></span>|<span data-ttu-id="c6bbf-200">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-200">String</span></span>|<span data-ttu-id="c6bbf-201">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-201">The contact's middle name.</span></span>|
|<span data-ttu-id="c6bbf-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c6bbf-202">mobilePhone</span></span>|<span data-ttu-id="c6bbf-203">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-203">String</span></span>|<span data-ttu-id="c6bbf-204">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="c6bbf-205">nickName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-205">nickName</span></span>|<span data-ttu-id="c6bbf-206">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-206">String</span></span>|<span data-ttu-id="c6bbf-207">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-207">The contact's nickname.</span></span>|
|<span data-ttu-id="c6bbf-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c6bbf-208">officeLocation</span></span>|<span data-ttu-id="c6bbf-209">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-209">String</span></span>|<span data-ttu-id="c6bbf-210">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="c6bbf-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="c6bbf-211">otherAddress</span></span>|[<span data-ttu-id="c6bbf-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6bbf-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c6bbf-213">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="c6bbf-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c6bbf-214">parentFolderId</span></span>|<span data-ttu-id="c6bbf-215">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-215">String</span></span>|<span data-ttu-id="c6bbf-216">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="c6bbf-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="c6bbf-217">personalNotes</span></span>|<span data-ttu-id="c6bbf-218">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-218">String</span></span>|<span data-ttu-id="c6bbf-219">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="c6bbf-220">profession</span><span class="sxs-lookup"><span data-stu-id="c6bbf-220">profession</span></span>|<span data-ttu-id="c6bbf-221">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-221">String</span></span>|<span data-ttu-id="c6bbf-222">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-222">The contact's profession.</span></span>|
|<span data-ttu-id="c6bbf-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-223">spouseName</span></span>|<span data-ttu-id="c6bbf-224">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-224">String</span></span>|<span data-ttu-id="c6bbf-225">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="c6bbf-226">surname</span><span class="sxs-lookup"><span data-stu-id="c6bbf-226">surname</span></span>|<span data-ttu-id="c6bbf-227">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-227">String</span></span>|<span data-ttu-id="c6bbf-228">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-228">The contact's surname.</span></span>|
|<span data-ttu-id="c6bbf-229">title</span><span class="sxs-lookup"><span data-stu-id="c6bbf-229">title</span></span>|<span data-ttu-id="c6bbf-230">String</span><span class="sxs-lookup"><span data-stu-id="c6bbf-230">String</span></span>|<span data-ttu-id="c6bbf-231">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-231">The contact's title.</span></span>|
|<span data-ttu-id="c6bbf-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-232">yomiCompanyName</span></span>|<span data-ttu-id="c6bbf-233">字符串</span><span class="sxs-lookup"><span data-stu-id="c6bbf-233">String</span></span>|<span data-ttu-id="c6bbf-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="c6bbf-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="c6bbf-236">yomiGivenName</span></span>|<span data-ttu-id="c6bbf-237">字符串</span><span class="sxs-lookup"><span data-stu-id="c6bbf-237">String</span></span>|<span data-ttu-id="c6bbf-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="c6bbf-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="c6bbf-240">yomiSurname</span></span>|<span data-ttu-id="c6bbf-241">字符串</span><span class="sxs-lookup"><span data-stu-id="c6bbf-241">String</span></span>|<span data-ttu-id="c6bbf-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="c6bbf-244">响应</span><span class="sxs-lookup"><span data-stu-id="c6bbf-244">Response</span></span>

<span data-ttu-id="c6bbf-245">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6bbf-246">示例</span><span class="sxs-lookup"><span data-stu-id="c6bbf-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6bbf-247">请求</span><span class="sxs-lookup"><span data-stu-id="c6bbf-247">Request</span></span>
<span data-ttu-id="c6bbf-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-248">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c6bbf-249">响应</span><span class="sxs-lookup"><span data-stu-id="c6bbf-249">Response</span></span>
<span data-ttu-id="c6bbf-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6bbf-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
