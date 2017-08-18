# <a name="update-group"></a><span data-ttu-id="093a4-101">更新组</span><span class="sxs-lookup"><span data-stu-id="093a4-101">Update group</span></span>

<span data-ttu-id="093a4-102">更新组对象的属性。</span><span class="sxs-lookup"><span data-stu-id="093a4-102">Update the properties of a group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="093a4-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="093a4-103">Prerequisites</span></span>
<span data-ttu-id="093a4-104">要执行此 API，需要以下**范围**：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="093a4-104">The following **scope** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="093a4-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="093a4-105">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="093a4-106">请求标头</span><span class="sxs-lookup"><span data-stu-id="093a4-106">Request headers</span></span>

| <span data-ttu-id="093a4-107">名称</span><span class="sxs-lookup"><span data-stu-id="093a4-107">Name</span></span>       | <span data-ttu-id="093a4-108">类型</span><span class="sxs-lookup"><span data-stu-id="093a4-108">Type</span></span> | <span data-ttu-id="093a4-109">说明</span><span class="sxs-lookup"><span data-stu-id="093a4-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="093a4-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="093a4-110">Authorization</span></span>  | <span data-ttu-id="093a4-111">string</span><span class="sxs-lookup"><span data-stu-id="093a4-111">string</span></span>  | <span data-ttu-id="093a4-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="093a4-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="093a4-114">请求正文</span><span class="sxs-lookup"><span data-stu-id="093a4-114">Request body</span></span>

<span data-ttu-id="093a4-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="093a4-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="093a4-118">属性</span><span class="sxs-lookup"><span data-stu-id="093a4-118">Property</span></span>     | <span data-ttu-id="093a4-119">类型</span><span class="sxs-lookup"><span data-stu-id="093a4-119">Type</span></span>   |<span data-ttu-id="093a4-120">说明</span><span class="sxs-lookup"><span data-stu-id="093a4-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="093a4-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="093a4-121">autoSubscribeNewMembers</span></span>|<span data-ttu-id="093a4-122">布尔</span><span class="sxs-lookup"><span data-stu-id="093a4-122">Boolean</span></span>|<span data-ttu-id="093a4-p103">默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="093a4-p103">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="093a4-125">说明</span><span class="sxs-lookup"><span data-stu-id="093a4-125">description</span></span>|<span data-ttu-id="093a4-126">String</span><span class="sxs-lookup"><span data-stu-id="093a4-126">String</span></span>|<span data-ttu-id="093a4-127">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="093a4-127">An optional description for the group.</span></span> |
|<span data-ttu-id="093a4-128">displayName</span><span class="sxs-lookup"><span data-stu-id="093a4-128">displayName</span></span>|<span data-ttu-id="093a4-129">String</span><span class="sxs-lookup"><span data-stu-id="093a4-129">String</span></span>|<span data-ttu-id="093a4-p104">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="093a4-p104">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="093a4-133">groupTypes</span><span class="sxs-lookup"><span data-stu-id="093a4-133">groupTypes</span></span>|<span data-ttu-id="093a4-134">String collection</span><span class="sxs-lookup"><span data-stu-id="093a4-134">String collection</span></span>|<span data-ttu-id="093a4-p105">指定要创建的组的类型。可取值为 **Unified**（要创建 Office 365 组）或 **DynamicMembership**（要创建动态组）。对于其他所有组类型（如启用安全机制的组和启用电子邮件的安全组），请勿设置此属性。</span><span class="sxs-lookup"><span data-stu-id="093a4-p105">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="093a4-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="093a4-138">mailEnabled</span></span>|<span data-ttu-id="093a4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="093a4-139">Boolean</span></span>|<span data-ttu-id="093a4-p106">指定该组是否启用邮件。如果 **securityEnabled** 属性也为 **true**，则该组是已启用邮件的安全组；否则是 Microsoft Exchange 通讯组。</span><span class="sxs-lookup"><span data-stu-id="093a4-p106">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="093a4-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="093a4-142">mailNickname</span></span>|<span data-ttu-id="093a4-143">String</span><span class="sxs-lookup"><span data-stu-id="093a4-143">String</span></span>|<span data-ttu-id="093a4-p107">组的邮件别名。创建组时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="093a4-p107">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="093a4-147">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="093a4-147">securityEnabled</span></span>|<span data-ttu-id="093a4-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="093a4-148">Boolean</span></span>|<span data-ttu-id="093a4-p108">指定是否为安全组。如果 **mailEnabled** 属性也为 true，则为启用邮件的安全组；否则为安全组。对于 Office 365 组，此属性必须为 **false**。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="093a4-p108">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="093a4-153">visibility</span><span class="sxs-lookup"><span data-stu-id="093a4-153">visibility</span></span>|<span data-ttu-id="093a4-154">布尔</span><span class="sxs-lookup"><span data-stu-id="093a4-154">Boolean</span></span>|<span data-ttu-id="093a4-p109">指定 Office 365 组的可见性。可能的值是：**Private**、**Public** 或空（解释为 **Public**）。</span><span class="sxs-lookup"><span data-stu-id="093a4-p109">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="093a4-157">**注意**</span><span class="sxs-lookup"><span data-stu-id="093a4-157">**Note**</span></span>

- <span data-ttu-id="093a4-158">可以更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="093a4-158">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="093a4-p110">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="093a4-p110">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="093a4-162">响应</span><span class="sxs-lookup"><span data-stu-id="093a4-162">Response</span></span>

<span data-ttu-id="093a4-163">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="093a4-163">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="093a4-164">示例</span><span class="sxs-lookup"><span data-stu-id="093a4-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="093a4-165">请求</span><span class="sxs-lookup"><span data-stu-id="093a4-165">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="093a4-166">响应</span><span class="sxs-lookup"><span data-stu-id="093a4-166">Response</span></span>

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
  "tocPath": ""
}-->