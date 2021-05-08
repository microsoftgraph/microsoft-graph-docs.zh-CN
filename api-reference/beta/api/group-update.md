---
title: 更新组
description: 更新 group [对象的属性](../resources/group.md) 。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 51a34d50801914dcc3e1e10c1813c25543880c0b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240754"
---
# <a name="update-group"></a><span data-ttu-id="a7bd9-103">更新组</span><span class="sxs-lookup"><span data-stu-id="a7bd9-103">Update group</span></span>

<span data-ttu-id="a7bd9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7bd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7bd9-105">更新 group [对象的属性](../resources/group.md) 。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7bd9-106">权限</span><span class="sxs-lookup"><span data-stu-id="a7bd9-106">Permissions</span></span>

<span data-ttu-id="a7bd9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7bd9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7bd9-109">Permission type</span></span>      | <span data-ttu-id="a7bd9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7bd9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7bd9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7bd9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7bd9-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7bd9-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="a7bd9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7bd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7bd9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-114">Not supported.</span></span>    |
|<span data-ttu-id="a7bd9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7bd9-115">Application</span></span> | <span data-ttu-id="a7bd9-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7bd9-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7bd9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7bd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7bd9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7bd9-118">Request headers</span></span>

| <span data-ttu-id="a7bd9-119">名称</span><span class="sxs-lookup"><span data-stu-id="a7bd9-119">Name</span></span>       | <span data-ttu-id="a7bd9-120">类型</span><span class="sxs-lookup"><span data-stu-id="a7bd9-120">Type</span></span> | <span data-ttu-id="a7bd9-121">说明</span><span class="sxs-lookup"><span data-stu-id="a7bd9-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7bd9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7bd9-122">Authorization</span></span>  | <span data-ttu-id="a7bd9-123">string</span><span class="sxs-lookup"><span data-stu-id="a7bd9-123">string</span></span>  | <span data-ttu-id="a7bd9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7bd9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7bd9-126">Request body</span></span>

<span data-ttu-id="a7bd9-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7bd9-130">属性</span><span class="sxs-lookup"><span data-stu-id="a7bd9-130">Property</span></span>   | <span data-ttu-id="a7bd9-131">类型</span><span class="sxs-lookup"><span data-stu-id="a7bd9-131">Type</span></span> |<span data-ttu-id="a7bd9-132">说明</span><span class="sxs-lookup"><span data-stu-id="a7bd9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7bd9-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="a7bd9-133">allowExternalSenders</span></span>|<span data-ttu-id="a7bd9-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7bd9-134">Boolean</span></span>|<span data-ttu-id="a7bd9-135">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-135">Default is `false`.</span></span> <span data-ttu-id="a7bd9-136">指示组织外部人员是否可以向该组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-136">Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="a7bd9-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="a7bd9-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="a7bd9-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7bd9-138">Boolean</span></span>|<span data-ttu-id="a7bd9-139">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-139">Default is `false`.</span></span> <span data-ttu-id="a7bd9-140">指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="a7bd9-141">当组上的 **subscriptionEnabled** 设置为 `false` 时，**autoSubscribeNewMembers** 不能为 `true`。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="a7bd9-142">说明</span><span class="sxs-lookup"><span data-stu-id="a7bd9-142">description</span></span>|<span data-ttu-id="a7bd9-143">String</span><span class="sxs-lookup"><span data-stu-id="a7bd9-143">String</span></span>|<span data-ttu-id="a7bd9-144">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-144">An optional description for the group.</span></span>|
|<span data-ttu-id="a7bd9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a7bd9-145">displayName</span></span>|<span data-ttu-id="a7bd9-146">String</span><span class="sxs-lookup"><span data-stu-id="a7bd9-146">String</span></span>|<span data-ttu-id="a7bd9-p106">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="a7bd9-149">groupTypes</span><span class="sxs-lookup"><span data-stu-id="a7bd9-149">groupTypes</span></span>|<span data-ttu-id="a7bd9-150">String collection</span><span class="sxs-lookup"><span data-stu-id="a7bd9-150">String collection</span></span>|<span data-ttu-id="a7bd9-151">指定组类型及其成员身份。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-151">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="a7bd9-152">如果集合包含 **Unified，** 则组是一Microsoft 365组;否则，它是一个安全组。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-152">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise, it's a security group.</span></span>  <br><br><span data-ttu-id="a7bd9-153">如果该集合包含 **DynamicMembership**，则该组具有动态成员身份；否则，成员身份是静态的。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-153">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="a7bd9-154">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="a7bd9-154">mailEnabled</span></span>|<span data-ttu-id="a7bd9-155">布尔</span><span class="sxs-lookup"><span data-stu-id="a7bd9-155">Boolean</span></span>|<span data-ttu-id="a7bd9-156">指定是否为启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-156">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="a7bd9-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a7bd9-157">mailNickname</span></span>|<span data-ttu-id="a7bd9-158">String</span><span class="sxs-lookup"><span data-stu-id="a7bd9-158">String</span></span>|<span data-ttu-id="a7bd9-159">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-159">The mail alias for the group.</span></span> <span data-ttu-id="a7bd9-160">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-160">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="a7bd9-161">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="a7bd9-161">securityEnabled</span></span>|<span data-ttu-id="a7bd9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7bd9-162">Boolean</span></span>|<span data-ttu-id="a7bd9-163">指定组是否是安全组，包括Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-163">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="a7bd9-164">visibility</span><span class="sxs-lookup"><span data-stu-id="a7bd9-164">visibility</span></span>|<span data-ttu-id="a7bd9-165">字符串</span><span class="sxs-lookup"><span data-stu-id="a7bd9-165">String</span></span>|<span data-ttu-id="a7bd9-166">指定 Microsoft 365 组的可见性。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-166">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="a7bd9-167">可能的值是：**专用**、**公用** 或空（解释为 **公用**）。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-167">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="a7bd9-168">由于 **组** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作添加、更新或删除现有组实例中扩展的自定义属性中你自己的特定于 `PATCH` 应用的数据。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-168">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="a7bd9-169">**注意：**</span><span class="sxs-lookup"><span data-stu-id="a7bd9-169">**Note:**</span></span>
>
> - <span data-ttu-id="a7bd9-170">可以通过在 **补丁请求中指定** 自动更新 **autoSubendalNewMembers** ，而不包括上表中其他属性。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-170">You can update **allowExternalSenders** and **autoSubscribeNewMembers** by specifying them in their own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="a7bd9-p109">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅 [已知问题](/graph/known-issues#group)。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#group) for examples.</span></span>
> - <span data-ttu-id="a7bd9-174">在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-174">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="a7bd9-175">响应</span><span class="sxs-lookup"><span data-stu-id="a7bd9-175">Response</span></span>

