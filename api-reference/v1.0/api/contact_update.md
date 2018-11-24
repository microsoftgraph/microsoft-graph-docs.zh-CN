# <a name="update-contact"></a><span data-ttu-id="8a3a2-101">更新联系人</span><span class="sxs-lookup"><span data-stu-id="8a3a2-101">Update contact</span></span>

<span data-ttu-id="8a3a2-102">更新 contact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a3a2-103">权限</span><span class="sxs-lookup"><span data-stu-id="8a3a2-103">Permissions</span></span>
<span data-ttu-id="8a3a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a3a2-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a3a2-106">Permission type</span></span>      | <span data-ttu-id="8a3a2-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a3a2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a3a2-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a3a2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8a3a2-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a3a2-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8a3a2-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a3a2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a3a2-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a3a2-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8a3a2-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a3a2-112">Application</span></span> | <span data-ttu-id="8a3a2-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a3a2-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a3a2-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a3a2-114">HTTP request</span></span>
<span data-ttu-id="8a3a2-115"><!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)从用户的默认[contactFolder](../resources/contactfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-115"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="8a3a2-116">来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="8a3a2-p102">[contactFolder](../resources/mailfolder.md) 的子文件夹中包含的 [联系人](../resources/contact.md)。下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8a3a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a3a2-119">Request headers</span></span>
| <span data-ttu-id="8a3a2-120">标头</span><span class="sxs-lookup"><span data-stu-id="8a3a2-120">Header</span></span>       | <span data-ttu-id="8a3a2-121">值</span><span class="sxs-lookup"><span data-stu-id="8a3a2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a3a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a3a2-122">Authorization</span></span>  | <span data-ttu-id="8a3a2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a3a2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a3a2-125">Content-Type</span></span>  | <span data-ttu-id="8a3a2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a3a2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a3a2-128">Request body</span></span>
<span data-ttu-id="8a3a2-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a3a2-132">属性</span><span class="sxs-lookup"><span data-stu-id="8a3a2-132">Property</span></span>     | <span data-ttu-id="8a3a2-133">类型</span><span class="sxs-lookup"><span data-stu-id="8a3a2-133">Type</span></span>   |<span data-ttu-id="8a3a2-134">说明</span><span class="sxs-lookup"><span data-stu-id="8a3a2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a3a2-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-135">assistantName</span></span>|<span data-ttu-id="8a3a2-136">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-136">String</span></span>|<span data-ttu-id="8a3a2-137">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="8a3a2-138">birthday</span><span class="sxs-lookup"><span data-stu-id="8a3a2-138">birthday</span></span>|<span data-ttu-id="8a3a2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a3a2-139">DateTimeOffset</span></span>|<span data-ttu-id="8a3a2-140">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-140">The contact's birthday.</span></span>|
|<span data-ttu-id="8a3a2-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="8a3a2-141">businessAddress</span></span>|[<span data-ttu-id="8a3a2-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="8a3a2-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8a3a2-143">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-143">The contact's business address.</span></span>|
|<span data-ttu-id="8a3a2-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="8a3a2-144">businessHomePage</span></span>|<span data-ttu-id="8a3a2-145">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-145">String</span></span>|<span data-ttu-id="8a3a2-146">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="8a3a2-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="8a3a2-147">businessPhones</span></span>|<span data-ttu-id="8a3a2-148">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-148">String</span></span>|<span data-ttu-id="8a3a2-149">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="8a3a2-150">categories</span><span class="sxs-lookup"><span data-stu-id="8a3a2-150">categories</span></span>|<span data-ttu-id="8a3a2-151">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-151">String</span></span>|<span data-ttu-id="8a3a2-152">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="8a3a2-153">children</span><span class="sxs-lookup"><span data-stu-id="8a3a2-153">children</span></span>|<span data-ttu-id="8a3a2-154">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-154">String</span></span>|<span data-ttu-id="8a3a2-155">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="8a3a2-156">companyName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-156">companyName</span></span>|<span data-ttu-id="8a3a2-157">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-157">String</span></span>|<span data-ttu-id="8a3a2-158">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="8a3a2-159">department</span><span class="sxs-lookup"><span data-stu-id="8a3a2-159">department</span></span>|<span data-ttu-id="8a3a2-160">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-160">String</span></span>|<span data-ttu-id="8a3a2-161">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-161">The contact's department.</span></span>|
|<span data-ttu-id="8a3a2-162">displayName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-162">displayName</span></span>|<span data-ttu-id="8a3a2-163">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-163">String</span></span>|<span data-ttu-id="8a3a2-164">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-164">The contact's display name.</span></span> <span data-ttu-id="8a3a2-165">请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-165">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="8a3a2-166">若要保留现有的值，始终为在更新操作的 displayName 包括它。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-166">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="8a3a2-167">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="8a3a2-167">emailAddresses</span></span>|<span data-ttu-id="8a3a2-168">[EmailAddress](../resources/emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a3a2-168">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="8a3a2-169">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-169">The contact's email addresses.</span></span>|
|<span data-ttu-id="8a3a2-170">fileAs</span><span class="sxs-lookup"><span data-stu-id="8a3a2-170">fileAs</span></span>|<span data-ttu-id="8a3a2-171">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-171">String</span></span>|<span data-ttu-id="8a3a2-172">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-172">The name the contact is filed under.</span></span>|
|<span data-ttu-id="8a3a2-173">generation</span><span class="sxs-lookup"><span data-stu-id="8a3a2-173">generation</span></span>|<span data-ttu-id="8a3a2-174">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-174">String</span></span>|<span data-ttu-id="8a3a2-175">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-175">The contact's generation.</span></span>|
|<span data-ttu-id="8a3a2-176">givenName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-176">givenName</span></span>|<span data-ttu-id="8a3a2-177">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-177">String</span></span>|<span data-ttu-id="8a3a2-178">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-178">The contact's given name.</span></span>|
|<span data-ttu-id="8a3a2-179">homeAddress</span><span class="sxs-lookup"><span data-stu-id="8a3a2-179">homeAddress</span></span>|[<span data-ttu-id="8a3a2-180">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="8a3a2-180">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8a3a2-181">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-181">The contact's home address.</span></span>|
|<span data-ttu-id="8a3a2-182">homePhones</span><span class="sxs-lookup"><span data-stu-id="8a3a2-182">homePhones</span></span>|<span data-ttu-id="8a3a2-183">String collection</span><span class="sxs-lookup"><span data-stu-id="8a3a2-183">String collection</span></span>|<span data-ttu-id="8a3a2-184">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-184">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="8a3a2-185">imAddresses</span><span class="sxs-lookup"><span data-stu-id="8a3a2-185">imAddresses</span></span>|<span data-ttu-id="8a3a2-186">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-186">String</span></span>|<span data-ttu-id="8a3a2-187">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-187">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="8a3a2-188">initials</span><span class="sxs-lookup"><span data-stu-id="8a3a2-188">initials</span></span>|<span data-ttu-id="8a3a2-189">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-189">String</span></span>|<span data-ttu-id="8a3a2-190">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-190">The contact's initials.</span></span>|
|<span data-ttu-id="8a3a2-191">jobTitle</span><span class="sxs-lookup"><span data-stu-id="8a3a2-191">jobTitle</span></span>|<span data-ttu-id="8a3a2-192">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-192">String</span></span>|<span data-ttu-id="8a3a2-193">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-193">The contact’s job title.</span></span>|
|<span data-ttu-id="8a3a2-194">manager</span><span class="sxs-lookup"><span data-stu-id="8a3a2-194">manager</span></span>|<span data-ttu-id="8a3a2-195">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-195">String</span></span>|<span data-ttu-id="8a3a2-196">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-196">The name of the contact's manager.</span></span>
|<span data-ttu-id="8a3a2-197">middleName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-197">middleName</span></span>|<span data-ttu-id="8a3a2-198">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-198">String</span></span>|<span data-ttu-id="8a3a2-199">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-199">The contact's middle name.</span></span>|
|<span data-ttu-id="8a3a2-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="8a3a2-200">mobilePhone</span></span>|<span data-ttu-id="8a3a2-201">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-201">String</span></span>|<span data-ttu-id="8a3a2-202">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-202">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="8a3a2-203">nickName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-203">nickName</span></span>|<span data-ttu-id="8a3a2-204">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-204">String</span></span>|<span data-ttu-id="8a3a2-205">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-205">The contact's nickname.</span></span>|
|<span data-ttu-id="8a3a2-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="8a3a2-206">officeLocation</span></span>|<span data-ttu-id="8a3a2-207">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-207">String</span></span>|<span data-ttu-id="8a3a2-208">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-208">The location of the contact's office.</span></span>|
|<span data-ttu-id="8a3a2-209">otherAddress</span><span class="sxs-lookup"><span data-stu-id="8a3a2-209">otherAddress</span></span>|[<span data-ttu-id="8a3a2-210">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="8a3a2-210">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8a3a2-211">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-211">Other addresses for the contact.</span></span>|
|<span data-ttu-id="8a3a2-212">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="8a3a2-212">parentFolderId</span></span>|<span data-ttu-id="8a3a2-213">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-213">String</span></span>|<span data-ttu-id="8a3a2-214">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-214">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="8a3a2-215">personalNotes</span><span class="sxs-lookup"><span data-stu-id="8a3a2-215">personalNotes</span></span>|<span data-ttu-id="8a3a2-216">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-216">String</span></span>|<span data-ttu-id="8a3a2-217">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-217">The user's notes about the contact.</span></span>|
|<span data-ttu-id="8a3a2-218">profession</span><span class="sxs-lookup"><span data-stu-id="8a3a2-218">profession</span></span>|<span data-ttu-id="8a3a2-219">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-219">String</span></span>|<span data-ttu-id="8a3a2-220">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-220">The contact's profession.</span></span>|
|<span data-ttu-id="8a3a2-221">spouseName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-221">spouseName</span></span>|<span data-ttu-id="8a3a2-222">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-222">String</span></span>|<span data-ttu-id="8a3a2-223">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-223">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="8a3a2-224">surname</span><span class="sxs-lookup"><span data-stu-id="8a3a2-224">surname</span></span>|<span data-ttu-id="8a3a2-225">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-225">String</span></span>|<span data-ttu-id="8a3a2-226">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-226">The contact's surname.</span></span>|
|<span data-ttu-id="8a3a2-227">title</span><span class="sxs-lookup"><span data-stu-id="8a3a2-227">title</span></span>|<span data-ttu-id="8a3a2-228">String</span><span class="sxs-lookup"><span data-stu-id="8a3a2-228">String</span></span>|<span data-ttu-id="8a3a2-229">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-229">The contact's title.</span></span>|
|<span data-ttu-id="8a3a2-230">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-230">yomiCompanyName</span></span>|<span data-ttu-id="8a3a2-231">字符串</span><span class="sxs-lookup"><span data-stu-id="8a3a2-231">String</span></span>|<span data-ttu-id="8a3a2-p107">联系人的注音日文公司名称。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="8a3a2-234">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="8a3a2-234">yomiGivenName</span></span>|<span data-ttu-id="8a3a2-235">字符串</span><span class="sxs-lookup"><span data-stu-id="8a3a2-235">String</span></span>|<span data-ttu-id="8a3a2-p108">联系人的注音日文名字。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="8a3a2-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="8a3a2-238">yomiSurname</span></span>|<span data-ttu-id="8a3a2-239">字符串</span><span class="sxs-lookup"><span data-stu-id="8a3a2-239">String</span></span>|<span data-ttu-id="8a3a2-p109">联系人的注音日文姓氏。此属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="8a3a2-242">响应</span><span class="sxs-lookup"><span data-stu-id="8a3a2-242">Response</span></span>

<span data-ttu-id="8a3a2-243">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-243">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a3a2-244">示例</span><span class="sxs-lookup"><span data-stu-id="8a3a2-244">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a3a2-245">请求</span><span class="sxs-lookup"><span data-stu-id="8a3a2-245">Request</span></span>
<span data-ttu-id="8a3a2-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-246">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="8a3a2-247">响应</span><span class="sxs-lookup"><span data-stu-id="8a3a2-247">Response</span></span>
<span data-ttu-id="8a3a2-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a3a2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
