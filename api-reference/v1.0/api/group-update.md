---
title: 更新组
description: 更新 group 对象的属性。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: adb66a65fa3c8612952b990e17922055d4d0984d
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036365"
---
# <a name="update-group"></a><span data-ttu-id="068eb-103">更新组</span><span class="sxs-lookup"><span data-stu-id="068eb-103">Update group</span></span>

<span data-ttu-id="068eb-104">更新 group 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="068eb-104">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="068eb-105">权限</span><span class="sxs-lookup"><span data-stu-id="068eb-105">Permissions</span></span>

<span data-ttu-id="068eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="068eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="068eb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="068eb-108">Permission type</span></span>      | <span data-ttu-id="068eb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="068eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="068eb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="068eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="068eb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="068eb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="068eb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="068eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="068eb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="068eb-113">Not supported.</span></span>    |
|<span data-ttu-id="068eb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="068eb-114">Application</span></span> | <span data-ttu-id="068eb-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="068eb-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="068eb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="068eb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="068eb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="068eb-117">Request headers</span></span>

| <span data-ttu-id="068eb-118">名称</span><span class="sxs-lookup"><span data-stu-id="068eb-118">Name</span></span>       | <span data-ttu-id="068eb-119">类型</span><span class="sxs-lookup"><span data-stu-id="068eb-119">Type</span></span> | <span data-ttu-id="068eb-120">说明</span><span class="sxs-lookup"><span data-stu-id="068eb-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="068eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="068eb-121">Authorization</span></span>  | <span data-ttu-id="068eb-122">string</span><span class="sxs-lookup"><span data-stu-id="068eb-122">string</span></span>  | <span data-ttu-id="068eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="068eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="068eb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="068eb-125">Request body</span></span>

<span data-ttu-id="068eb-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="068eb-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="068eb-129">属性</span><span class="sxs-lookup"><span data-stu-id="068eb-129">Property</span></span>   | <span data-ttu-id="068eb-130">类型</span><span class="sxs-lookup"><span data-stu-id="068eb-130">Type</span></span> |<span data-ttu-id="068eb-131">说明</span><span class="sxs-lookup"><span data-stu-id="068eb-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="068eb-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="068eb-132">allowExternalSenders</span></span>|<span data-ttu-id="068eb-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="068eb-133">Boolean</span></span>|<span data-ttu-id="068eb-p104">默认为 **false**。指明组织外部人员能否向群组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="068eb-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="068eb-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="068eb-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="068eb-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="068eb-137">Boolean</span></span>|<span data-ttu-id="068eb-p105">默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="068eb-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="068eb-140">description</span><span class="sxs-lookup"><span data-stu-id="068eb-140">description</span></span>|<span data-ttu-id="068eb-141">String</span><span class="sxs-lookup"><span data-stu-id="068eb-141">String</span></span>|<span data-ttu-id="068eb-142">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="068eb-142">An optional description for the group.</span></span> |
|<span data-ttu-id="068eb-143">displayName</span><span class="sxs-lookup"><span data-stu-id="068eb-143">displayName</span></span>|<span data-ttu-id="068eb-144">String</span><span class="sxs-lookup"><span data-stu-id="068eb-144">String</span></span>|<span data-ttu-id="068eb-p106">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。</span><span class="sxs-lookup"><span data-stu-id="068eb-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span> |
|<span data-ttu-id="068eb-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="068eb-147">groupTypes</span></span>|<span data-ttu-id="068eb-148">String collection</span><span class="sxs-lookup"><span data-stu-id="068eb-148">String collection</span></span>|<span data-ttu-id="068eb-149">指定组类型及其成员身份。</span><span class="sxs-lookup"><span data-stu-id="068eb-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="068eb-150">如果集合包含 **Unified**，则该组是 Office 365 组，否则它是一个安全组。</span><span class="sxs-lookup"><span data-stu-id="068eb-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="068eb-151">如果该集合包含 **DynamicMembership**，则该组具有动态成员身份；否则，成员身份是静态的。</span><span class="sxs-lookup"><span data-stu-id="068eb-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="068eb-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="068eb-152">mailEnabled</span></span>|<span data-ttu-id="068eb-153">布尔</span><span class="sxs-lookup"><span data-stu-id="068eb-153">Boolean</span></span>|<span data-ttu-id="068eb-154">指定是否为启用邮件的组。</span><span class="sxs-lookup"><span data-stu-id="068eb-154">Specifies whether the group is mail-enabled.</span></span>|
|<span data-ttu-id="068eb-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="068eb-155">mailNickname</span></span>|<span data-ttu-id="068eb-156">String</span><span class="sxs-lookup"><span data-stu-id="068eb-156">String</span></span>|<span data-ttu-id="068eb-157">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="068eb-157">The mail alias for the group.</span></span> <span data-ttu-id="068eb-158">创建组时必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="068eb-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="068eb-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="068eb-159">securityEnabled</span></span>|<span data-ttu-id="068eb-160">布尔</span><span class="sxs-lookup"><span data-stu-id="068eb-160">Boolean</span></span>|<span data-ttu-id="068eb-161">指定是否为安全组。</span><span class="sxs-lookup"><span data-stu-id="068eb-161">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="068eb-162">visibility</span><span class="sxs-lookup"><span data-stu-id="068eb-162">visibility</span></span>|<span data-ttu-id="068eb-163">String</span><span class="sxs-lookup"><span data-stu-id="068eb-163">String</span></span>|<span data-ttu-id="068eb-164">指定 Office 365 组的可见性。</span><span class="sxs-lookup"><span data-stu-id="068eb-164">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="068eb-165">可能的是包括：**专用**、**公用**或为空（解释为**公用**）。</span><span class="sxs-lookup"><span data-stu-id="068eb-165">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="068eb-166">**注意：**</span><span class="sxs-lookup"><span data-stu-id="068eb-166">**Note:**</span></span>
>
> - <span data-ttu-id="068eb-167">可更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="068eb-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request,without including the other properties in the table above.</span></span>
> - <span data-ttu-id="068eb-p109">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="068eb-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="068eb-171">在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](https://docs.microsoft.com/zh-CN/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。</span><span class="sxs-lookup"><span data-stu-id="068eb-171">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>


## <a name="response"></a><span data-ttu-id="068eb-172">响应</span><span class="sxs-lookup"><span data-stu-id="068eb-172">Response</span></span>

<span data-ttu-id="068eb-173">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="068eb-173">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="068eb-174">示例</span><span class="sxs-lookup"><span data-stu-id="068eb-174">Example</span></span>

<span data-ttu-id="068eb-175">以下示例演示如何创建组。</span><span class="sxs-lookup"><span data-stu-id="068eb-175">The following example shows how to create a calculated field.</span></span>

### <a name="request"></a><span data-ttu-id="068eb-176">请求</span><span class="sxs-lookup"><span data-stu-id="068eb-176">Request</span></span>

<span data-ttu-id="068eb-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="068eb-177">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="068eb-178">响应</span><span class="sxs-lookup"><span data-stu-id="068eb-178">Response</span></span>

<span data-ttu-id="068eb-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="068eb-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="068eb-180">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="068eb-180">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="068eb-181">C#</span><span class="sxs-lookup"><span data-stu-id="068eb-181">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="068eb-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="068eb-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
