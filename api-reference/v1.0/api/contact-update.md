---
title: 更新联系人
description: 更新 contact 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0d8a6d344326d1dfb03a23fc21e7e21680a827dd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277495"
---
# <a name="update-contact"></a><span data-ttu-id="79f6d-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="79f6d-103">Update contact</span></span>

<span data-ttu-id="79f6d-104">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="79f6d-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79f6d-105">权限</span><span class="sxs-lookup"><span data-stu-id="79f6d-105">Permissions</span></span>
<span data-ttu-id="79f6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79f6d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="79f6d-108">Permission type</span></span>      | <span data-ttu-id="79f6d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79f6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79f6d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79f6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79f6d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79f6d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="79f6d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79f6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f6d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79f6d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="79f6d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="79f6d-114">Application</span></span> | <span data-ttu-id="79f6d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79f6d-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79f6d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79f6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="79f6d-117">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="79f6d-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="79f6d-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="79f6d-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="79f6d-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79f6d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="79f6d-121">Request headers</span></span>
| <span data-ttu-id="79f6d-122">标头</span><span class="sxs-lookup"><span data-stu-id="79f6d-122">Header</span></span>       | <span data-ttu-id="79f6d-123">值</span><span class="sxs-lookup"><span data-stu-id="79f6d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79f6d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79f6d-124">Authorization</span></span>  | <span data-ttu-id="79f6d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79f6d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79f6d-127">Content-Type</span></span>  | <span data-ttu-id="79f6d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="79f6d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79f6d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="79f6d-130">Request body</span></span>
<span data-ttu-id="79f6d-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79f6d-134">属性</span><span class="sxs-lookup"><span data-stu-id="79f6d-134">Property</span></span>     | <span data-ttu-id="79f6d-135">类型</span><span class="sxs-lookup"><span data-stu-id="79f6d-135">Type</span></span>   |<span data-ttu-id="79f6d-136">说明</span><span class="sxs-lookup"><span data-stu-id="79f6d-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79f6d-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="79f6d-137">assistantName</span></span>|<span data-ttu-id="79f6d-138">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-138">String</span></span>|<span data-ttu-id="79f6d-139">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="79f6d-140">birthday</span><span class="sxs-lookup"><span data-stu-id="79f6d-140">birthday</span></span>|<span data-ttu-id="79f6d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79f6d-141">DateTimeOffset</span></span>|<span data-ttu-id="79f6d-142">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="79f6d-142">The contact's birthday.</span></span>|
|<span data-ttu-id="79f6d-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="79f6d-143">businessAddress</span></span>|[<span data-ttu-id="79f6d-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="79f6d-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="79f6d-145">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="79f6d-145">The contact's business address.</span></span>|
|<span data-ttu-id="79f6d-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="79f6d-146">businessHomePage</span></span>|<span data-ttu-id="79f6d-147">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-147">String</span></span>|<span data-ttu-id="79f6d-148">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="79f6d-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="79f6d-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="79f6d-149">businessPhones</span></span>|<span data-ttu-id="79f6d-150">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-150">String</span></span>|<span data-ttu-id="79f6d-151">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="79f6d-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="79f6d-152">categories</span><span class="sxs-lookup"><span data-stu-id="79f6d-152">categories</span></span>|<span data-ttu-id="79f6d-153">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-153">String</span></span>|<span data-ttu-id="79f6d-154">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="79f6d-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="79f6d-155">children</span><span class="sxs-lookup"><span data-stu-id="79f6d-155">children</span></span>|<span data-ttu-id="79f6d-156">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-156">String</span></span>|<span data-ttu-id="79f6d-157">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="79f6d-158">companyName</span><span class="sxs-lookup"><span data-stu-id="79f6d-158">companyName</span></span>|<span data-ttu-id="79f6d-159">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-159">String</span></span>|<span data-ttu-id="79f6d-160">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="79f6d-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="79f6d-161">department</span><span class="sxs-lookup"><span data-stu-id="79f6d-161">department</span></span>|<span data-ttu-id="79f6d-162">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-162">String</span></span>|<span data-ttu-id="79f6d-163">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="79f6d-163">The contact's department.</span></span>|
|<span data-ttu-id="79f6d-164">displayName</span><span class="sxs-lookup"><span data-stu-id="79f6d-164">displayName</span></span>|<span data-ttu-id="79f6d-165">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-165">String</span></span>|<span data-ttu-id="79f6d-166">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="79f6d-166">The contact's display name.</span></span> <span data-ttu-id="79f6d-167">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="79f6d-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="79f6d-168">若要保留预先存在的值，请始终在更新操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="79f6d-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="79f6d-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="79f6d-169">emailAddresses</span></span>|<span data-ttu-id="79f6d-170">[EmailAddress](../resources/emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79f6d-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="79f6d-171">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="79f6d-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="79f6d-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="79f6d-172">fileAs</span></span>|<span data-ttu-id="79f6d-173">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-173">String</span></span>|<span data-ttu-id="79f6d-174">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="79f6d-175">generation</span><span class="sxs-lookup"><span data-stu-id="79f6d-175">generation</span></span>|<span data-ttu-id="79f6d-176">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-176">String</span></span>|<span data-ttu-id="79f6d-177">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="79f6d-177">The contact's generation.</span></span>|
|<span data-ttu-id="79f6d-178">givenName</span><span class="sxs-lookup"><span data-stu-id="79f6d-178">givenName</span></span>|<span data-ttu-id="79f6d-179">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-179">String</span></span>|<span data-ttu-id="79f6d-180">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-180">The contact's given name.</span></span>|
|<span data-ttu-id="79f6d-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="79f6d-181">homeAddress</span></span>|[<span data-ttu-id="79f6d-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="79f6d-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="79f6d-183">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="79f6d-183">The contact's home address.</span></span>|
|<span data-ttu-id="79f6d-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="79f6d-184">homePhones</span></span>|<span data-ttu-id="79f6d-185">String collection</span><span class="sxs-lookup"><span data-stu-id="79f6d-185">String collection</span></span>|<span data-ttu-id="79f6d-186">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="79f6d-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="79f6d-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="79f6d-187">imAddresses</span></span>|<span data-ttu-id="79f6d-188">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-188">String</span></span>|<span data-ttu-id="79f6d-189">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="79f6d-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="79f6d-190">initials</span><span class="sxs-lookup"><span data-stu-id="79f6d-190">initials</span></span>|<span data-ttu-id="79f6d-191">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-191">String</span></span>|<span data-ttu-id="79f6d-192">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="79f6d-192">The contact's initials.</span></span>|
|<span data-ttu-id="79f6d-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="79f6d-193">jobTitle</span></span>|<span data-ttu-id="79f6d-194">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-194">String</span></span>|<span data-ttu-id="79f6d-195">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="79f6d-195">The contact’s job title.</span></span>|
|<span data-ttu-id="79f6d-196">manager</span><span class="sxs-lookup"><span data-stu-id="79f6d-196">manager</span></span>|<span data-ttu-id="79f6d-197">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-197">String</span></span>|<span data-ttu-id="79f6d-198">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="79f6d-199">middleName</span><span class="sxs-lookup"><span data-stu-id="79f6d-199">middleName</span></span>|<span data-ttu-id="79f6d-200">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-200">String</span></span>|<span data-ttu-id="79f6d-201">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-201">The contact's middle name.</span></span>|
|<span data-ttu-id="79f6d-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="79f6d-202">mobilePhone</span></span>|<span data-ttu-id="79f6d-203">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-203">String</span></span>|<span data-ttu-id="79f6d-204">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="79f6d-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="79f6d-205">nickName</span><span class="sxs-lookup"><span data-stu-id="79f6d-205">nickName</span></span>|<span data-ttu-id="79f6d-206">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-206">String</span></span>|<span data-ttu-id="79f6d-207">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="79f6d-207">The contact's nickname.</span></span>|
|<span data-ttu-id="79f6d-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="79f6d-208">officeLocation</span></span>|<span data-ttu-id="79f6d-209">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-209">String</span></span>|<span data-ttu-id="79f6d-210">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="79f6d-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="79f6d-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="79f6d-211">otherAddress</span></span>|[<span data-ttu-id="79f6d-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="79f6d-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="79f6d-213">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="79f6d-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="79f6d-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="79f6d-214">parentFolderId</span></span>|<span data-ttu-id="79f6d-215">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-215">String</span></span>|<span data-ttu-id="79f6d-216">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="79f6d-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="79f6d-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="79f6d-217">personalNotes</span></span>|<span data-ttu-id="79f6d-218">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-218">String</span></span>|<span data-ttu-id="79f6d-219">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="79f6d-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="79f6d-220">profession</span><span class="sxs-lookup"><span data-stu-id="79f6d-220">profession</span></span>|<span data-ttu-id="79f6d-221">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-221">String</span></span>|<span data-ttu-id="79f6d-222">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="79f6d-222">The contact's profession.</span></span>|
|<span data-ttu-id="79f6d-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="79f6d-223">spouseName</span></span>|<span data-ttu-id="79f6d-224">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-224">String</span></span>|<span data-ttu-id="79f6d-225">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="79f6d-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="79f6d-226">surname</span><span class="sxs-lookup"><span data-stu-id="79f6d-226">surname</span></span>|<span data-ttu-id="79f6d-227">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-227">String</span></span>|<span data-ttu-id="79f6d-228">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="79f6d-228">The contact's surname.</span></span>|
|<span data-ttu-id="79f6d-229">title</span><span class="sxs-lookup"><span data-stu-id="79f6d-229">title</span></span>|<span data-ttu-id="79f6d-230">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-230">String</span></span>|<span data-ttu-id="79f6d-231">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="79f6d-231">The contact's title.</span></span>|
|<span data-ttu-id="79f6d-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="79f6d-232">yomiCompanyName</span></span>|<span data-ttu-id="79f6d-233">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-233">String</span></span>|<span data-ttu-id="79f6d-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="79f6d-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="79f6d-236">yomiGivenName</span></span>|<span data-ttu-id="79f6d-237">字符串</span><span class="sxs-lookup"><span data-stu-id="79f6d-237">String</span></span>|<span data-ttu-id="79f6d-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="79f6d-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="79f6d-240">yomiSurname</span></span>|<span data-ttu-id="79f6d-241">String</span><span class="sxs-lookup"><span data-stu-id="79f6d-241">String</span></span>|<span data-ttu-id="79f6d-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="79f6d-244">响应</span><span class="sxs-lookup"><span data-stu-id="79f6d-244">Response</span></span>

<span data-ttu-id="79f6d-245">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79f6d-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79f6d-246">示例</span><span class="sxs-lookup"><span data-stu-id="79f6d-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79f6d-247">请求</span><span class="sxs-lookup"><span data-stu-id="79f6d-247">Request</span></span>
<span data-ttu-id="79f6d-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79f6d-248">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="79f6d-249">响应</span><span class="sxs-lookup"><span data-stu-id="79f6d-249">Response</span></span>
<span data-ttu-id="79f6d-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79f6d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="79f6d-253">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="79f6d-253">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="79f6d-254">C#</span><span class="sxs-lookup"><span data-stu-id="79f6d-254">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79f6d-255">Javascript</span><span class="sxs-lookup"><span data-stu-id="79f6d-255">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="79f6d-256">目标-C</span><span class="sxs-lookup"><span data-stu-id="79f6d-256">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_contact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contact-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
