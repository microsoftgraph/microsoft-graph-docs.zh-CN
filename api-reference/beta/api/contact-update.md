---
title: 更新联系人
description: 更新联系人对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c6ed3304b5f44a8bb1d35c1db491e8eaf7ae47b4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528205"
---
# <a name="update-contact"></a><span data-ttu-id="0e091-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="0e091-103">Update contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e091-104">更新联系人对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e091-104">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e091-105">权限</span><span class="sxs-lookup"><span data-stu-id="0e091-105">Permissions</span></span>
<span data-ttu-id="0e091-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e091-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e091-108">Permission type</span></span>      | <span data-ttu-id="0e091-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e091-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e091-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e091-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e091-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e091-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0e091-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e091-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e091-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e091-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0e091-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e091-114">Application</span></span> | <span data-ttu-id="0e091-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e091-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e091-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e091-116">HTTP request</span></span>
<span data-ttu-id="0e091-117"><!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)从用户的默认[contactFolder](../resources/contactfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="0e091-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="0e091-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0e091-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="0e091-119">[联系人](../resources/contact.md) [contactFolder](../resources/mailfolder.md)子文件夹中包含。</span><span class="sxs-lookup"><span data-stu-id="0e091-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="0e091-120">下面的示例演示一个级别的嵌套，但联系人可以位于子级的子级，依此类推。</span><span class="sxs-lookup"><span data-stu-id="0e091-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0e091-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e091-121">Request headers</span></span>
| <span data-ttu-id="0e091-122">标头</span><span class="sxs-lookup"><span data-stu-id="0e091-122">Header</span></span>       | <span data-ttu-id="0e091-123">值</span><span class="sxs-lookup"><span data-stu-id="0e091-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e091-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e091-124">Authorization</span></span>  | <span data-ttu-id="0e091-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e091-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0e091-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e091-127">Content-Type</span></span>  | <span data-ttu-id="0e091-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0e091-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e091-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e091-130">Request body</span></span>
<span data-ttu-id="0e091-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0e091-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e091-134">属性</span><span class="sxs-lookup"><span data-stu-id="0e091-134">Property</span></span>     | <span data-ttu-id="0e091-135">类型</span><span class="sxs-lookup"><span data-stu-id="0e091-135">Type</span></span>   |<span data-ttu-id="0e091-136">说明</span><span class="sxs-lookup"><span data-stu-id="0e091-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e091-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="0e091-137">assistantName</span></span>|<span data-ttu-id="0e091-138">String</span><span class="sxs-lookup"><span data-stu-id="0e091-138">String</span></span>|<span data-ttu-id="0e091-139">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="0e091-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="0e091-140">birthday</span><span class="sxs-lookup"><span data-stu-id="0e091-140">birthday</span></span>|<span data-ttu-id="0e091-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e091-141">DateTimeOffset</span></span>|<span data-ttu-id="0e091-142">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="0e091-142">The contact's birthday.</span></span>|
|<span data-ttu-id="0e091-143">categories</span><span class="sxs-lookup"><span data-stu-id="0e091-143">categories</span></span>|<span data-ttu-id="0e091-144">String</span><span class="sxs-lookup"><span data-stu-id="0e091-144">String</span></span>|<span data-ttu-id="0e091-145">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="0e091-145">The categories associated with the contact.</span></span>|
|<span data-ttu-id="0e091-146">children</span><span class="sxs-lookup"><span data-stu-id="0e091-146">children</span></span>|<span data-ttu-id="0e091-147">String</span><span class="sxs-lookup"><span data-stu-id="0e091-147">String</span></span>||
|<span data-ttu-id="0e091-148">companyName</span><span class="sxs-lookup"><span data-stu-id="0e091-148">companyName</span></span>|<span data-ttu-id="0e091-149">String</span><span class="sxs-lookup"><span data-stu-id="0e091-149">String</span></span>|<span data-ttu-id="0e091-150">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="0e091-150">The name of the contact's company.</span></span>|
|<span data-ttu-id="0e091-151">department</span><span class="sxs-lookup"><span data-stu-id="0e091-151">department</span></span>|<span data-ttu-id="0e091-152">String</span><span class="sxs-lookup"><span data-stu-id="0e091-152">String</span></span>|<span data-ttu-id="0e091-153">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="0e091-153">The contact's department.</span></span>|
|<span data-ttu-id="0e091-154">displayName</span><span class="sxs-lookup"><span data-stu-id="0e091-154">displayName</span></span>|<span data-ttu-id="0e091-155">String</span><span class="sxs-lookup"><span data-stu-id="0e091-155">String</span></span>|<span data-ttu-id="0e091-156">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e091-156">The contact's display name.</span></span> <span data-ttu-id="0e091-157">请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。</span><span class="sxs-lookup"><span data-stu-id="0e091-157">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="0e091-158">若要保留现有的值，始终为在更新操作的 displayName 包括它。</span><span class="sxs-lookup"><span data-stu-id="0e091-158">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="0e091-159">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="0e091-159">emailAddresses</span></span>|<span data-ttu-id="0e091-160">[typedEmailAddress](../resources/typedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e091-160">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="0e091-161">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0e091-161">The contact's email addresses.</span></span>|
|<span data-ttu-id="0e091-162">fileAs</span><span class="sxs-lookup"><span data-stu-id="0e091-162">fileAs</span></span>|<span data-ttu-id="0e091-163">String</span><span class="sxs-lookup"><span data-stu-id="0e091-163">String</span></span>|<span data-ttu-id="0e091-164">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="0e091-164">The name the contact is filed under.</span></span>|
|<span data-ttu-id="0e091-165">gender</span><span class="sxs-lookup"><span data-stu-id="0e091-165">gender</span></span> |<span data-ttu-id="0e091-166">String</span><span class="sxs-lookup"><span data-stu-id="0e091-166">String</span></span> |<span data-ttu-id="0e091-167">联系人的性别。</span><span class="sxs-lookup"><span data-stu-id="0e091-167">The contact's gender.</span></span> |
|<span data-ttu-id="0e091-168">generation</span><span class="sxs-lookup"><span data-stu-id="0e091-168">generation</span></span>|<span data-ttu-id="0e091-169">String</span><span class="sxs-lookup"><span data-stu-id="0e091-169">String</span></span>|<span data-ttu-id="0e091-170">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="0e091-170">The contact's generation.</span></span>|
|<span data-ttu-id="0e091-171">givenName</span><span class="sxs-lookup"><span data-stu-id="0e091-171">givenName</span></span>|<span data-ttu-id="0e091-172">String</span><span class="sxs-lookup"><span data-stu-id="0e091-172">String</span></span>|<span data-ttu-id="0e091-173">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="0e091-173">The contact's given name.</span></span>|
|<span data-ttu-id="0e091-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="0e091-174">imAddresses</span></span>|<span data-ttu-id="0e091-175">String</span><span class="sxs-lookup"><span data-stu-id="0e091-175">String</span></span>|<span data-ttu-id="0e091-176">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="0e091-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="0e091-177">initials</span><span class="sxs-lookup"><span data-stu-id="0e091-177">initials</span></span>|<span data-ttu-id="0e091-178">String</span><span class="sxs-lookup"><span data-stu-id="0e091-178">String</span></span>|<span data-ttu-id="0e091-179">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="0e091-179">The contact's initials.</span></span>|
|<span data-ttu-id="0e091-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0e091-180">jobTitle</span></span>|<span data-ttu-id="0e091-181">String</span><span class="sxs-lookup"><span data-stu-id="0e091-181">String</span></span>|<span data-ttu-id="0e091-182">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="0e091-182">The contact’s job title.</span></span>|
|<span data-ttu-id="0e091-183">manager</span><span class="sxs-lookup"><span data-stu-id="0e091-183">manager</span></span>|<span data-ttu-id="0e091-184">String</span><span class="sxs-lookup"><span data-stu-id="0e091-184">String</span></span>|<span data-ttu-id="0e091-185">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="0e091-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="0e091-186">middleName</span><span class="sxs-lookup"><span data-stu-id="0e091-186">middleName</span></span>|<span data-ttu-id="0e091-187">String</span><span class="sxs-lookup"><span data-stu-id="0e091-187">String</span></span>|<span data-ttu-id="0e091-188">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="0e091-188">The contact's middle name.</span></span>|
|<span data-ttu-id="0e091-189">nickName</span><span class="sxs-lookup"><span data-stu-id="0e091-189">nickName</span></span>|<span data-ttu-id="0e091-190">String</span><span class="sxs-lookup"><span data-stu-id="0e091-190">String</span></span>|<span data-ttu-id="0e091-191">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="0e091-191">The contact's nickname.</span></span>|
|<span data-ttu-id="0e091-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0e091-192">officeLocation</span></span>|<span data-ttu-id="0e091-193">String</span><span class="sxs-lookup"><span data-stu-id="0e091-193">String</span></span>|<span data-ttu-id="0e091-194">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="0e091-194">The location of the contact's office.</span></span>|
|<span data-ttu-id="0e091-195">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="0e091-195">parentFolderId</span></span>|<span data-ttu-id="0e091-196">String</span><span class="sxs-lookup"><span data-stu-id="0e091-196">String</span></span>|<span data-ttu-id="0e091-197">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="0e091-197">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="0e091-198">personalNotes</span><span class="sxs-lookup"><span data-stu-id="0e091-198">personalNotes</span></span>|<span data-ttu-id="0e091-199">String</span><span class="sxs-lookup"><span data-stu-id="0e091-199">String</span></span>|<span data-ttu-id="0e091-200">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="0e091-200">The user's notes about the contact.</span></span>|
|<span data-ttu-id="0e091-201">phones</span><span class="sxs-lookup"><span data-stu-id="0e091-201">phones</span></span> |<span data-ttu-id="0e091-202">[phone](../resources/phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e091-202">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="0e091-203">例如，家庭电话、 移动电话和商务电话与该联系人，关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="0e091-203">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="0e091-204">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="0e091-204">postalAddresses</span></span> |<span data-ttu-id="0e091-205">[physicalAddress](../resources/physicaladdress.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e091-205">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="0e091-206">解决与该联系人，例如家庭地址和业务地址。</span><span class="sxs-lookup"><span data-stu-id="0e091-206">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="0e091-207">profession</span><span class="sxs-lookup"><span data-stu-id="0e091-207">profession</span></span>|<span data-ttu-id="0e091-208">String</span><span class="sxs-lookup"><span data-stu-id="0e091-208">String</span></span>|<span data-ttu-id="0e091-209">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="0e091-209">The contact's profession.</span></span>|
|<span data-ttu-id="0e091-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="0e091-210">spouseName</span></span>|<span data-ttu-id="0e091-211">String</span><span class="sxs-lookup"><span data-stu-id="0e091-211">String</span></span>|<span data-ttu-id="0e091-212">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="0e091-212">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="0e091-213">surname</span><span class="sxs-lookup"><span data-stu-id="0e091-213">surname</span></span>|<span data-ttu-id="0e091-214">String</span><span class="sxs-lookup"><span data-stu-id="0e091-214">String</span></span>|<span data-ttu-id="0e091-215">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="0e091-215">The contact's surname.</span></span>|
|<span data-ttu-id="0e091-216">title</span><span class="sxs-lookup"><span data-stu-id="0e091-216">title</span></span>|<span data-ttu-id="0e091-217">字符串</span><span class="sxs-lookup"><span data-stu-id="0e091-217">String</span></span>|<span data-ttu-id="0e091-218">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="0e091-218">The contact's title.</span></span>|
|<span data-ttu-id="0e091-219">websites</span><span class="sxs-lookup"><span data-stu-id="0e091-219">websites</span></span> |<span data-ttu-id="0e091-220">[website](../resources/website.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e091-220">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="0e091-221">与联系人关联的网站。</span><span class="sxs-lookup"><span data-stu-id="0e091-221">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="0e091-222">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="0e091-222">weddingAnniversary</span></span> |<span data-ttu-id="0e091-223">日期</span><span class="sxs-lookup"><span data-stu-id="0e091-223">Date</span></span> |<span data-ttu-id="0e091-224">联系人的婚礼周年日。</span><span class="sxs-lookup"><span data-stu-id="0e091-224">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="0e091-225">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="0e091-225">yomiCompanyName</span></span>|<span data-ttu-id="0e091-226">String</span><span class="sxs-lookup"><span data-stu-id="0e091-226">String</span></span>|<span data-ttu-id="0e091-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="0e091-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="0e091-229">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="0e091-229">yomiGivenName</span></span>|<span data-ttu-id="0e091-230">String</span><span class="sxs-lookup"><span data-stu-id="0e091-230">String</span></span>|<span data-ttu-id="0e091-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="0e091-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="0e091-233">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="0e091-233">yomiSurname</span></span>|<span data-ttu-id="0e091-234">字符串</span><span class="sxs-lookup"><span data-stu-id="0e091-234">String</span></span>|<span data-ttu-id="0e091-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="0e091-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="0e091-237">由于**联系人**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**联系人**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="0e091-237">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="0e091-238">响应</span><span class="sxs-lookup"><span data-stu-id="0e091-238">Response</span></span>

<span data-ttu-id="0e091-239">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新[联系人](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e091-239">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e091-240">示例</span><span class="sxs-lookup"><span data-stu-id="0e091-240">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e091-241">请求</span><span class="sxs-lookup"><span data-stu-id="0e091-241">Request</span></span>
<span data-ttu-id="0e091-242">下面的示例将更新指定的联系人的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0e091-242">The following example updates the personal email address of the specified contact.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0e091-243">响应</span><span class="sxs-lookup"><span data-stu-id="0e091-243">Response</span></span>
<span data-ttu-id="0e091-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e091-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0e091-247">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0e091-247">See also</span></span>

- [<span data-ttu-id="0e091-248">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0e091-248">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0e091-249">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="0e091-249">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/contact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
