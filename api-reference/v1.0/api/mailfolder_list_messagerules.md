# <a name="list-rules"></a><span data-ttu-id="683c2-101">列出规则</span><span class="sxs-lookup"><span data-stu-id="683c2-101">List rules</span></span>

<span data-ttu-id="683c2-102">获取为用户收件箱定义的所有 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="683c2-102">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="683c2-103">权限</span><span class="sxs-lookup"><span data-stu-id="683c2-103">Permissions</span></span>
<span data-ttu-id="683c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="683c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="683c2-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="683c2-106">Permission type</span></span>      | <span data-ttu-id="683c2-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="683c2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="683c2-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="683c2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="683c2-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="683c2-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="683c2-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="683c2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="683c2-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="683c2-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="683c2-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="683c2-112">Application</span></span> | <span data-ttu-id="683c2-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="683c2-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="683c2-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="683c2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="683c2-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="683c2-115">Optional query parameters</span></span>
<span data-ttu-id="683c2-116">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="683c2-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="683c2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="683c2-117">Request headers</span></span>
| <span data-ttu-id="683c2-118">名称</span><span class="sxs-lookup"><span data-stu-id="683c2-118">Name</span></span>       | <span data-ttu-id="683c2-119">类型</span><span class="sxs-lookup"><span data-stu-id="683c2-119">Type</span></span> | <span data-ttu-id="683c2-120">说明</span><span class="sxs-lookup"><span data-stu-id="683c2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="683c2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="683c2-121">Authorization</span></span>  | <span data-ttu-id="683c2-122">string</span><span class="sxs-lookup"><span data-stu-id="683c2-122">string</span></span>  | <span data-ttu-id="683c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="683c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="683c2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="683c2-125">Request body</span></span>
<span data-ttu-id="683c2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="683c2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="683c2-127">响应</span><span class="sxs-lookup"><span data-stu-id="683c2-127">Response</span></span>
<span data-ttu-id="683c2-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [messageRule](../resources/messagerule.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="683c2-128">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="683c2-129">示例</span><span class="sxs-lookup"><span data-stu-id="683c2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="683c2-130">请求</span><span class="sxs-lookup"><span data-stu-id="683c2-130">Request</span></span>
<span data-ttu-id="683c2-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="683c2-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
```
##### <a name="response"></a><span data-ttu-id="683c2-132">响应</span><span class="sxs-lookup"><span data-stu-id="683c2-132">Response</span></span>
<span data-ttu-id="683c2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="683c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
      "id":"AQAAAJ5dZqA=",
      "displayName":"From partner",
      "sequence":2,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "senderContains":[
          "ADELE"
        ]
      },
      "actions":{
        "stopProcessingRules":true,
        "forwardTo":[
          {
            "emailAddress":{
              "name":"Alex Wilbur",
              "address":"AlexW@contoso.onmicrosoft.com"
            }
          }
        ]
      }
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