<span data-ttu-id="a7bd9-176">如果成功， 此方法返回 `204 No Content` 响应代码 - 更新下列属性时除了 `200 OK` 响应代码：**allowEx在alSenders**、 **autoSubendNewMembers**， **HideFromAddressList**， **hideFromOutlookClients**， **isSubeendByMail**， **unseenCount**。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-176">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="examples"></a><span data-ttu-id="a7bd9-177">示例</span><span class="sxs-lookup"><span data-stu-id="a7bd9-177">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="a7bd9-178">示例 1：显示名称组更新组和说明</span><span class="sxs-lookup"><span data-stu-id="a7bd9-178">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="a7bd9-179">请求</span><span class="sxs-lookup"><span data-stu-id="a7bd9-179">Request</span></span>

<span data-ttu-id="a7bd9-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a7bd9-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7bd9-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
   "description":"description-value",
   "displayName":"displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="a7bd9-182">C#</span><span class="sxs-lookup"><span data-stu-id="a7bd9-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7bd9-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7bd9-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7bd9-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7bd9-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7bd9-185">Java</span><span class="sxs-lookup"><span data-stu-id="a7bd9-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a7bd9-186">响应</span><span class="sxs-lookup"><span data-stu-id="a7bd9-186">Response</span></span>

<span data-ttu-id="a7bd9-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-187">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="a7bd9-188">示例 2：将敏感度标签应用于Microsoft 365组</span><span class="sxs-lookup"><span data-stu-id="a7bd9-188">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="a7bd9-189">请求</span><span class="sxs-lookup"><span data-stu-id="a7bd9-189">Request</span></span>

<span data-ttu-id="a7bd9-190">可以使用列表标签 获取要应用于组Microsoft 365 [ID。](informationprotectionpolicy-list-labels.md)</span><span class="sxs-lookup"><span data-stu-id="a7bd9-190">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="a7bd9-191">然后，可以使用标签 ID 更新组的 [assignedLabels](../resources/assignedlabel.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-191">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 


# <a name="http"></a>[<span data-ttu-id="a7bd9-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7bd9-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "assignedLabels": 
  [
    {
        "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a7bd9-193">C#</span><span class="sxs-lookup"><span data-stu-id="a7bd9-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7bd9-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7bd9-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7bd9-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7bd9-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7bd9-196">Java</span><span class="sxs-lookup"><span data-stu-id="a7bd9-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a7bd9-197">响应</span><span class="sxs-lookup"><span data-stu-id="a7bd9-197">Response</span></span>

<span data-ttu-id="a7bd9-198">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a7bd9-198">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a7bd9-199">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a7bd9-199">See also</span></span>

- [<span data-ttu-id="a7bd9-200">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a7bd9-200">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a7bd9-201">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a7bd9-201">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a7bd9-202">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a7bd9-202">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
