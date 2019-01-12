---
title: 更新组
description: 更新 group 对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f1f86067771a4732c8839f48bc02dd3edd15c19b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915233"
---
# <a name="update-group"></a><span data-ttu-id="8b6d9-103">更新组</span><span class="sxs-lookup"><span data-stu-id="8b6d9-103">Update group</span></span>

> <span data-ttu-id="8b6d9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b6d9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b6d9-106">更新[组](../resources/group.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-106">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b6d9-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b6d9-107">Permissions</span></span>

<span data-ttu-id="8b6d9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b6d9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b6d9-110">Permission type</span></span>      | <span data-ttu-id="8b6d9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b6d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b6d9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b6d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b6d9-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b6d9-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b6d9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b6d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b6d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-115">Not supported.</span></span>    |
|<span data-ttu-id="8b6d9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b6d9-116">Application</span></span> | <span data-ttu-id="8b6d9-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b6d9-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b6d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b6d9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b6d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b6d9-119">Request headers</span></span>

| <span data-ttu-id="8b6d9-120">名称</span><span class="sxs-lookup"><span data-stu-id="8b6d9-120">Name</span></span>       | <span data-ttu-id="8b6d9-121">类型</span><span class="sxs-lookup"><span data-stu-id="8b6d9-121">Type</span></span> | <span data-ttu-id="8b6d9-122">说明</span><span class="sxs-lookup"><span data-stu-id="8b6d9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b6d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b6d9-123">Authorization</span></span>  | <span data-ttu-id="8b6d9-124">string</span><span class="sxs-lookup"><span data-stu-id="8b6d9-124">string</span></span>  | <span data-ttu-id="8b6d9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b6d9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b6d9-127">Request body</span></span>

<span data-ttu-id="8b6d9-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8b6d9-131">属性</span><span class="sxs-lookup"><span data-stu-id="8b6d9-131">Property</span></span>   | <span data-ttu-id="8b6d9-132">类型</span><span class="sxs-lookup"><span data-stu-id="8b6d9-132">Type</span></span> |<span data-ttu-id="8b6d9-133">说明</span><span class="sxs-lookup"><span data-stu-id="8b6d9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b6d9-134">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="8b6d9-134">allowExternalSenders</span></span>|<span data-ttu-id="8b6d9-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b6d9-135">Boolean</span></span>|<span data-ttu-id="8b6d9-p105">默认为 **false**。指明组织外部人员能否向群组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p105">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="8b6d9-138">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="8b6d9-138">autoSubscribeNewMembers</span></span>|<span data-ttu-id="8b6d9-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b6d9-139">Boolean</span></span>|<span data-ttu-id="8b6d9-p106">默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p106">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="8b6d9-142">说明</span><span class="sxs-lookup"><span data-stu-id="8b6d9-142">description</span></span>|<span data-ttu-id="8b6d9-143">String</span><span class="sxs-lookup"><span data-stu-id="8b6d9-143">String</span></span>|<span data-ttu-id="8b6d9-144">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-144">An optional description for the group.</span></span> |
|<span data-ttu-id="8b6d9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8b6d9-145">displayName</span></span>|<span data-ttu-id="8b6d9-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8b6d9-146">String</span></span>|<span data-ttu-id="8b6d9-p107">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p107">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="8b6d9-150">groupTypes</span><span class="sxs-lookup"><span data-stu-id="8b6d9-150">groupTypes</span></span>|<span data-ttu-id="8b6d9-151">String collection</span><span class="sxs-lookup"><span data-stu-id="8b6d9-151">String collection</span></span>|<span data-ttu-id="8b6d9-p108">指定要创建的组的类型。可取值为 **Unified**（要创建 Office 365 组）或 **DynamicMembership**（要创建动态组）。对于其他所有组类型（如启用安全机制的组和启用电子邮件的安全组），请勿设置此属性。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p108">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="8b6d9-155">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="8b6d9-155">mailEnabled</span></span>|<span data-ttu-id="8b6d9-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b6d9-156">Boolean</span></span>|<span data-ttu-id="8b6d9-p109">指定该组是否启用邮件。如果 **securityEnabled** 属性也为 **true**，则该组是已启用邮件的安全组；否则是 Microsoft Exchange 通讯组。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p109">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="8b6d9-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8b6d9-159">mailNickname</span></span>|<span data-ttu-id="8b6d9-160">字符串</span><span class="sxs-lookup"><span data-stu-id="8b6d9-160">String</span></span>|<span data-ttu-id="8b6d9-p110">组的邮件别名。创建组时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p110">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="8b6d9-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="8b6d9-164">securityEnabled</span></span>|<span data-ttu-id="8b6d9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b6d9-165">Boolean</span></span>|<span data-ttu-id="8b6d9-p111">指定是否为安全组。如果 **mailEnabled** 属性也为 true，则为启用邮件的安全组；否则为安全组。对于 Office 365 组，此属性必须为 **false**。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p111">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="8b6d9-170">visibility</span><span class="sxs-lookup"><span data-stu-id="8b6d9-170">visibility</span></span>|<span data-ttu-id="8b6d9-171">String</span><span class="sxs-lookup"><span data-stu-id="8b6d9-171">String</span></span>|<span data-ttu-id="8b6d9-p112">指定 Office 365 组的可见性。可能的值是：**专用**、**公用**或空（解释为**公用**）。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p112">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="8b6d9-174">由于**group**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**组**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-174">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="8b6d9-175">**注意：**</span><span class="sxs-lookup"><span data-stu-id="8b6d9-175">**Note:**</span></span>
>
> - <span data-ttu-id="8b6d9-176">可以更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-176">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="8b6d9-p113">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-p113">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="8b6d9-180">响应</span><span class="sxs-lookup"><span data-stu-id="8b6d9-180">Response</span></span>

<span data-ttu-id="8b6d9-181">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-181">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8b6d9-182">示例</span><span class="sxs-lookup"><span data-stu-id="8b6d9-182">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8b6d9-183">请求</span><span class="sxs-lookup"><span data-stu-id="8b6d9-183">Request</span></span>

<span data-ttu-id="8b6d9-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-184">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8b6d9-185">响应</span><span class="sxs-lookup"><span data-stu-id="8b6d9-185">Response</span></span>

<span data-ttu-id="8b6d9-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8b6d9-186">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="8b6d9-187">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8b6d9-187">See also</span></span>

- [<span data-ttu-id="8b6d9-188">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="8b6d9-188">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8b6d9-189">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="8b6d9-189">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="8b6d9-190">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="8b6d9-190">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
