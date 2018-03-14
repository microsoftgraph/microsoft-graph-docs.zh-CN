# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="a11e9-101">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a11e9-101">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="a11e9-102">更新 [groupLifecyclePolicy 资源类型](../resources/grouplifecyclepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a11e9-102">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a11e9-103">权限</span><span class="sxs-lookup"><span data-stu-id="a11e9-103">Permissions</span></span>

<span data-ttu-id="a11e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a11e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 
|<span data-ttu-id="a11e9-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="a11e9-106">Permission type</span></span>      | <span data-ttu-id="a11e9-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a11e9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a11e9-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a11e9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a11e9-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a11e9-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a11e9-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a11e9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a11e9-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a11e9-111">Not supported.</span></span>    |
|<span data-ttu-id="a11e9-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="a11e9-112">Application</span></span> | <span data-ttu-id="a11e9-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a11e9-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a11e9-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a11e9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a11e9-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a11e9-115">Optional request headers</span></span>
| <span data-ttu-id="a11e9-116">名称</span><span class="sxs-lookup"><span data-stu-id="a11e9-116">Name</span></span> | <span data-ttu-id="a11e9-117">说明</span><span class="sxs-lookup"><span data-stu-id="a11e9-117">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="a11e9-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a11e9-118">Authorization</span></span> | <span data-ttu-id="a11e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a11e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a11e9-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a11e9-121">Content-Type</span></span>  | <span data-ttu-id="a11e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a11e9-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a11e9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a11e9-123">Request body</span></span>

<span data-ttu-id="a11e9-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a11e9-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a11e9-125">未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a11e9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a11e9-126">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="a11e9-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a11e9-127">属性</span><span class="sxs-lookup"><span data-stu-id="a11e9-127">Property</span></span> | <span data-ttu-id="a11e9-128">类型</span><span class="sxs-lookup"><span data-stu-id="a11e9-128">Type</span></span> | <span data-ttu-id="a11e9-129">说明</span><span class="sxs-lookup"><span data-stu-id="a11e9-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a11e9-130">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a11e9-130">alternateNotificationEmails</span></span>|<span data-ttu-id="a11e9-131">String</span><span class="sxs-lookup"><span data-stu-id="a11e9-131">String</span></span>| <span data-ttu-id="a11e9-132">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="a11e9-132">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="a11e9-133">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a11e9-133">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="a11e9-134">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="a11e9-134">groupLifetimeInDays</span></span>|<span data-ttu-id="a11e9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a11e9-135">Int32</span></span>| <span data-ttu-id="a11e9-136">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="a11e9-136">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="a11e9-137">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="a11e9-137">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="a11e9-138">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="a11e9-138">managedGroupTypes</span></span>|<span data-ttu-id="a11e9-139">String</span><span class="sxs-lookup"><span data-stu-id="a11e9-139">String</span></span>| <span data-ttu-id="a11e9-140">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="a11e9-140">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="a11e9-141">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="a11e9-141">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="a11e9-142">响应</span><span class="sxs-lookup"><span data-stu-id="a11e9-142">Response</span></span>

<span data-ttu-id="a11e9-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a11e9-143">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a11e9-144">示例</span><span class="sxs-lookup"><span data-stu-id="a11e9-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a11e9-145">请求</span><span class="sxs-lookup"><span data-stu-id="a11e9-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="a11e9-146">响应</span><span class="sxs-lookup"><span data-stu-id="a11e9-146">Response</span></span>
<span data-ttu-id="a11e9-147">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a11e9-147">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->