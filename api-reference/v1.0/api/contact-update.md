---
title: 更新联系人
description: 更新 contact 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 51231bdca731fb1636a3b52cdc1a27b36a21c28b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048797"
---
# <a name="update-contact"></a><span data-ttu-id="1a61f-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="1a61f-103">Update contact</span></span>

<span data-ttu-id="1a61f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a61f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a61f-105">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a61f-105">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a61f-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a61f-106">Permissions</span></span>
<span data-ttu-id="1a61f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a61f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a61f-109">Permission type</span></span>      | <span data-ttu-id="1a61f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a61f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a61f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a61f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1a61f-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a61f-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1a61f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a61f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a61f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a61f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1a61f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a61f-115">Application</span></span> | <span data-ttu-id="1a61f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a61f-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a61f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a61f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1a61f-118">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="1a61f-118">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="1a61f-119">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="1a61f-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="1a61f-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1a61f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a61f-122">Request headers</span></span>
| <span data-ttu-id="1a61f-123">标头</span><span class="sxs-lookup"><span data-stu-id="1a61f-123">Header</span></span>       | <span data-ttu-id="1a61f-124">值</span><span class="sxs-lookup"><span data-stu-id="1a61f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a61f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a61f-125">Authorization</span></span>  | <span data-ttu-id="1a61f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1a61f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a61f-128">Content-Type</span></span>  | <span data-ttu-id="1a61f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1a61f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a61f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a61f-131">Request body</span></span>
<span data-ttu-id="1a61f-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1a61f-135">属性</span><span class="sxs-lookup"><span data-stu-id="1a61f-135">Property</span></span>     | <span data-ttu-id="1a61f-136">类型</span><span class="sxs-lookup"><span data-stu-id="1a61f-136">Type</span></span>   |<span data-ttu-id="1a61f-137">说明</span><span class="sxs-lookup"><span data-stu-id="1a61f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a61f-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="1a61f-138">assistantName</span></span>|<span data-ttu-id="1a61f-139">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-139">String</span></span>|<span data-ttu-id="1a61f-140">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="1a61f-141">birthday</span><span class="sxs-lookup"><span data-stu-id="1a61f-141">birthday</span></span>|<span data-ttu-id="1a61f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a61f-142">DateTimeOffset</span></span>|<span data-ttu-id="1a61f-143">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="1a61f-143">The contact's birthday.</span></span>|
|<span data-ttu-id="1a61f-144">businessAddress</span><span class="sxs-lookup"><span data-stu-id="1a61f-144">businessAddress</span></span>|[<span data-ttu-id="1a61f-145">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="1a61f-145">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="1a61f-146">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="1a61f-146">The contact's business address.</span></span>|
|<span data-ttu-id="1a61f-147">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="1a61f-147">businessHomePage</span></span>|<span data-ttu-id="1a61f-148">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-148">String</span></span>|<span data-ttu-id="1a61f-149">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="1a61f-149">The business home page of the contact.</span></span>|
|<span data-ttu-id="1a61f-150">businessPhones</span><span class="sxs-lookup"><span data-stu-id="1a61f-150">businessPhones</span></span>|<span data-ttu-id="1a61f-151">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-151">String</span></span>|<span data-ttu-id="1a61f-152">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="1a61f-152">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="1a61f-153">categories</span><span class="sxs-lookup"><span data-stu-id="1a61f-153">categories</span></span>|<span data-ttu-id="1a61f-154">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-154">String</span></span>|<span data-ttu-id="1a61f-155">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="1a61f-155">The categories associated with the contact.</span></span>|
|<span data-ttu-id="1a61f-156">children</span><span class="sxs-lookup"><span data-stu-id="1a61f-156">children</span></span>|<span data-ttu-id="1a61f-157">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-157">String</span></span>|<span data-ttu-id="1a61f-158">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-158">The names of the contact's children.</span></span>|
|<span data-ttu-id="1a61f-159">companyName</span><span class="sxs-lookup"><span data-stu-id="1a61f-159">companyName</span></span>|<span data-ttu-id="1a61f-160">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-160">String</span></span>|<span data-ttu-id="1a61f-161">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="1a61f-161">The name of the contact's company.</span></span>|
|<span data-ttu-id="1a61f-162">department</span><span class="sxs-lookup"><span data-stu-id="1a61f-162">department</span></span>|<span data-ttu-id="1a61f-163">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-163">String</span></span>|<span data-ttu-id="1a61f-164">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="1a61f-164">The contact's department.</span></span>|
|<span data-ttu-id="1a61f-165">displayName</span><span class="sxs-lookup"><span data-stu-id="1a61f-165">displayName</span></span>|<span data-ttu-id="1a61f-166">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-166">String</span></span>|<span data-ttu-id="1a61f-167">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1a61f-167">The contact's display name.</span></span> <span data-ttu-id="1a61f-168">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="1a61f-168">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="1a61f-169">若要保留预先存在的值，请始终在更新操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="1a61f-169">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="1a61f-170">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="1a61f-170">emailAddresses</span></span>|<span data-ttu-id="1a61f-171">[EmailAddress](../resources/emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a61f-171">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="1a61f-172">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1a61f-172">The contact's email addresses.</span></span>|
|<span data-ttu-id="1a61f-173">fileAs</span><span class="sxs-lookup"><span data-stu-id="1a61f-173">fileAs</span></span>|<span data-ttu-id="1a61f-174">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-174">String</span></span>|<span data-ttu-id="1a61f-175">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-175">The name the contact is filed under.</span></span>|
|<span data-ttu-id="1a61f-176">generation</span><span class="sxs-lookup"><span data-stu-id="1a61f-176">generation</span></span>|<span data-ttu-id="1a61f-177">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-177">String</span></span>|<span data-ttu-id="1a61f-178">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="1a61f-178">The contact's generation.</span></span>|
|<span data-ttu-id="1a61f-179">givenName</span><span class="sxs-lookup"><span data-stu-id="1a61f-179">givenName</span></span>|<span data-ttu-id="1a61f-180">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-180">String</span></span>|<span data-ttu-id="1a61f-181">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-181">The contact's given name.</span></span>|
|<span data-ttu-id="1a61f-182">homeAddress</span><span class="sxs-lookup"><span data-stu-id="1a61f-182">homeAddress</span></span>|[<span data-ttu-id="1a61f-183">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="1a61f-183">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="1a61f-184">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="1a61f-184">The contact's home address.</span></span>|
|<span data-ttu-id="1a61f-185">homePhones</span><span class="sxs-lookup"><span data-stu-id="1a61f-185">homePhones</span></span>|<span data-ttu-id="1a61f-186">String collection</span><span class="sxs-lookup"><span data-stu-id="1a61f-186">String collection</span></span>|<span data-ttu-id="1a61f-187">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="1a61f-187">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="1a61f-188">imAddresses</span><span class="sxs-lookup"><span data-stu-id="1a61f-188">imAddresses</span></span>|<span data-ttu-id="1a61f-189">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-189">String</span></span>|<span data-ttu-id="1a61f-190">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="1a61f-190">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="1a61f-191">initials</span><span class="sxs-lookup"><span data-stu-id="1a61f-191">initials</span></span>|<span data-ttu-id="1a61f-192">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-192">String</span></span>|<span data-ttu-id="1a61f-193">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="1a61f-193">The contact's initials.</span></span>|
|<span data-ttu-id="1a61f-194">jobTitle</span><span class="sxs-lookup"><span data-stu-id="1a61f-194">jobTitle</span></span>|<span data-ttu-id="1a61f-195">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-195">String</span></span>|<span data-ttu-id="1a61f-196">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="1a61f-196">The contact’s job title.</span></span>|
|<span data-ttu-id="1a61f-197">manager</span><span class="sxs-lookup"><span data-stu-id="1a61f-197">manager</span></span>|<span data-ttu-id="1a61f-198">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-198">String</span></span>|<span data-ttu-id="1a61f-199">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-199">The name of the contact's manager.</span></span>
|<span data-ttu-id="1a61f-200">middleName</span><span class="sxs-lookup"><span data-stu-id="1a61f-200">middleName</span></span>|<span data-ttu-id="1a61f-201">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-201">String</span></span>|<span data-ttu-id="1a61f-202">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-202">The contact's middle name.</span></span>|
|<span data-ttu-id="1a61f-203">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="1a61f-203">mobilePhone</span></span>|<span data-ttu-id="1a61f-204">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-204">String</span></span>|<span data-ttu-id="1a61f-205">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="1a61f-205">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="1a61f-206">nickName</span><span class="sxs-lookup"><span data-stu-id="1a61f-206">nickName</span></span>|<span data-ttu-id="1a61f-207">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-207">String</span></span>|<span data-ttu-id="1a61f-208">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="1a61f-208">The contact's nickname.</span></span>|
|<span data-ttu-id="1a61f-209">officeLocation</span><span class="sxs-lookup"><span data-stu-id="1a61f-209">officeLocation</span></span>|<span data-ttu-id="1a61f-210">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-210">String</span></span>|<span data-ttu-id="1a61f-211">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="1a61f-211">The location of the contact's office.</span></span>|
|<span data-ttu-id="1a61f-212">otherAddress</span><span class="sxs-lookup"><span data-stu-id="1a61f-212">otherAddress</span></span>|[<span data-ttu-id="1a61f-213">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="1a61f-213">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="1a61f-214">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="1a61f-214">Other addresses for the contact.</span></span>|
|<span data-ttu-id="1a61f-215">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="1a61f-215">parentFolderId</span></span>|<span data-ttu-id="1a61f-216">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-216">String</span></span>|<span data-ttu-id="1a61f-217">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="1a61f-217">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="1a61f-218">personalNotes</span><span class="sxs-lookup"><span data-stu-id="1a61f-218">personalNotes</span></span>|<span data-ttu-id="1a61f-219">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-219">String</span></span>|<span data-ttu-id="1a61f-220">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="1a61f-220">The user's notes about the contact.</span></span>|
|<span data-ttu-id="1a61f-221">profession</span><span class="sxs-lookup"><span data-stu-id="1a61f-221">profession</span></span>|<span data-ttu-id="1a61f-222">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-222">String</span></span>|<span data-ttu-id="1a61f-223">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="1a61f-223">The contact's profession.</span></span>|
|<span data-ttu-id="1a61f-224">spouseName</span><span class="sxs-lookup"><span data-stu-id="1a61f-224">spouseName</span></span>|<span data-ttu-id="1a61f-225">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-225">String</span></span>|<span data-ttu-id="1a61f-226">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="1a61f-226">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="1a61f-227">surname</span><span class="sxs-lookup"><span data-stu-id="1a61f-227">surname</span></span>|<span data-ttu-id="1a61f-228">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-228">String</span></span>|<span data-ttu-id="1a61f-229">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="1a61f-229">The contact's surname.</span></span>|
|<span data-ttu-id="1a61f-230">title</span><span class="sxs-lookup"><span data-stu-id="1a61f-230">title</span></span>|<span data-ttu-id="1a61f-231">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-231">String</span></span>|<span data-ttu-id="1a61f-232">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="1a61f-232">The contact's title.</span></span>|
|<span data-ttu-id="1a61f-233">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="1a61f-233">yomiCompanyName</span></span>|<span data-ttu-id="1a61f-234">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-234">String</span></span>|<span data-ttu-id="1a61f-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="1a61f-237">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="1a61f-237">yomiGivenName</span></span>|<span data-ttu-id="1a61f-238">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-238">String</span></span>|<span data-ttu-id="1a61f-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="1a61f-241">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="1a61f-241">yomiSurname</span></span>|<span data-ttu-id="1a61f-242">String</span><span class="sxs-lookup"><span data-stu-id="1a61f-242">String</span></span>|<span data-ttu-id="1a61f-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="1a61f-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="1a61f-245">响应</span><span class="sxs-lookup"><span data-stu-id="1a61f-245">Response</span></span>

<span data-ttu-id="1a61f-246">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a61f-246">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a61f-247">示例</span><span class="sxs-lookup"><span data-stu-id="1a61f-247">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a61f-248">请求</span><span class="sxs-lookup"><span data-stu-id="1a61f-248">Request</span></span>
<span data-ttu-id="1a61f-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a61f-249">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a61f-250">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a61f-250">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1a61f-251">C#</span><span class="sxs-lookup"><span data-stu-id="1a61f-251">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a61f-252">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a61f-252">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a61f-253">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a61f-253">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a61f-254">Java</span><span class="sxs-lookup"><span data-stu-id="1a61f-254">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a61f-255">响应</span><span class="sxs-lookup"><span data-stu-id="1a61f-255">Response</span></span>
<span data-ttu-id="1a61f-256">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a61f-256">Here is an example of the response.</span></span> <span data-ttu-id="1a61f-257">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1a61f-257">Note: The response object shown here might be shortened for readability.</span></span>
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

