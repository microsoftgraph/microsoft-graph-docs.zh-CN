---
title: 更新组
description: 更新[组](../resources/group.md)对象的属性。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d38fdab04f4f470ba9c712f4447ecae3aa7d79bb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895774"
---
# <a name="update-group"></a><span data-ttu-id="944d2-103">更新组</span><span class="sxs-lookup"><span data-stu-id="944d2-103">Update group</span></span>

<span data-ttu-id="944d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="944d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="944d2-105">更新[组](../resources/group.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="944d2-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="944d2-106">权限</span><span class="sxs-lookup"><span data-stu-id="944d2-106">Permissions</span></span>

<span data-ttu-id="944d2-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="944d2-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="944d2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="944d2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="944d2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="944d2-109">Permission type</span></span>      | <span data-ttu-id="944d2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="944d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="944d2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="944d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="944d2-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="944d2-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="944d2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="944d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="944d2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="944d2-114">Not supported.</span></span>    |
|<span data-ttu-id="944d2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="944d2-115">Application</span></span> | <span data-ttu-id="944d2-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944d2-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="944d2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="944d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="944d2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="944d2-118">Request headers</span></span>

| <span data-ttu-id="944d2-119">名称</span><span class="sxs-lookup"><span data-stu-id="944d2-119">Name</span></span>       | <span data-ttu-id="944d2-120">类型</span><span class="sxs-lookup"><span data-stu-id="944d2-120">Type</span></span> | <span data-ttu-id="944d2-121">说明</span><span class="sxs-lookup"><span data-stu-id="944d2-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="944d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="944d2-122">Authorization</span></span>  | <span data-ttu-id="944d2-123">string</span><span class="sxs-lookup"><span data-stu-id="944d2-123">string</span></span>  | <span data-ttu-id="944d2-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="944d2-124">Bearer {token}.</span></span> <span data-ttu-id="944d2-125">Required.</span><span class="sxs-lookup"><span data-stu-id="944d2-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="944d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="944d2-126">Request body</span></span>

<span data-ttu-id="944d2-127">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="944d2-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="944d2-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="944d2-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="944d2-129">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="944d2-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="944d2-130">属性</span><span class="sxs-lookup"><span data-stu-id="944d2-130">Property</span></span>   | <span data-ttu-id="944d2-131">类型</span><span class="sxs-lookup"><span data-stu-id="944d2-131">Type</span></span> |<span data-ttu-id="944d2-132">说明</span><span class="sxs-lookup"><span data-stu-id="944d2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="944d2-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="944d2-133">allowExternalSenders</span></span>|<span data-ttu-id="944d2-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="944d2-134">Boolean</span></span>|<span data-ttu-id="944d2-135">Default is **false**.</span><span class="sxs-lookup"><span data-stu-id="944d2-135">Default is **false**.</span></span> <span data-ttu-id="944d2-136">Indicates if people external to the organization can send messages to the group.</span><span class="sxs-lookup"><span data-stu-id="944d2-136">Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="944d2-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="944d2-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="944d2-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="944d2-138">Boolean</span></span>|<span data-ttu-id="944d2-139">Default is **false**.</span><span class="sxs-lookup"><span data-stu-id="944d2-139">Default is **false**.</span></span> <span data-ttu-id="944d2-140">Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span><span class="sxs-lookup"><span data-stu-id="944d2-140">Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="944d2-141">description</span><span class="sxs-lookup"><span data-stu-id="944d2-141">description</span></span>|<span data-ttu-id="944d2-142">String</span><span class="sxs-lookup"><span data-stu-id="944d2-142">String</span></span>|<span data-ttu-id="944d2-143">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="944d2-143">An optional description for the group.</span></span> |
|<span data-ttu-id="944d2-144">displayName</span><span class="sxs-lookup"><span data-stu-id="944d2-144">displayName</span></span>|<span data-ttu-id="944d2-145">String</span><span class="sxs-lookup"><span data-stu-id="944d2-145">String</span></span>|<span data-ttu-id="944d2-146">The display name for the group.</span><span class="sxs-lookup"><span data-stu-id="944d2-146">The display name for the group.</span></span> <span data-ttu-id="944d2-147">This property is required when a group is created and it cannot be cleared during updates.</span><span class="sxs-lookup"><span data-stu-id="944d2-147">This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="944d2-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="944d2-148">groupTypes</span></span>|<span data-ttu-id="944d2-149">String collection</span><span class="sxs-lookup"><span data-stu-id="944d2-149">String collection</span></span>|<span data-ttu-id="944d2-150">指定组类型及其成员身份。</span><span class="sxs-lookup"><span data-stu-id="944d2-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="944d2-151">如果集合包含**统一**的，则组为 Microsoft 365 组;否则，它是一个安全组。</span><span class="sxs-lookup"><span data-stu-id="944d2-151">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="944d2-152">如果该集合包含 **DynamicMembership**，则该组具有动态成员身份；否则，成员身份是静态的。</span><span class="sxs-lookup"><span data-stu-id="944d2-152">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="944d2-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="944d2-153">mailEnabled</span></span>|<span data-ttu-id="944d2-154">布尔</span><span class="sxs-lookup"><span data-stu-id="944d2-154">Boolean</span></span>|<span data-ttu-id="944d2-155">指定是否为启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="944d2-155">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="944d2-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="944d2-156">mailNickname</span></span>|<span data-ttu-id="944d2-157">String</span><span class="sxs-lookup"><span data-stu-id="944d2-157">String</span></span>|<span data-ttu-id="944d2-158">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="944d2-158">The mail alias for the group.</span></span> <span data-ttu-id="944d2-159">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="944d2-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="944d2-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="944d2-160">securityEnabled</span></span>|<span data-ttu-id="944d2-161">布尔</span><span class="sxs-lookup"><span data-stu-id="944d2-161">Boolean</span></span>|<span data-ttu-id="944d2-162">指定该组是否为安全组，包括 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="944d2-162">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="944d2-163">visibility</span><span class="sxs-lookup"><span data-stu-id="944d2-163">visibility</span></span>|<span data-ttu-id="944d2-164">String</span><span class="sxs-lookup"><span data-stu-id="944d2-164">String</span></span>|<span data-ttu-id="944d2-165">指定 Microsoft 365 组的可见性。</span><span class="sxs-lookup"><span data-stu-id="944d2-165">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="944d2-166">可能的值是：**专用**、**公用**或空（解释为**公用**）。</span><span class="sxs-lookup"><span data-stu-id="944d2-166">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="944d2-167">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用该 `PATCH` 操作在现有**组**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="944d2-167">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="944d2-168">**注意：**</span><span class="sxs-lookup"><span data-stu-id="944d2-168">**Note:**</span></span>
>
> - <span data-ttu-id="944d2-169">可以更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="944d2-169">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="944d2-170">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions.</span><span class="sxs-lookup"><span data-stu-id="944d2-170">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions.</span></span> <span data-ttu-id="944d2-171">All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions.</span><span class="sxs-lookup"><span data-stu-id="944d2-171">All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions.</span></span> <span data-ttu-id="944d2-172">See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span><span class="sxs-lookup"><span data-stu-id="944d2-172">See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="944d2-173">在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。</span><span class="sxs-lookup"><span data-stu-id="944d2-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="944d2-174">响应</span><span class="sxs-lookup"><span data-stu-id="944d2-174">Response</span></span>

<span data-ttu-id="944d2-175">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="944d2-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="944d2-176">示例</span><span class="sxs-lookup"><span data-stu-id="944d2-176">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="944d2-177">示例1：更新组的显示名称和说明</span><span class="sxs-lookup"><span data-stu-id="944d2-177">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="944d2-178">请求</span><span class="sxs-lookup"><span data-stu-id="944d2-178">Request</span></span>

<span data-ttu-id="944d2-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="944d2-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="944d2-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="944d2-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="944d2-181">C#</span><span class="sxs-lookup"><span data-stu-id="944d2-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="944d2-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="944d2-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="944d2-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="944d2-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="944d2-184">响应</span><span class="sxs-lookup"><span data-stu-id="944d2-184">Response</span></span>

<span data-ttu-id="944d2-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="944d2-185">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="944d2-186">示例2：将敏感度标签应用于 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="944d2-186">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="944d2-187">请求</span><span class="sxs-lookup"><span data-stu-id="944d2-187">Request</span></span>

<span data-ttu-id="944d2-188">您可以使用[列表标签](informationprotectionpolicy-list-labels.md)获取要应用于 Microsoft 365 组的标签的 ID。</span><span class="sxs-lookup"><span data-stu-id="944d2-188">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="944d2-189">然后，可以使用标签 ID 更新组的[assignedLabels](../resources/assignedlabel.md)属性。</span><span class="sxs-lookup"><span data-stu-id="944d2-189">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_group"
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

#### <a name="response"></a><span data-ttu-id="944d2-190">响应</span><span class="sxs-lookup"><span data-stu-id="944d2-190">Response</span></span>

<span data-ttu-id="944d2-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="944d2-191">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="944d2-192">另请参阅</span><span class="sxs-lookup"><span data-stu-id="944d2-192">See also</span></span>

- [<span data-ttu-id="944d2-193">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="944d2-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="944d2-194">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="944d2-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="944d2-195">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="944d2-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
