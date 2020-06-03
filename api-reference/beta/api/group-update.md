---
title: 更新组
description: 更新[组](../resources/group.md)对象的属性。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 98a2f1188cb86530414f3d8b3ed5a66296f27e32
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524530"
---
# <a name="update-group"></a><span data-ttu-id="7d82c-103">更新组</span><span class="sxs-lookup"><span data-stu-id="7d82c-103">Update group</span></span>

<span data-ttu-id="7d82c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d82c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d82c-105">更新[组](../resources/group.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7d82c-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d82c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7d82c-106">Permissions</span></span>

<span data-ttu-id="7d82c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d82c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d82c-109">Permission type</span></span>      | <span data-ttu-id="7d82c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d82c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d82c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d82c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d82c-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d82c-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7d82c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d82c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d82c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d82c-114">Not supported.</span></span>    |
|<span data-ttu-id="7d82c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d82c-115">Application</span></span> | <span data-ttu-id="7d82c-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d82c-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d82c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d82c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7d82c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d82c-118">Request headers</span></span>

| <span data-ttu-id="7d82c-119">名称</span><span class="sxs-lookup"><span data-stu-id="7d82c-119">Name</span></span>       | <span data-ttu-id="7d82c-120">类型</span><span class="sxs-lookup"><span data-stu-id="7d82c-120">Type</span></span> | <span data-ttu-id="7d82c-121">说明</span><span class="sxs-lookup"><span data-stu-id="7d82c-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7d82c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d82c-122">Authorization</span></span>  | <span data-ttu-id="7d82c-123">string</span><span class="sxs-lookup"><span data-stu-id="7d82c-123">string</span></span>  | <span data-ttu-id="7d82c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d82c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d82c-126">Request body</span></span>

<span data-ttu-id="7d82c-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7d82c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7d82c-130">Property</span></span>   | <span data-ttu-id="7d82c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7d82c-131">Type</span></span> |<span data-ttu-id="7d82c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7d82c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d82c-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="7d82c-133">allowExternalSenders</span></span>|<span data-ttu-id="7d82c-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d82c-134">Boolean</span></span>|<span data-ttu-id="7d82c-p104">默认为 **false**。指明组织外部人员能否向群组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="7d82c-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="7d82c-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="7d82c-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d82c-138">Boolean</span></span>|<span data-ttu-id="7d82c-p105">默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="7d82c-141">description</span><span class="sxs-lookup"><span data-stu-id="7d82c-141">description</span></span>|<span data-ttu-id="7d82c-142">String</span><span class="sxs-lookup"><span data-stu-id="7d82c-142">String</span></span>|<span data-ttu-id="7d82c-143">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="7d82c-143">An optional description for the group.</span></span> |
|<span data-ttu-id="7d82c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="7d82c-144">displayName</span></span>|<span data-ttu-id="7d82c-145">String</span><span class="sxs-lookup"><span data-stu-id="7d82c-145">String</span></span>|<span data-ttu-id="7d82c-p106">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="7d82c-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="7d82c-148">groupTypes</span></span>|<span data-ttu-id="7d82c-149">String collection</span><span class="sxs-lookup"><span data-stu-id="7d82c-149">String collection</span></span>|<span data-ttu-id="7d82c-150">指定组类型及其成员身份。</span><span class="sxs-lookup"><span data-stu-id="7d82c-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="7d82c-151">如果集合包含 **Unified**，则该组是 Office 365 组，否则它是一个安全组。</span><span class="sxs-lookup"><span data-stu-id="7d82c-151">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="7d82c-152">如果该集合包含 **DynamicMembership**，则该组具有动态成员身份；否则，成员身份是静态的。</span><span class="sxs-lookup"><span data-stu-id="7d82c-152">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="7d82c-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7d82c-153">mailEnabled</span></span>|<span data-ttu-id="7d82c-154">布尔</span><span class="sxs-lookup"><span data-stu-id="7d82c-154">Boolean</span></span>|<span data-ttu-id="7d82c-155">指定是否为启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="7d82c-155">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="7d82c-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7d82c-156">mailNickname</span></span>|<span data-ttu-id="7d82c-157">String</span><span class="sxs-lookup"><span data-stu-id="7d82c-157">String</span></span>|<span data-ttu-id="7d82c-158">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="7d82c-158">The mail alias for the group.</span></span> <span data-ttu-id="7d82c-159">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="7d82c-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="7d82c-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7d82c-160">securityEnabled</span></span>|<span data-ttu-id="7d82c-161">布尔</span><span class="sxs-lookup"><span data-stu-id="7d82c-161">Boolean</span></span>|<span data-ttu-id="7d82c-162">指定该组是否为安全组，包括 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="7d82c-162">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="7d82c-163">visibility</span><span class="sxs-lookup"><span data-stu-id="7d82c-163">visibility</span></span>|<span data-ttu-id="7d82c-164">String</span><span class="sxs-lookup"><span data-stu-id="7d82c-164">String</span></span>|<span data-ttu-id="7d82c-p108">指定 Office 365 组的可见性。可能的值是：**专用**、**公用**或空（解释为**公用**）。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="7d82c-167">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用该 `PATCH` 操作在现有**组**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="7d82c-167">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="7d82c-168">**注意：**</span><span class="sxs-lookup"><span data-stu-id="7d82c-168">**Note:**</span></span>
>
> - <span data-ttu-id="7d82c-169">可以更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="7d82c-169">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="7d82c-p109">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="7d82c-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="7d82c-173">在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。</span><span class="sxs-lookup"><span data-stu-id="7d82c-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="7d82c-174">响应</span><span class="sxs-lookup"><span data-stu-id="7d82c-174">Response</span></span>

<span data-ttu-id="7d82c-175">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7d82c-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7d82c-176">示例</span><span class="sxs-lookup"><span data-stu-id="7d82c-176">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="7d82c-177">示例1：更新组的显示名称和说明</span><span class="sxs-lookup"><span data-stu-id="7d82c-177">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="7d82c-178">请求</span><span class="sxs-lookup"><span data-stu-id="7d82c-178">Request</span></span>

<span data-ttu-id="7d82c-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7d82c-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d82c-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d82c-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7d82c-181">C#</span><span class="sxs-lookup"><span data-stu-id="7d82c-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d82c-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d82c-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d82c-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d82c-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d82c-184">响应</span><span class="sxs-lookup"><span data-stu-id="7d82c-184">Response</span></span>

<span data-ttu-id="7d82c-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7d82c-185">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-an-office-365-group"></a><span data-ttu-id="7d82c-186">示例2：将敏感度标签应用于 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="7d82c-186">Example 2: Apply sensitivity label to an Office 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="7d82c-187">请求</span><span class="sxs-lookup"><span data-stu-id="7d82c-187">Request</span></span>

<span data-ttu-id="7d82c-188">您可以使用[列表标签](informationprotectionpolicy-list-labels.md)获取要应用于 Office 365 组的标签的 ID。</span><span class="sxs-lookup"><span data-stu-id="7d82c-188">You can obtain the ID of the label you want to apply to an Office 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="7d82c-189">然后，可以使用标签 ID 更新组的[assignedLabels](../resources/assignedlabel.md)属性。</span><span class="sxs-lookup"><span data-stu-id="7d82c-189">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 

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

#### <a name="response"></a><span data-ttu-id="7d82c-190">响应</span><span class="sxs-lookup"><span data-stu-id="7d82c-190">Response</span></span>

<span data-ttu-id="7d82c-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7d82c-191">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="7d82c-192">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7d82c-192">See also</span></span>

- [<span data-ttu-id="7d82c-193">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7d82c-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7d82c-194">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7d82c-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7d82c-195">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7d82c-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
