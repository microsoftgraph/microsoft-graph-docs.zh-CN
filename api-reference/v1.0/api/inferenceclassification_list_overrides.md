# <a name="list-overrides"></a><span data-ttu-id="5ef15-101">列出替代</span><span class="sxs-lookup"><span data-stu-id="5ef15-101">List overrides</span></span>

<span data-ttu-id="5ef15-102">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="5ef15-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="5ef15-p101">每个替代均对应一个发件人的 SMTP 地址。最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="5ef15-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ef15-105">权限</span><span class="sxs-lookup"><span data-stu-id="5ef15-105">Permissions</span></span>
<span data-ttu-id="5ef15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5ef15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ef15-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ef15-108">Permission type</span></span>      | <span data-ttu-id="5ef15-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ef15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ef15-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ef15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ef15-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ef15-111">Mail.Read</span></span>    |
|<span data-ttu-id="5ef15-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ef15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ef15-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ef15-113">Mail.Read</span></span>    |
|<span data-ttu-id="5ef15-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ef15-114">Application</span></span> | <span data-ttu-id="5ef15-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5ef15-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ef15-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ef15-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="5ef15-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ef15-117">Request headers</span></span>
| <span data-ttu-id="5ef15-118">名称</span><span class="sxs-lookup"><span data-stu-id="5ef15-118">Name</span></span>       | <span data-ttu-id="5ef15-119">类型</span><span class="sxs-lookup"><span data-stu-id="5ef15-119">Type</span></span> | <span data-ttu-id="5ef15-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ef15-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ef15-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ef15-121">Authorization</span></span>  | <span data-ttu-id="5ef15-122">string</span><span class="sxs-lookup"><span data-stu-id="5ef15-122">string</span></span>  | <span data-ttu-id="5ef15-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ef15-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ef15-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ef15-125">Request body</span></span>
<span data-ttu-id="5ef15-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ef15-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ef15-127">响应</span><span class="sxs-lookup"><span data-stu-id="5ef15-127">Response</span></span>

<span data-ttu-id="5ef15-p104">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象集合。如果用户未设置任何替代，则返回空集合。</span><span class="sxs-lookup"><span data-stu-id="5ef15-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="5ef15-130">示例</span><span class="sxs-lookup"><span data-stu-id="5ef15-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ef15-131">请求</span><span class="sxs-lookup"><span data-stu-id="5ef15-131">Request</span></span>
<span data-ttu-id="5ef15-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ef15-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="5ef15-133">响应</span><span class="sxs-lookup"><span data-stu-id="5ef15-133">Response</span></span>
<span data-ttu-id="5ef15-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ef15-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->