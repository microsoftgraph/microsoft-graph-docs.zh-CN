# <a name="update-contact"></a><span data-ttu-id="cdfcf-101">更新联系人</span><span class="sxs-lookup"><span data-stu-id="cdfcf-101">Update contact</span></span>

<span data-ttu-id="cdfcf-102">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdfcf-103">权限</span><span class="sxs-lookup"><span data-stu-id="cdfcf-103">Permissions</span></span>
<span data-ttu-id="cdfcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cdfcf-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdfcf-106">Permission type</span></span>      | <span data-ttu-id="cdfcf-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdfcf-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="cdfcf-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdfcf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cdfcf-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfcf-109">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="cdfcf-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdfcf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfcf-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfcf-111">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="cdfcf-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdfcf-112">Application</span></span> | <span data-ttu-id="cdfcf-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfcf-113">Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cdfcf-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdfcf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cdfcf-115">来自用户的默认 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="cdfcf-116">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="cdfcf-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cdfcf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdfcf-119">Request headers</span></span>
| <span data-ttu-id="cdfcf-120">标头</span><span class="sxs-lookup"><span data-stu-id="cdfcf-120">Header</span></span>       | <span data-ttu-id="cdfcf-121">值</span><span class="sxs-lookup"><span data-stu-id="cdfcf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdfcf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdfcf-122">Authorization</span></span>  | <span data-ttu-id="cdfcf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdfcf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdfcf-125">Content-Type</span></span>  | <span data-ttu-id="cdfcf-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdfcf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdfcf-128">Request body</span></span>
<span data-ttu-id="cdfcf-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cdfcf-132">属性</span><span class="sxs-lookup"><span data-stu-id="cdfcf-132">Property</span></span>     | <span data-ttu-id="cdfcf-133">类型</span><span class="sxs-lookup"><span data-stu-id="cdfcf-133">Type</span></span>   |<span data-ttu-id="cdfcf-134">说明</span><span class="sxs-lookup"><span data-stu-id="cdfcf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdfcf-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-135">assistantName</span></span>|<span data-ttu-id="cdfcf-136">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-136">String</span></span>|<span data-ttu-id="cdfcf-137">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="cdfcf-138">birthday</span><span class="sxs-lookup"><span data-stu-id="cdfcf-138">birthday</span></span>|<span data-ttu-id="cdfcf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdfcf-139">DateTimeOffset</span></span>|<span data-ttu-id="cdfcf-140">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-140">The contact's birthday.</span></span>|
|<span data-ttu-id="cdfcf-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="cdfcf-141">businessAddress</span></span>|[<span data-ttu-id="cdfcf-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="cdfcf-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="cdfcf-143">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-143">The contact's business address.</span></span>|
|<span data-ttu-id="cdfcf-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="cdfcf-144">businessHomePage</span></span>|<span data-ttu-id="cdfcf-145">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-145">String</span></span>|<span data-ttu-id="cdfcf-146">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="cdfcf-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="cdfcf-147">businessPhones</span></span>|<span data-ttu-id="cdfcf-148">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-148">String</span></span>|<span data-ttu-id="cdfcf-149">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="cdfcf-150">categories</span><span class="sxs-lookup"><span data-stu-id="cdfcf-150">categories</span></span>|<span data-ttu-id="cdfcf-151">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-151">String</span></span>|<span data-ttu-id="cdfcf-152">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="cdfcf-153">children</span><span class="sxs-lookup"><span data-stu-id="cdfcf-153">children</span></span>|<span data-ttu-id="cdfcf-154">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-154">String</span></span>|<span data-ttu-id="cdfcf-155">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="cdfcf-156">companyName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-156">companyName</span></span>|<span data-ttu-id="cdfcf-157">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-157">String</span></span>|<span data-ttu-id="cdfcf-158">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="cdfcf-159">department</span><span class="sxs-lookup"><span data-stu-id="cdfcf-159">department</span></span>|<span data-ttu-id="cdfcf-160">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-160">String</span></span>|<span data-ttu-id="cdfcf-161">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-161">The contact's department.</span></span>|
|<span data-ttu-id="cdfcf-162">displayName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-162">displayName</span></span>|<span data-ttu-id="cdfcf-163">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-163">String</span></span>|<span data-ttu-id="cdfcf-164">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-164">The contact's display name.</span></span>|
|<span data-ttu-id="cdfcf-165">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="cdfcf-165">emailAddresses</span></span>|<span data-ttu-id="cdfcf-166">[EmailAddress](../resources/emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cdfcf-166">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="cdfcf-167">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-167">The contact's email addresses.</span></span>|
|<span data-ttu-id="cdfcf-168">fileAs</span><span class="sxs-lookup"><span data-stu-id="cdfcf-168">fileAs</span></span>|<span data-ttu-id="cdfcf-169">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-169">String</span></span>|<span data-ttu-id="cdfcf-170">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-170">The name the contact is filed under.</span></span>|
|<span data-ttu-id="cdfcf-171">generation</span><span class="sxs-lookup"><span data-stu-id="cdfcf-171">generation</span></span>|<span data-ttu-id="cdfcf-172">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-172">String</span></span>|<span data-ttu-id="cdfcf-173">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-173">The contact's generation.</span></span>|
|<span data-ttu-id="cdfcf-174">givenName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-174">givenName</span></span>|<span data-ttu-id="cdfcf-175">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-175">String</span></span>|<span data-ttu-id="cdfcf-176">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-176">The contact's given name.</span></span>|
|<span data-ttu-id="cdfcf-177">homeAddress</span><span class="sxs-lookup"><span data-stu-id="cdfcf-177">homeAddress</span></span>|[<span data-ttu-id="cdfcf-178">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="cdfcf-178">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="cdfcf-179">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-179">The contact's home address.</span></span>|
|<span data-ttu-id="cdfcf-180">homePhones</span><span class="sxs-lookup"><span data-stu-id="cdfcf-180">homePhones</span></span>|<span data-ttu-id="cdfcf-181">String collection</span><span class="sxs-lookup"><span data-stu-id="cdfcf-181">String collection</span></span>|<span data-ttu-id="cdfcf-182">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-182">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="cdfcf-183">imAddresses</span><span class="sxs-lookup"><span data-stu-id="cdfcf-183">imAddresses</span></span>|<span data-ttu-id="cdfcf-184">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-184">String</span></span>|<span data-ttu-id="cdfcf-185">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-185">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="cdfcf-186">initials</span><span class="sxs-lookup"><span data-stu-id="cdfcf-186">initials</span></span>|<span data-ttu-id="cdfcf-187">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-187">String</span></span>|<span data-ttu-id="cdfcf-188">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-188">The contact's initials.</span></span>|
|<span data-ttu-id="cdfcf-189">jobTitle</span><span class="sxs-lookup"><span data-stu-id="cdfcf-189">jobTitle</span></span>|<span data-ttu-id="cdfcf-190">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-190">String</span></span>|<span data-ttu-id="cdfcf-191">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-191">The contact’s job title.</span></span>|
|<span data-ttu-id="cdfcf-192">manager</span><span class="sxs-lookup"><span data-stu-id="cdfcf-192">manager</span></span>|<span data-ttu-id="cdfcf-193">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-193">String</span></span>|<span data-ttu-id="cdfcf-194">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-194">The name of the contact's manager.</span></span>
|<span data-ttu-id="cdfcf-195">middleName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-195">middleName</span></span>|<span data-ttu-id="cdfcf-196">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-196">String</span></span>|<span data-ttu-id="cdfcf-197">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-197">The contact's middle name.</span></span>|
|<span data-ttu-id="cdfcf-198">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="cdfcf-198">mobilePhone</span></span>|<span data-ttu-id="cdfcf-199">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-199">String</span></span>|<span data-ttu-id="cdfcf-200">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-200">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="cdfcf-201">nickName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-201">nickName</span></span>|<span data-ttu-id="cdfcf-202">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-202">String</span></span>|<span data-ttu-id="cdfcf-203">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-203">The contact's nickname.</span></span>|
|<span data-ttu-id="cdfcf-204">officeLocation</span><span class="sxs-lookup"><span data-stu-id="cdfcf-204">officeLocation</span></span>|<span data-ttu-id="cdfcf-205">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-205">String</span></span>|<span data-ttu-id="cdfcf-206">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-206">The location of the contact's office.</span></span>|
|<span data-ttu-id="cdfcf-207">otherAddress</span><span class="sxs-lookup"><span data-stu-id="cdfcf-207">otherAddress</span></span>|[<span data-ttu-id="cdfcf-208">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="cdfcf-208">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="cdfcf-209">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-209">Other addresses for the contact.</span></span>|
|<span data-ttu-id="cdfcf-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="cdfcf-210">parentFolderId</span></span>|<span data-ttu-id="cdfcf-211">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-211">String</span></span>|<span data-ttu-id="cdfcf-212">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-212">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="cdfcf-213">personalNotes</span><span class="sxs-lookup"><span data-stu-id="cdfcf-213">personalNotes</span></span>|<span data-ttu-id="cdfcf-214">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-214">String</span></span>|<span data-ttu-id="cdfcf-215">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-215">The user's notes about the contact.</span></span>|
|<span data-ttu-id="cdfcf-216">profession</span><span class="sxs-lookup"><span data-stu-id="cdfcf-216">profession</span></span>|<span data-ttu-id="cdfcf-217">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-217">String</span></span>|<span data-ttu-id="cdfcf-218">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-218">The contact's profession.</span></span>|
|<span data-ttu-id="cdfcf-219">spouseName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-219">spouseName</span></span>|<span data-ttu-id="cdfcf-220">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-220">String</span></span>|<span data-ttu-id="cdfcf-221">联系人配偶的姓名。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-221">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="cdfcf-222">surname</span><span class="sxs-lookup"><span data-stu-id="cdfcf-222">surname</span></span>|<span data-ttu-id="cdfcf-223">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-223">String</span></span>|<span data-ttu-id="cdfcf-224">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-224">The contact's surname.</span></span>|
|<span data-ttu-id="cdfcf-225">title</span><span class="sxs-lookup"><span data-stu-id="cdfcf-225">title</span></span>|<span data-ttu-id="cdfcf-226">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-226">String</span></span>|<span data-ttu-id="cdfcf-227">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-227">The contact's title.</span></span>|
|<span data-ttu-id="cdfcf-228">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-228">yomiCompanyName</span></span>|<span data-ttu-id="cdfcf-229">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-229">String</span></span>|<span data-ttu-id="cdfcf-p106">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p106">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="cdfcf-232">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="cdfcf-232">yomiGivenName</span></span>|<span data-ttu-id="cdfcf-233">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-233">String</span></span>|<span data-ttu-id="cdfcf-p107">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p107">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="cdfcf-236">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="cdfcf-236">yomiSurname</span></span>|<span data-ttu-id="cdfcf-237">String</span><span class="sxs-lookup"><span data-stu-id="cdfcf-237">String</span></span>|<span data-ttu-id="cdfcf-p108">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p108">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="cdfcf-240">响应</span><span class="sxs-lookup"><span data-stu-id="cdfcf-240">Response</span></span>

<span data-ttu-id="cdfcf-241">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-241">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdfcf-242">示例</span><span class="sxs-lookup"><span data-stu-id="cdfcf-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdfcf-243">请求</span><span class="sxs-lookup"><span data-stu-id="cdfcf-243">Request</span></span>
<span data-ttu-id="cdfcf-244">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-244">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="cdfcf-245">响应</span><span class="sxs-lookup"><span data-stu-id="cdfcf-245">Response</span></span>
<span data-ttu-id="cdfcf-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdfcf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
