---
title: 更新组
description: 更新 group 对象的属性。
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 36b8a21589bdfd1687939eb636bf5de254d37bab
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680736"
---
# <a name="update-group"></a><span data-ttu-id="32d37-103">更新组</span><span class="sxs-lookup"><span data-stu-id="32d37-103">Update group</span></span>

<span data-ttu-id="32d37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32d37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32d37-105">更新 group 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="32d37-105">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="32d37-106">权限</span><span class="sxs-lookup"><span data-stu-id="32d37-106">Permissions</span></span>

<span data-ttu-id="32d37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32d37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32d37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="32d37-109">Permission type</span></span>      | <span data-ttu-id="32d37-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32d37-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32d37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32d37-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32d37-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="32d37-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="32d37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32d37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32d37-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="32d37-114">Not supported.</span></span>    |
|<span data-ttu-id="32d37-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="32d37-115">Application</span></span> | <span data-ttu-id="32d37-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d37-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32d37-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32d37-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32d37-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="32d37-118">Request headers</span></span>

| <span data-ttu-id="32d37-119">名称</span><span class="sxs-lookup"><span data-stu-id="32d37-119">Name</span></span>       | <span data-ttu-id="32d37-120">类型</span><span class="sxs-lookup"><span data-stu-id="32d37-120">Type</span></span> | <span data-ttu-id="32d37-121">说明</span><span class="sxs-lookup"><span data-stu-id="32d37-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="32d37-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32d37-122">Authorization</span></span>  | <span data-ttu-id="32d37-123">string</span><span class="sxs-lookup"><span data-stu-id="32d37-123">string</span></span>  | <span data-ttu-id="32d37-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32d37-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32d37-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="32d37-126">Request body</span></span>

