---
title: 更新联系人
description: 更新 contact 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3108edc3db30865cfd9541c053dbe1ea5105dd63
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047110"
---
# <a name="update-contact"></a><span data-ttu-id="82cd8-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="82cd8-103">Update contact</span></span>

<span data-ttu-id="82cd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82cd8-105">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82cd8-105">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="82cd8-106">权限</span><span class="sxs-lookup"><span data-stu-id="82cd8-106">Permissions</span></span>
<span data-ttu-id="82cd8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82cd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cd8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82cd8-109">Permission type</span></span>      | <span data-ttu-id="82cd8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82cd8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82cd8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82cd8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="82cd8-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82cd8-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="82cd8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82cd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82cd8-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82cd8-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="82cd8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82cd8-115">Application</span></span> | <span data-ttu-id="82cd8-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82cd8-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="82cd8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82cd8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="82cd8-118">[用户](../resources/contact.md)的默认[contactFolder 中的联系人](../resources/contactfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="82cd8-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="82cd8-119">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="82cd8-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="82cd8-120">[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="82cd8-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="82cd8-121">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="82cd8-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="82cd8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="82cd8-122">Request headers</span></span>
| <span data-ttu-id="82cd8-123">标头</span><span class="sxs-lookup"><span data-stu-id="82cd8-123">Header</span></span>       | <span data-ttu-id="82cd8-124">值</span><span class="sxs-lookup"><span data-stu-id="82cd8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82cd8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="82cd8-125">Authorization</span></span>  | <span data-ttu-id="82cd8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82cd8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82cd8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82cd8-128">Content-Type</span></span>  | <span data-ttu-id="82cd8-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="82cd8-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82cd8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="82cd8-131">Request body</span></span>
<span data-ttu-id="82cd8-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="82cd8-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="82cd8-135">属性</span><span class="sxs-lookup"><span data-stu-id="82cd8-135">Property</span></span>     | <span data-ttu-id="82cd8-136">类型</span><span class="sxs-lookup"><span data-stu-id="82cd8-136">Type</span></span>   |<span data-ttu-id="82cd8-137">说明</span><span class="sxs-lookup"><span data-stu-id="82cd8-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82cd8-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="82cd8-138">assistantName</span></span>|<span data-ttu-id="82cd8-139">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-139">String</span></span>|<span data-ttu-id="82cd8-140">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="82cd8-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="82cd8-141">birthday</span><span class="sxs-lookup"><span data-stu-id="82cd8-141">birthday</span></span>|<span data-ttu-id="82cd8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82cd8-142">DateTimeOffset</span></span>|<span data-ttu-id="82cd8-143">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="82cd8-143">The contact's birthday.</span></span>|
|<span data-ttu-id="82cd8-144">categories</span><span class="sxs-lookup"><span data-stu-id="82cd8-144">categories</span></span>|<span data-ttu-id="82cd8-145">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-145">String</span></span>|<span data-ttu-id="82cd8-146">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="82cd8-146">The categories associated with the contact.</span></span>|
|<span data-ttu-id="82cd8-147">children</span><span class="sxs-lookup"><span data-stu-id="82cd8-147">children</span></span>|<span data-ttu-id="82cd8-148">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-148">String</span></span>||
|<span data-ttu-id="82cd8-149">companyName</span><span class="sxs-lookup"><span data-stu-id="82cd8-149">companyName</span></span>|<span data-ttu-id="82cd8-150">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-150">String</span></span>|<span data-ttu-id="82cd8-151">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="82cd8-151">The name of the contact's company.</span></span>|
|<span data-ttu-id="82cd8-152">department</span><span class="sxs-lookup"><span data-stu-id="82cd8-152">department</span></span>|<span data-ttu-id="82cd8-153">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-153">String</span></span>|<span data-ttu-id="82cd8-154">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="82cd8-154">The contact's department.</span></span>|
|<span data-ttu-id="82cd8-155">displayName</span><span class="sxs-lookup"><span data-stu-id="82cd8-155">displayName</span></span>|<span data-ttu-id="82cd8-156">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-156">String</span></span>|<span data-ttu-id="82cd8-157">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="82cd8-157">The contact's display name.</span></span> <span data-ttu-id="82cd8-158">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="82cd8-158">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="82cd8-159">若要保留预先存在的值，请始终在更新操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="82cd8-159">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="82cd8-160">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="82cd8-160">emailAddresses</span></span>|<span data-ttu-id="82cd8-161">[typedEmailAddress](../resources/typedemailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82cd8-161">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="82cd8-162">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="82cd8-162">The contact's email addresses.</span></span>|
|<span data-ttu-id="82cd8-163">fileAs</span><span class="sxs-lookup"><span data-stu-id="82cd8-163">fileAs</span></span>|<span data-ttu-id="82cd8-164">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-164">String</span></span>|<span data-ttu-id="82cd8-165">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="82cd8-165">The name the contact is filed under.</span></span>|
|<span data-ttu-id="82cd8-166">gender</span><span class="sxs-lookup"><span data-stu-id="82cd8-166">gender</span></span> |<span data-ttu-id="82cd8-167">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-167">String</span></span> |<span data-ttu-id="82cd8-168">联系人的性别。</span><span class="sxs-lookup"><span data-stu-id="82cd8-168">The contact's gender.</span></span> |
|<span data-ttu-id="82cd8-169">generation</span><span class="sxs-lookup"><span data-stu-id="82cd8-169">generation</span></span>|<span data-ttu-id="82cd8-170">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-170">String</span></span>|<span data-ttu-id="82cd8-171">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="82cd8-171">The contact's generation.</span></span>|
|<span data-ttu-id="82cd8-172">givenName</span><span class="sxs-lookup"><span data-stu-id="82cd8-172">givenName</span></span>|<span data-ttu-id="82cd8-173">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-173">String</span></span>|<span data-ttu-id="82cd8-174">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="82cd8-174">The contact's given name.</span></span>|
|<span data-ttu-id="82cd8-175">imAddresses</span><span class="sxs-lookup"><span data-stu-id="82cd8-175">imAddresses</span></span>|<span data-ttu-id="82cd8-176">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-176">String</span></span>|<span data-ttu-id="82cd8-177">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="82cd8-177">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="82cd8-178">initials</span><span class="sxs-lookup"><span data-stu-id="82cd8-178">initials</span></span>|<span data-ttu-id="82cd8-179">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-179">String</span></span>|<span data-ttu-id="82cd8-180">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="82cd8-180">The contact's initials.</span></span>|
|<span data-ttu-id="82cd8-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="82cd8-181">jobTitle</span></span>|<span data-ttu-id="82cd8-182">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-182">String</span></span>|<span data-ttu-id="82cd8-183">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="82cd8-183">The contact’s job title.</span></span>|
|<span data-ttu-id="82cd8-184">manager</span><span class="sxs-lookup"><span data-stu-id="82cd8-184">manager</span></span>|<span data-ttu-id="82cd8-185">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-185">String</span></span>|<span data-ttu-id="82cd8-186">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="82cd8-186">The name of the contact's manager.</span></span>
|<span data-ttu-id="82cd8-187">middleName</span><span class="sxs-lookup"><span data-stu-id="82cd8-187">middleName</span></span>|<span data-ttu-id="82cd8-188">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-188">String</span></span>|<span data-ttu-id="82cd8-189">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="82cd8-189">The contact's middle name.</span></span>|
|<span data-ttu-id="82cd8-190">nickName</span><span class="sxs-lookup"><span data-stu-id="82cd8-190">nickName</span></span>|<span data-ttu-id="82cd8-191">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-191">String</span></span>|<span data-ttu-id="82cd8-192">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="82cd8-192">The contact's nickname.</span></span>|
|<span data-ttu-id="82cd8-193">officeLocation</span><span class="sxs-lookup"><span data-stu-id="82cd8-193">officeLocation</span></span>|<span data-ttu-id="82cd8-194">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-194">String</span></span>|<span data-ttu-id="82cd8-195">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="82cd8-195">The location of the contact's office.</span></span>|
|<span data-ttu-id="82cd8-196">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="82cd8-196">parentFolderId</span></span>|<span data-ttu-id="82cd8-197">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-197">String</span></span>|<span data-ttu-id="82cd8-198">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="82cd8-198">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="82cd8-199">personalNotes</span><span class="sxs-lookup"><span data-stu-id="82cd8-199">personalNotes</span></span>|<span data-ttu-id="82cd8-200">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-200">String</span></span>|<span data-ttu-id="82cd8-201">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="82cd8-201">The user's notes about the contact.</span></span>|
|<span data-ttu-id="82cd8-202">phones</span><span class="sxs-lookup"><span data-stu-id="82cd8-202">phones</span></span> |<span data-ttu-id="82cd8-203">[phone](../resources/phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="82cd8-203">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="82cd8-204">电话联系人关联的电话号码，例如住宅电话、移动电话和业务电话。</span><span class="sxs-lookup"><span data-stu-id="82cd8-204">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="82cd8-205">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="82cd8-205">postalAddresses</span></span> |<span data-ttu-id="82cd8-206">[physicalAddress](../resources/physicaladdress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82cd8-206">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="82cd8-207">与联系人关联的地址，例如，住宅地址和公司地址。</span><span class="sxs-lookup"><span data-stu-id="82cd8-207">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="82cd8-208">profession</span><span class="sxs-lookup"><span data-stu-id="82cd8-208">profession</span></span>|<span data-ttu-id="82cd8-209">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-209">String</span></span>|<span data-ttu-id="82cd8-210">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="82cd8-210">The contact's profession.</span></span>|
|<span data-ttu-id="82cd8-211">spouseName</span><span class="sxs-lookup"><span data-stu-id="82cd8-211">spouseName</span></span>|<span data-ttu-id="82cd8-212">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-212">String</span></span>|<span data-ttu-id="82cd8-213">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="82cd8-213">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="82cd8-214">surname</span><span class="sxs-lookup"><span data-stu-id="82cd8-214">surname</span></span>|<span data-ttu-id="82cd8-215">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-215">String</span></span>|<span data-ttu-id="82cd8-216">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="82cd8-216">The contact's surname.</span></span>|
|<span data-ttu-id="82cd8-217">title</span><span class="sxs-lookup"><span data-stu-id="82cd8-217">title</span></span>|<span data-ttu-id="82cd8-218">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-218">String</span></span>|<span data-ttu-id="82cd8-219">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="82cd8-219">The contact's title.</span></span>|
|<span data-ttu-id="82cd8-220">websites</span><span class="sxs-lookup"><span data-stu-id="82cd8-220">websites</span></span> |<span data-ttu-id="82cd8-221">[website](../resources/website.md) collection</span><span class="sxs-lookup"><span data-stu-id="82cd8-221">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="82cd8-222">与联系人关联的网站。</span><span class="sxs-lookup"><span data-stu-id="82cd8-222">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="82cd8-223">将anniversary</span><span class="sxs-lookup"><span data-stu-id="82cd8-223">weddingAnniversary</span></span> |<span data-ttu-id="82cd8-224">日期</span><span class="sxs-lookup"><span data-stu-id="82cd8-224">Date</span></span> |<span data-ttu-id="82cd8-225">联系人的周年日。</span><span class="sxs-lookup"><span data-stu-id="82cd8-225">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="82cd8-226">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="82cd8-226">yomiCompanyName</span></span>|<span data-ttu-id="82cd8-227">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-227">String</span></span>|<span data-ttu-id="82cd8-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="82cd8-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="82cd8-230">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="82cd8-230">yomiGivenName</span></span>|<span data-ttu-id="82cd8-231">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-231">String</span></span>|<span data-ttu-id="82cd8-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="82cd8-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="82cd8-234">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="82cd8-234">yomiSurname</span></span>|<span data-ttu-id="82cd8-235">String</span><span class="sxs-lookup"><span data-stu-id="82cd8-235">String</span></span>|<span data-ttu-id="82cd8-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="82cd8-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="82cd8-238">由于 **联系人** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作在现有联系人实例的扩展的自定义属性中添加、更新或删除你自己的特定于 `PATCH` **应用** 的数据。</span><span class="sxs-lookup"><span data-stu-id="82cd8-238">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="82cd8-239">响应</span><span class="sxs-lookup"><span data-stu-id="82cd8-239">Response</span></span>

<span data-ttu-id="82cd8-240">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/contact.md)代码和更新的 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="82cd8-240">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82cd8-241">示例</span><span class="sxs-lookup"><span data-stu-id="82cd8-241">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82cd8-242">请求</span><span class="sxs-lookup"><span data-stu-id="82cd8-242">Request</span></span>
<span data-ttu-id="82cd8-243">以下示例更新指定联系人的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="82cd8-243">The following example updates the personal email address of the specified contact.</span></span>

# <a name="http"></a>[<span data-ttu-id="82cd8-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="82cd8-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82cd8-245">C#</span><span class="sxs-lookup"><span data-stu-id="82cd8-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82cd8-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82cd8-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82cd8-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82cd8-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82cd8-248">Java</span><span class="sxs-lookup"><span data-stu-id="82cd8-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82cd8-249">响应</span><span class="sxs-lookup"><span data-stu-id="82cd8-249">Response</span></span>
<span data-ttu-id="82cd8-250">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="82cd8-250">Here is an example of the response.</span></span> <span data-ttu-id="82cd8-251">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82cd8-251">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="82cd8-252">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82cd8-252">See also</span></span>

- [<span data-ttu-id="82cd8-253">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="82cd8-253">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="82cd8-254">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="82cd8-254">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


