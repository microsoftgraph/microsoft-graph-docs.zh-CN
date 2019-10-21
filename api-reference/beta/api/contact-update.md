---
title: 更新联系人
description: 更新 contact 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cc60a830771482d4233c879707e62013d74c838a
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "36418010"
---
# <a name="update-contact"></a><span data-ttu-id="94589-103">更新联系人</span><span class="sxs-lookup"><span data-stu-id="94589-103">Update contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94589-104">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94589-104">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94589-105">权限</span><span class="sxs-lookup"><span data-stu-id="94589-105">Permissions</span></span>
<span data-ttu-id="94589-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94589-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94589-108">Permission type</span></span>      | <span data-ttu-id="94589-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94589-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94589-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94589-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94589-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94589-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="94589-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94589-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94589-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94589-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="94589-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94589-114">Application</span></span> | <span data-ttu-id="94589-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94589-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94589-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94589-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="94589-117">用户的默认[contactFolder](../resources/contactfolder.md)中的[联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="94589-117">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="94589-118">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="94589-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="94589-119">[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="94589-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="94589-120">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="94589-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94589-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="94589-121">Request headers</span></span>
| <span data-ttu-id="94589-122">标头</span><span class="sxs-lookup"><span data-stu-id="94589-122">Header</span></span>       | <span data-ttu-id="94589-123">值</span><span class="sxs-lookup"><span data-stu-id="94589-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94589-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="94589-124">Authorization</span></span>  | <span data-ttu-id="94589-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94589-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94589-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94589-127">Content-Type</span></span>  | <span data-ttu-id="94589-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="94589-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94589-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="94589-130">Request body</span></span>
<span data-ttu-id="94589-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="94589-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94589-134">属性</span><span class="sxs-lookup"><span data-stu-id="94589-134">Property</span></span>     | <span data-ttu-id="94589-135">类型</span><span class="sxs-lookup"><span data-stu-id="94589-135">Type</span></span>   |<span data-ttu-id="94589-136">说明</span><span class="sxs-lookup"><span data-stu-id="94589-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94589-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="94589-137">assistantName</span></span>|<span data-ttu-id="94589-138">String</span><span class="sxs-lookup"><span data-stu-id="94589-138">String</span></span>|<span data-ttu-id="94589-139">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="94589-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="94589-140">birthday</span><span class="sxs-lookup"><span data-stu-id="94589-140">birthday</span></span>|<span data-ttu-id="94589-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94589-141">DateTimeOffset</span></span>|<span data-ttu-id="94589-142">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="94589-142">The contact's birthday.</span></span>|
|<span data-ttu-id="94589-143">categories</span><span class="sxs-lookup"><span data-stu-id="94589-143">categories</span></span>|<span data-ttu-id="94589-144">String</span><span class="sxs-lookup"><span data-stu-id="94589-144">String</span></span>|<span data-ttu-id="94589-145">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="94589-145">The categories associated with the contact.</span></span>|
|<span data-ttu-id="94589-146">children</span><span class="sxs-lookup"><span data-stu-id="94589-146">children</span></span>|<span data-ttu-id="94589-147">String</span><span class="sxs-lookup"><span data-stu-id="94589-147">String</span></span>||
|<span data-ttu-id="94589-148">companyName</span><span class="sxs-lookup"><span data-stu-id="94589-148">companyName</span></span>|<span data-ttu-id="94589-149">String</span><span class="sxs-lookup"><span data-stu-id="94589-149">String</span></span>|<span data-ttu-id="94589-150">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="94589-150">The name of the contact's company.</span></span>|
|<span data-ttu-id="94589-151">部门</span><span class="sxs-lookup"><span data-stu-id="94589-151">department</span></span>|<span data-ttu-id="94589-152">String</span><span class="sxs-lookup"><span data-stu-id="94589-152">String</span></span>|<span data-ttu-id="94589-153">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="94589-153">The contact's department.</span></span>|
|<span data-ttu-id="94589-154">displayName</span><span class="sxs-lookup"><span data-stu-id="94589-154">displayName</span></span>|<span data-ttu-id="94589-155">String</span><span class="sxs-lookup"><span data-stu-id="94589-155">String</span></span>|<span data-ttu-id="94589-156">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="94589-156">The contact's display name.</span></span> <span data-ttu-id="94589-157">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="94589-157">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="94589-158">若要保留预先存在的值，请始终在更新操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="94589-158">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="94589-159">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="94589-159">emailAddresses</span></span>|<span data-ttu-id="94589-160">[typedEmailAddress](../resources/typedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="94589-160">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="94589-161">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="94589-161">The contact's email addresses.</span></span>|
|<span data-ttu-id="94589-162">fileAs</span><span class="sxs-lookup"><span data-stu-id="94589-162">fileAs</span></span>|<span data-ttu-id="94589-163">String</span><span class="sxs-lookup"><span data-stu-id="94589-163">String</span></span>|<span data-ttu-id="94589-164">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="94589-164">The name the contact is filed under.</span></span>|
|<span data-ttu-id="94589-165">gender</span><span class="sxs-lookup"><span data-stu-id="94589-165">gender</span></span> |<span data-ttu-id="94589-166">String</span><span class="sxs-lookup"><span data-stu-id="94589-166">String</span></span> |<span data-ttu-id="94589-167">联系人的性别。</span><span class="sxs-lookup"><span data-stu-id="94589-167">The contact's gender.</span></span> |
|<span data-ttu-id="94589-168">generation</span><span class="sxs-lookup"><span data-stu-id="94589-168">generation</span></span>|<span data-ttu-id="94589-169">String</span><span class="sxs-lookup"><span data-stu-id="94589-169">String</span></span>|<span data-ttu-id="94589-170">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="94589-170">The contact's generation.</span></span>|
|<span data-ttu-id="94589-171">givenName</span><span class="sxs-lookup"><span data-stu-id="94589-171">givenName</span></span>|<span data-ttu-id="94589-172">String</span><span class="sxs-lookup"><span data-stu-id="94589-172">String</span></span>|<span data-ttu-id="94589-173">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="94589-173">The contact's given name.</span></span>|
|<span data-ttu-id="94589-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="94589-174">imAddresses</span></span>|<span data-ttu-id="94589-175">String</span><span class="sxs-lookup"><span data-stu-id="94589-175">String</span></span>|<span data-ttu-id="94589-176">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="94589-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="94589-177">initials</span><span class="sxs-lookup"><span data-stu-id="94589-177">initials</span></span>|<span data-ttu-id="94589-178">String</span><span class="sxs-lookup"><span data-stu-id="94589-178">String</span></span>|<span data-ttu-id="94589-179">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="94589-179">The contact's initials.</span></span>|
|<span data-ttu-id="94589-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="94589-180">jobTitle</span></span>|<span data-ttu-id="94589-181">String</span><span class="sxs-lookup"><span data-stu-id="94589-181">String</span></span>|<span data-ttu-id="94589-182">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="94589-182">The contact’s job title.</span></span>|
|<span data-ttu-id="94589-183">manager</span><span class="sxs-lookup"><span data-stu-id="94589-183">manager</span></span>|<span data-ttu-id="94589-184">String</span><span class="sxs-lookup"><span data-stu-id="94589-184">String</span></span>|<span data-ttu-id="94589-185">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="94589-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="94589-186">middleName</span><span class="sxs-lookup"><span data-stu-id="94589-186">middleName</span></span>|<span data-ttu-id="94589-187">String</span><span class="sxs-lookup"><span data-stu-id="94589-187">String</span></span>|<span data-ttu-id="94589-188">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="94589-188">The contact's middle name.</span></span>|
|<span data-ttu-id="94589-189">nickName</span><span class="sxs-lookup"><span data-stu-id="94589-189">nickName</span></span>|<span data-ttu-id="94589-190">String</span><span class="sxs-lookup"><span data-stu-id="94589-190">String</span></span>|<span data-ttu-id="94589-191">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="94589-191">The contact's nickname.</span></span>|
|<span data-ttu-id="94589-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="94589-192">officeLocation</span></span>|<span data-ttu-id="94589-193">String</span><span class="sxs-lookup"><span data-stu-id="94589-193">String</span></span>|<span data-ttu-id="94589-194">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="94589-194">The location of the contact's office.</span></span>|
|<span data-ttu-id="94589-195">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="94589-195">parentFolderId</span></span>|<span data-ttu-id="94589-196">String</span><span class="sxs-lookup"><span data-stu-id="94589-196">String</span></span>|<span data-ttu-id="94589-197">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="94589-197">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="94589-198">personalNotes</span><span class="sxs-lookup"><span data-stu-id="94589-198">personalNotes</span></span>|<span data-ttu-id="94589-199">String</span><span class="sxs-lookup"><span data-stu-id="94589-199">String</span></span>|<span data-ttu-id="94589-200">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="94589-200">The user's notes about the contact.</span></span>|
|<span data-ttu-id="94589-201">phones</span><span class="sxs-lookup"><span data-stu-id="94589-201">phones</span></span> |<span data-ttu-id="94589-202">[phone](../resources/phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="94589-202">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="94589-203">与联系人关联的电话号码，例如，家庭电话、移动电话和商务电话。</span><span class="sxs-lookup"><span data-stu-id="94589-203">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="94589-204">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="94589-204">postalAddresses</span></span> |<span data-ttu-id="94589-205">[physicalAddress](../resources/physicaladdress.md)集合</span><span class="sxs-lookup"><span data-stu-id="94589-205">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="94589-206">与联系人关联的地址，例如家庭地址和公司地址。</span><span class="sxs-lookup"><span data-stu-id="94589-206">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="94589-207">profession</span><span class="sxs-lookup"><span data-stu-id="94589-207">profession</span></span>|<span data-ttu-id="94589-208">String</span><span class="sxs-lookup"><span data-stu-id="94589-208">String</span></span>|<span data-ttu-id="94589-209">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="94589-209">The contact's profession.</span></span>|
|<span data-ttu-id="94589-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="94589-210">spouseName</span></span>|<span data-ttu-id="94589-211">String</span><span class="sxs-lookup"><span data-stu-id="94589-211">String</span></span>|<span data-ttu-id="94589-212">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="94589-212">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="94589-213">surname</span><span class="sxs-lookup"><span data-stu-id="94589-213">surname</span></span>|<span data-ttu-id="94589-214">String</span><span class="sxs-lookup"><span data-stu-id="94589-214">String</span></span>|<span data-ttu-id="94589-215">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="94589-215">The contact's surname.</span></span>|
|<span data-ttu-id="94589-216">title</span><span class="sxs-lookup"><span data-stu-id="94589-216">title</span></span>|<span data-ttu-id="94589-217">String</span><span class="sxs-lookup"><span data-stu-id="94589-217">String</span></span>|<span data-ttu-id="94589-218">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="94589-218">The contact's title.</span></span>|
|<span data-ttu-id="94589-219">websites</span><span class="sxs-lookup"><span data-stu-id="94589-219">websites</span></span> |<span data-ttu-id="94589-220">[website](../resources/website.md) collection</span><span class="sxs-lookup"><span data-stu-id="94589-220">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="94589-221">与联系人关联的网站。</span><span class="sxs-lookup"><span data-stu-id="94589-221">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="94589-222">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="94589-222">weddingAnniversary</span></span> |<span data-ttu-id="94589-223">日期</span><span class="sxs-lookup"><span data-stu-id="94589-223">Date</span></span> |<span data-ttu-id="94589-224">联系人的婚礼周年纪念。</span><span class="sxs-lookup"><span data-stu-id="94589-224">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="94589-225">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="94589-225">yomiCompanyName</span></span>|<span data-ttu-id="94589-226">String</span><span class="sxs-lookup"><span data-stu-id="94589-226">String</span></span>|<span data-ttu-id="94589-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="94589-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="94589-229">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="94589-229">yomiGivenName</span></span>|<span data-ttu-id="94589-230">字符串</span><span class="sxs-lookup"><span data-stu-id="94589-230">String</span></span>|<span data-ttu-id="94589-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="94589-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="94589-233">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="94589-233">yomiSurname</span></span>|<span data-ttu-id="94589-234">String</span><span class="sxs-lookup"><span data-stu-id="94589-234">String</span></span>|<span data-ttu-id="94589-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="94589-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="94589-237">由于**联系人**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用该`PATCH`操作在现有**联系人**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="94589-237">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="94589-238">响应</span><span class="sxs-lookup"><span data-stu-id="94589-238">Response</span></span>

<span data-ttu-id="94589-239">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[contact](../resources/contact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94589-239">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94589-240">示例</span><span class="sxs-lookup"><span data-stu-id="94589-240">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94589-241">请求</span><span class="sxs-lookup"><span data-stu-id="94589-241">Request</span></span>
<span data-ttu-id="94589-242">下面的示例更新指定联系人的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="94589-242">The following example updates the personal email address of the specified contact.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94589-243">HTTP</span><span class="sxs-lookup"><span data-stu-id="94589-243">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="94589-244">C#</span><span class="sxs-lookup"><span data-stu-id="94589-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94589-245">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94589-245">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94589-246">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94589-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94589-247">响应</span><span class="sxs-lookup"><span data-stu-id="94589-247">Response</span></span>
<span data-ttu-id="94589-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94589-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="94589-251">另请参阅</span><span class="sxs-lookup"><span data-stu-id="94589-251">See also</span></span>

- [<span data-ttu-id="94589-252">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="94589-252">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="94589-253">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="94589-253">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