<span data-ttu-id="32d37-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="32d37-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="32d37-130">属性</span><span class="sxs-lookup"><span data-stu-id="32d37-130">Property</span></span>   | <span data-ttu-id="32d37-131">类型</span><span class="sxs-lookup"><span data-stu-id="32d37-131">Type</span></span> |<span data-ttu-id="32d37-132">说明</span><span class="sxs-lookup"><span data-stu-id="32d37-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32d37-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="32d37-133">allowExternalSenders</span></span>|<span data-ttu-id="32d37-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="32d37-134">Boolean</span></span>|<span data-ttu-id="32d37-135">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="32d37-135">Default is `false`.</span></span> <span data-ttu-id="32d37-136">指示组织外部人员是否可以向该组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="32d37-136">Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="32d37-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="32d37-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="32d37-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="32d37-138">Boolean</span></span>|<span data-ttu-id="32d37-139">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="32d37-139">Default is `false`.</span></span> <span data-ttu-id="32d37-140">指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="32d37-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="32d37-141">当组上的 **subscriptionEnabled** 设置为 `false` 时，**autoSubscribeNewMembers** 不能为 `true`。</span><span class="sxs-lookup"><span data-stu-id="32d37-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="32d37-142">说明</span><span class="sxs-lookup"><span data-stu-id="32d37-142">description</span></span>|<span data-ttu-id="32d37-143">String</span><span class="sxs-lookup"><span data-stu-id="32d37-143">String</span></span>|<span data-ttu-id="32d37-144">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="32d37-144">An optional description for the group.</span></span> |
|<span data-ttu-id="32d37-145">displayName</span><span class="sxs-lookup"><span data-stu-id="32d37-145">displayName</span></span>|<span data-ttu-id="32d37-146">String</span><span class="sxs-lookup"><span data-stu-id="32d37-146">String</span></span>|<span data-ttu-id="32d37-p106">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="32d37-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="32d37-149">groupTypes</span><span class="sxs-lookup"><span data-stu-id="32d37-149">groupTypes</span></span>|<span data-ttu-id="32d37-150">String collection</span><span class="sxs-lookup"><span data-stu-id="32d37-150">String collection</span></span>|<span data-ttu-id="32d37-151">指定组类型及其成员身份。</span><span class="sxs-lookup"><span data-stu-id="32d37-151">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="32d37-152">如果集合包含 **Unified**，则该组是 Microsoft 365 组，否则它就是一个安全组。</span><span class="sxs-lookup"><span data-stu-id="32d37-152">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="32d37-153">如果该集合包含 **DynamicMembership**，则该组具有动态成员身份；否则，成员身份是静态的。</span><span class="sxs-lookup"><span data-stu-id="32d37-153">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="32d37-154">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="32d37-154">mailEnabled</span></span>|<span data-ttu-id="32d37-155">布尔</span><span class="sxs-lookup"><span data-stu-id="32d37-155">Boolean</span></span>|<span data-ttu-id="32d37-156">指定是否为启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="32d37-156">Specifies whether the group is mail-enabled.</span></span>|
|<span data-ttu-id="32d37-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="32d37-157">mailNickname</span></span>|<span data-ttu-id="32d37-158">String</span><span class="sxs-lookup"><span data-stu-id="32d37-158">String</span></span>|<span data-ttu-id="32d37-p107">组的邮件别名。创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="32d37-p107">The mail alias for the group. This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="32d37-161">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="32d37-161">securityEnabled</span></span>|<span data-ttu-id="32d37-162">布尔</span><span class="sxs-lookup"><span data-stu-id="32d37-162">Boolean</span></span>|<span data-ttu-id="32d37-163">指定是否为安全组。</span><span class="sxs-lookup"><span data-stu-id="32d37-163">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="32d37-164">visibility</span><span class="sxs-lookup"><span data-stu-id="32d37-164">visibility</span></span>|<span data-ttu-id="32d37-165">String</span><span class="sxs-lookup"><span data-stu-id="32d37-165">String</span></span>|<span data-ttu-id="32d37-166">指定 Microsoft 365 组的可见性。</span><span class="sxs-lookup"><span data-stu-id="32d37-166">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="32d37-167">可能的是包括：**专用**、**公用** 或为空（解释为 **公用**）。</span><span class="sxs-lookup"><span data-stu-id="32d37-167">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="32d37-168">**注意：**</span><span class="sxs-lookup"><span data-stu-id="32d37-168">**Note:**</span></span>
>
> - <span data-ttu-id="32d37-169">可以通过在 **补丁请求中指定** 自动更新 **autoSubendalNewMembers** ，而不包括上表中其他属性。</span><span class="sxs-lookup"><span data-stu-id="32d37-169">You can update **allowExternalSenders** and **autoSubscribeNewMembers** by specifying them in their own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="32d37-p109">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅 [已知问题](/graph/known-issues#groups)。</span><span class="sxs-lookup"><span data-stu-id="32d37-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#groups) for examples.</span></span>
> - <span data-ttu-id="32d37-173">在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。</span><span class="sxs-lookup"><span data-stu-id="32d37-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>

## <a name="response"></a><span data-ttu-id="32d37-174">响应</span><span class="sxs-lookup"><span data-stu-id="32d37-174">Response</span></span>

<span data-ttu-id="32d37-175">如果成功， 此方法返回 `204 No Content` 响应代码 - 更新下列属性时除了 `200 OK` 响应代码：**allowEx在alSenders**、 **autoSubendNewMembers**， **HideFromAddressList**， **hideFromOutlookClients**， **isSubeendByMail**， **unseenCount**。</span><span class="sxs-lookup"><span data-stu-id="32d37-175">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="example"></a><span data-ttu-id="32d37-176">示例</span><span class="sxs-lookup"><span data-stu-id="32d37-176">Example</span></span>

<span data-ttu-id="32d37-177">以下示例演示如何更新组。</span><span class="sxs-lookup"><span data-stu-id="32d37-177">The following example shows how to update a group.</span></span>

### <a name="request"></a><span data-ttu-id="32d37-178">请求</span><span class="sxs-lookup"><span data-stu-id="32d37-178">Request</span></span>

<span data-ttu-id="32d37-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="32d37-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32d37-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="32d37-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
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
# <a name="c"></a>[<span data-ttu-id="32d37-181">C#</span><span class="sxs-lookup"><span data-stu-id="32d37-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32d37-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32d37-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32d37-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32d37-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32d37-184">Java</span><span class="sxs-lookup"><span data-stu-id="32d37-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32d37-185">响应</span><span class="sxs-lookup"><span data-stu-id="32d37-185">Response</span></span>

<span data-ttu-id="32d37-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="32d37-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
