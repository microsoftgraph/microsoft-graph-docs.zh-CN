# <a name="get-group"></a><span data-ttu-id="e3e8e-101">获取组</span><span class="sxs-lookup"><span data-stu-id="e3e8e-101">Get group</span></span>

<span data-ttu-id="e3e8e-102">检索与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-102">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="e3e8e-103">**注意：**如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="e3e8e-104">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3e8e-105">权限</span><span class="sxs-lookup"><span data-stu-id="e3e8e-105">Permissions</span></span>
<span data-ttu-id="e3e8e-106">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="e3e8e-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e3e8e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3e8e-108">Permission type</span></span>      | <span data-ttu-id="e3e8e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3e8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3e8e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3e8e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3e8e-111">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3e8e-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="e3e8e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3e8e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e3e8e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-113">Not supported.</span></span>  |
|<span data-ttu-id="e3e8e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3e8e-114">Application</span></span> | <span data-ttu-id="e3e8e-115">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3e8e-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e3e8e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3e8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="e3e8e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3e8e-117">Request headers</span></span>
| <span data-ttu-id="e3e8e-118">标头</span><span class="sxs-lookup"><span data-stu-id="e3e8e-118">Header</span></span>       | <span data-ttu-id="e3e8e-119">值</span><span class="sxs-lookup"><span data-stu-id="e3e8e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3e8e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e8e-120">Authorization</span></span>  | <span data-ttu-id="e3e8e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3e8e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3e8e-123">Request body</span></span>
<span data-ttu-id="e3e8e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e3e8e-125">响应</span><span class="sxs-lookup"><span data-stu-id="e3e8e-125">Response</span></span>
<span data-ttu-id="e3e8e-126">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-126">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3e8e-127">示例</span><span class="sxs-lookup"><span data-stu-id="e3e8e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3e8e-128">请求</span><span class="sxs-lookup"><span data-stu-id="e3e8e-128">Request</span></span>
<span data-ttu-id="e3e8e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="e3e8e-130">响应</span><span class="sxs-lookup"><span data-stu-id="e3e8e-130">Response</span></span>
<span data-ttu-id="e3e8e-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-131">The following is an example of the response.</span></span> 

><span data-ttu-id="e3e8e-p104">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e3e8e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->