# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="71f48-101">创建 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="71f48-101">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="71f48-102">新建 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="71f48-102">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71f48-103">权限</span><span class="sxs-lookup"><span data-stu-id="71f48-103">Permissions</span></span>

<span data-ttu-id="71f48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="71f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71f48-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="71f48-106">Permission type</span></span>      | <span data-ttu-id="71f48-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71f48-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f48-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71f48-108">Delegated (work or school account)</span></span> | <span data-ttu-id="71f48-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f48-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="71f48-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71f48-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71f48-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="71f48-111">Not supported.</span></span>    |
|<span data-ttu-id="71f48-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="71f48-112">Application</span></span> | <span data-ttu-id="71f48-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f48-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71f48-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71f48-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="71f48-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="71f48-115">Request headers</span></span>

| <span data-ttu-id="71f48-116">名称</span><span class="sxs-lookup"><span data-stu-id="71f48-116">Name</span></span> | <span data-ttu-id="71f48-117">说明</span><span class="sxs-lookup"><span data-stu-id="71f48-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="71f48-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f48-118">Authorization</span></span> | <span data-ttu-id="71f48-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71f48-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71f48-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71f48-121">Content-Type</span></span>  | <span data-ttu-id="71f48-122">application/json</span><span class="sxs-lookup"><span data-stu-id="71f48-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="71f48-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="71f48-123">Request body</span></span>
<span data-ttu-id="71f48-124">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f48-124">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71f48-125">响应</span><span class="sxs-lookup"><span data-stu-id="71f48-125">Response</span></span>

<span data-ttu-id="71f48-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71f48-126">If successful, this method returns a `201 Created` response code and [profilePhoto](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f48-127">示例</span><span class="sxs-lookup"><span data-stu-id="71f48-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71f48-128">请求</span><span class="sxs-lookup"><span data-stu-id="71f48-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="71f48-129">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f48-129">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71f48-130">响应</span><span class="sxs-lookup"><span data-stu-id="71f48-130">Response</span></span>

<span data-ttu-id="71f48-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71f48-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->