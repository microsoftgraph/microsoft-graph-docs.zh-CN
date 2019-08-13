---
title: 更新组
description: 更新[组](../resources/group.md)对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 12db45a1f1361ece2d98435fa5ea16dee6adc129
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323102"
---
# <a name="update-group"></a><span data-ttu-id="aca6e-103">更新组</span><span class="sxs-lookup"><span data-stu-id="aca6e-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aca6e-104">更新[组](../resources/group.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aca6e-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aca6e-105">权限</span><span class="sxs-lookup"><span data-stu-id="aca6e-105">Permissions</span></span>

<span data-ttu-id="aca6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aca6e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aca6e-108">Permission type</span></span>      | <span data-ttu-id="aca6e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aca6e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aca6e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aca6e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aca6e-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aca6e-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="aca6e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aca6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aca6e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="aca6e-113">Not supported.</span></span>    |
|<span data-ttu-id="aca6e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aca6e-114">Application</span></span> | <span data-ttu-id="aca6e-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca6e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aca6e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aca6e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="aca6e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="aca6e-117">Request headers</span></span>

| <span data-ttu-id="aca6e-118">名称</span><span class="sxs-lookup"><span data-stu-id="aca6e-118">Name</span></span>       | <span data-ttu-id="aca6e-119">类型</span><span class="sxs-lookup"><span data-stu-id="aca6e-119">Type</span></span> | <span data-ttu-id="aca6e-120">说明</span><span class="sxs-lookup"><span data-stu-id="aca6e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aca6e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aca6e-121">Authorization</span></span>  | <span data-ttu-id="aca6e-122">string</span><span class="sxs-lookup"><span data-stu-id="aca6e-122">string</span></span>  | <span data-ttu-id="aca6e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aca6e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="aca6e-125">Request body</span></span>

<span data-ttu-id="aca6e-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aca6e-129">属性</span><span class="sxs-lookup"><span data-stu-id="aca6e-129">Property</span></span>   | <span data-ttu-id="aca6e-130">类型</span><span class="sxs-lookup"><span data-stu-id="aca6e-130">Type</span></span> |<span data-ttu-id="aca6e-131">说明</span><span class="sxs-lookup"><span data-stu-id="aca6e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aca6e-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="aca6e-132">allowExternalSenders</span></span>|<span data-ttu-id="aca6e-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="aca6e-133">Boolean</span></span>|<span data-ttu-id="aca6e-p104">默认为 **false**。指明组织外部人员能否向群组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="aca6e-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="aca6e-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="aca6e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="aca6e-137">Boolean</span></span>|<span data-ttu-id="aca6e-p105">默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="aca6e-140">description</span><span class="sxs-lookup"><span data-stu-id="aca6e-140">description</span></span>|<span data-ttu-id="aca6e-141">String</span><span class="sxs-lookup"><span data-stu-id="aca6e-141">String</span></span>|<span data-ttu-id="aca6e-142">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="aca6e-142">An optional description for the group.</span></span> |
|<span data-ttu-id="aca6e-143">displayName</span><span class="sxs-lookup"><span data-stu-id="aca6e-143">displayName</span></span>|<span data-ttu-id="aca6e-144">String</span><span class="sxs-lookup"><span data-stu-id="aca6e-144">String</span></span>|<span data-ttu-id="aca6e-145">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aca6e-145">The display name for the group.</span></span> <span data-ttu-id="aca6e-146">此属性是在创建组时所必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="aca6e-146">This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="aca6e-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="aca6e-147">groupTypes</span></span>|<span data-ttu-id="aca6e-148">String collection</span><span class="sxs-lookup"><span data-stu-id="aca6e-148">String collection</span></span>|<span data-ttu-id="aca6e-149">指定组类型及其成员身份。</span><span class="sxs-lookup"><span data-stu-id="aca6e-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="aca6e-150">如果集合包含**统一**的, 则组为 Office 365 组;否则, 它是一个安全组。</span><span class="sxs-lookup"><span data-stu-id="aca6e-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="aca6e-151">如果集合包括**DynamicMembership**, 则组具有动态成员身份;否则, 成员身份是静态的。</span><span class="sxs-lookup"><span data-stu-id="aca6e-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="aca6e-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="aca6e-152">mailEnabled</span></span>|<span data-ttu-id="aca6e-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="aca6e-153">Boolean</span></span>|<span data-ttu-id="aca6e-154">指定该组是否启用邮件。</span><span class="sxs-lookup"><span data-stu-id="aca6e-154">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="aca6e-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="aca6e-155">mailNickname</span></span>|<span data-ttu-id="aca6e-156">String</span><span class="sxs-lookup"><span data-stu-id="aca6e-156">String</span></span>|<span data-ttu-id="aca6e-157">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="aca6e-157">The mail alias for the group.</span></span> <span data-ttu-id="aca6e-158">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="aca6e-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="aca6e-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="aca6e-159">securityEnabled</span></span>|<span data-ttu-id="aca6e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="aca6e-160">Boolean</span></span>|<span data-ttu-id="aca6e-161">指定该组是否为安全组, 包括 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="aca6e-161">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="aca6e-162">visibility</span><span class="sxs-lookup"><span data-stu-id="aca6e-162">visibility</span></span>|<span data-ttu-id="aca6e-163">String</span><span class="sxs-lookup"><span data-stu-id="aca6e-163">String</span></span>|<span data-ttu-id="aca6e-p108">指定 Office 365 组的可见性。可能的值是：**专用**、**公用**或空（解释为**公用**）。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="aca6e-166">由于**组**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**组**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="aca6e-166">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="aca6e-167">**注意：**</span><span class="sxs-lookup"><span data-stu-id="aca6e-167">**Note:**</span></span>
>
> - <span data-ttu-id="aca6e-168">可以更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="aca6e-168">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="aca6e-p109">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="aca6e-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="aca6e-172">在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能非常复杂;若要了解详细信息, 请参阅[在 Exchange Server 中管理启用邮件的安全组](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。</span><span class="sxs-lookup"><span data-stu-id="aca6e-172">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>
 


## <a name="response"></a><span data-ttu-id="aca6e-173">响应</span><span class="sxs-lookup"><span data-stu-id="aca6e-173">Response</span></span>

<span data-ttu-id="aca6e-174">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aca6e-174">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aca6e-175">示例</span><span class="sxs-lookup"><span data-stu-id="aca6e-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aca6e-176">请求</span><span class="sxs-lookup"><span data-stu-id="aca6e-176">Request</span></span>

<span data-ttu-id="aca6e-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aca6e-177">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aca6e-178">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="aca6e-178">HTTP</span></span>](#tab/http)
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
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aca6e-179">C#</span><span class="sxs-lookup"><span data-stu-id="aca6e-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aca6e-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aca6e-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aca6e-181">目标-C</span><span class="sxs-lookup"><span data-stu-id="aca6e-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aca6e-182">Java</span><span class="sxs-lookup"><span data-stu-id="aca6e-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aca6e-183">响应</span><span class="sxs-lookup"><span data-stu-id="aca6e-183">Response</span></span>

<span data-ttu-id="aca6e-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aca6e-184">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="aca6e-185">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aca6e-185">See also</span></span>

- [<span data-ttu-id="aca6e-186">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="aca6e-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="aca6e-187">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="aca6e-187">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="aca6e-188">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="aca6e-188">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
