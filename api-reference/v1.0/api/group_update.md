# <a name="update-group"></a><span data-ttu-id="a4b00-101">更新组</span><span class="sxs-lookup"><span data-stu-id="a4b00-101">Update group</span></span>
<span data-ttu-id="a4b00-102">更新 group 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4b00-102">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4b00-103">权限</span><span class="sxs-lookup"><span data-stu-id="a4b00-103">Permissions</span></span>
<span data-ttu-id="a4b00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a4b00-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4b00-106">Permission type</span></span>      | <span data-ttu-id="a4b00-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4b00-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4b00-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4b00-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a4b00-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b00-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4b00-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4b00-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4b00-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4b00-111">Not supported.</span></span>    |
|<span data-ttu-id="a4b00-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4b00-112">Application</span></span> | <span data-ttu-id="a4b00-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b00-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4b00-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4b00-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a4b00-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4b00-115">Request headers</span></span>

| <span data-ttu-id="a4b00-116">名称</span><span class="sxs-lookup"><span data-stu-id="a4b00-116">Name</span></span>       | <span data-ttu-id="a4b00-117">类型</span><span class="sxs-lookup"><span data-stu-id="a4b00-117">Type</span></span> | <span data-ttu-id="a4b00-118">说明</span><span class="sxs-lookup"><span data-stu-id="a4b00-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4b00-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4b00-119">Authorization</span></span>  | <span data-ttu-id="a4b00-120">string</span><span class="sxs-lookup"><span data-stu-id="a4b00-120">string</span></span>  | <span data-ttu-id="a4b00-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4b00-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4b00-123">Request body</span></span>

<span data-ttu-id="a4b00-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a4b00-127">属性</span><span class="sxs-lookup"><span data-stu-id="a4b00-127">Property</span></span>     | <span data-ttu-id="a4b00-128">类型</span><span class="sxs-lookup"><span data-stu-id="a4b00-128">Type</span></span>   |<span data-ttu-id="a4b00-129">说明</span><span class="sxs-lookup"><span data-stu-id="a4b00-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4b00-130">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="a4b00-130">allowExternalSenders</span></span>|<span data-ttu-id="a4b00-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4b00-131">Boolean</span></span>|<span data-ttu-id="a4b00-p104">默认为 **false**。指明组织外部人员能否向群组发送邮件。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="a4b00-134">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="a4b00-134">autoSubscribeNewMembers</span></span>|<span data-ttu-id="a4b00-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4b00-135">Boolean</span></span>|<span data-ttu-id="a4b00-p105">默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="a4b00-138">description</span><span class="sxs-lookup"><span data-stu-id="a4b00-138">description</span></span>|<span data-ttu-id="a4b00-139">String</span><span class="sxs-lookup"><span data-stu-id="a4b00-139">String</span></span>|<span data-ttu-id="a4b00-140">可选的组说明。</span><span class="sxs-lookup"><span data-stu-id="a4b00-140">An optional description for the group.</span></span> |
|<span data-ttu-id="a4b00-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a4b00-141">displayName</span></span>|<span data-ttu-id="a4b00-142">String</span><span class="sxs-lookup"><span data-stu-id="a4b00-142">String</span></span>|<span data-ttu-id="a4b00-p106">组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="a4b00-146">groupTypes</span><span class="sxs-lookup"><span data-stu-id="a4b00-146">groupTypes</span></span>|<span data-ttu-id="a4b00-147">String collection</span><span class="sxs-lookup"><span data-stu-id="a4b00-147">String collection</span></span>|<span data-ttu-id="a4b00-p107">指定要创建的组的类型。可取值为 **Unified**（要创建 Office 365 组）或 **DynamicMembership**（要创建动态组）。对于其他所有组类型（如启用安全机制的组和启用电子邮件的安全组），请勿设置此属性。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p107">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="a4b00-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="a4b00-151">mailEnabled</span></span>|<span data-ttu-id="a4b00-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4b00-152">Boolean</span></span>|<span data-ttu-id="a4b00-p108">指定该组是否启用邮件。如果 **securityEnabled** 属性也为 **true**，则该组是已启用邮件的安全组；否则是 Microsoft Exchange 通讯组。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p108">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="a4b00-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a4b00-155">mailNickname</span></span>|<span data-ttu-id="a4b00-156">String</span><span class="sxs-lookup"><span data-stu-id="a4b00-156">String</span></span>|<span data-ttu-id="a4b00-p109">组的邮件别名。创建组时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p109">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="a4b00-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="a4b00-160">securityEnabled</span></span>|<span data-ttu-id="a4b00-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4b00-161">Boolean</span></span>|<span data-ttu-id="a4b00-p110">指定是否为安全组。如果 **mailEnabled** 属性也为 true，则为启用邮件的安全组；否则为安全组。对于 Office 365 组，此属性必须为 **false**。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p110">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="a4b00-166">visibility</span><span class="sxs-lookup"><span data-stu-id="a4b00-166">visibility</span></span>|<span data-ttu-id="a4b00-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4b00-167">Boolean</span></span>|<span data-ttu-id="a4b00-p111">指定 Office 365 组的可见性。可能的值是：**专用**、**公用**或空（解释为**公用**）。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p111">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="a4b00-170">**注意**</span><span class="sxs-lookup"><span data-stu-id="a4b00-170">**Note**</span></span>

- <span data-ttu-id="a4b00-171">可以更新 **autoSubscribeNewMembers**，方法是在其自身的 PATCH 请求中指定它，而不包括上表中的其他属性。</span><span class="sxs-lookup"><span data-stu-id="a4b00-171">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="a4b00-p112">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p112">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="a4b00-175">响应</span><span class="sxs-lookup"><span data-stu-id="a4b00-175">Response</span></span>
<span data-ttu-id="a4b00-176">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4b00-176">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4b00-177">示例</span><span class="sxs-lookup"><span data-stu-id="a4b00-177">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a4b00-178">请求</span><span class="sxs-lookup"><span data-stu-id="a4b00-178">Request</span></span>
<span data-ttu-id="a4b00-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a4b00-179">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="a4b00-180">响应</span><span class="sxs-lookup"><span data-stu-id="a4b00-180">Response</span></span>
<span data-ttu-id="a4b00-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a4b00-181">The following is an example of the response.</span></span>
><span data-ttu-id="a4b00-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a4b00-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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