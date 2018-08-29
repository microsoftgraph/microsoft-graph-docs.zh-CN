# <a name="message-move"></a><span data-ttu-id="271c7-101">消息：移动</span><span class="sxs-lookup"><span data-stu-id="271c7-101">message: move</span></span>

<span data-ttu-id="271c7-102">将消息移动至文件夹。</span><span class="sxs-lookup"><span data-stu-id="271c7-102">Move a DriveItem to a new folder</span></span> <span data-ttu-id="271c7-103">这便在目标文件夹中创建了新消息的副本，并删除原始消息。</span><span class="sxs-lookup"><span data-stu-id="271c7-103">Move the message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="271c7-104">权限</span><span class="sxs-lookup"><span data-stu-id="271c7-104">Permissions</span></span>

<span data-ttu-id="271c7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="271c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="271c7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="271c7-107">Permission type</span></span> | <span data-ttu-id="271c7-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="271c7-108">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="271c7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="271c7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="271c7-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="271c7-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="271c7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="271c7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="271c7-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="271c7-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="271c7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="271c7-113">Application</span></span> | <span data-ttu-id="271c7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="271c7-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="271c7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="271c7-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="271c7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="271c7-116">Request headers</span></span>

| <span data-ttu-id="271c7-117">标头</span><span class="sxs-lookup"><span data-stu-id="271c7-117">Header</span></span> | <span data-ttu-id="271c7-118">值</span><span class="sxs-lookup"><span data-stu-id="271c7-118">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="271c7-119">授权</span><span class="sxs-lookup"><span data-stu-id="271c7-119">Authorization</span></span> | <span data-ttu-id="271c7-120">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="271c7-120"></span></span> <span data-ttu-id="271c7-121">必需。</span><span class="sxs-lookup"><span data-stu-id="271c7-121">Required.</span></span> |
| <span data-ttu-id="271c7-122">内容类型</span><span class="sxs-lookup"><span data-stu-id="271c7-122">Content-Type</span></span> | <span data-ttu-id="271c7-123">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="271c7-123"></span></span> <span data-ttu-id="271c7-124">必需。</span><span class="sxs-lookup"><span data-stu-id="271c7-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="271c7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="271c7-125">Request body</span></span>

<span data-ttu-id="271c7-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="271c7-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="271c7-127">参数</span><span class="sxs-lookup"><span data-stu-id="271c7-127">Parameter</span></span>   | <span data-ttu-id="271c7-128">类型</span><span class="sxs-lookup"><span data-stu-id="271c7-128">Type</span></span> |<span data-ttu-id="271c7-129">说明</span><span class="sxs-lookup"><span data-stu-id="271c7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="271c7-130">destinationId</span><span class="sxs-lookup"><span data-stu-id="271c7-130">destinationId</span></span>|<span data-ttu-id="271c7-131">字符串</span><span class="sxs-lookup"><span data-stu-id="271c7-131">String</span></span>|<span data-ttu-id="271c7-132">目标文件夹 ID，或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="271c7-132">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="271c7-133">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md) 。</span><span class="sxs-lookup"><span data-stu-id="271c7-133">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="271c7-134">响应</span><span class="sxs-lookup"><span data-stu-id="271c7-134">Response</span></span>

<span data-ttu-id="271c7-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [消息](../resources/message.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="271c7-135">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="271c7-136">示例</span><span class="sxs-lookup"><span data-stu-id="271c7-136">Example</span></span>

<span data-ttu-id="271c7-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="271c7-137">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="271c7-138">请求</span><span class="sxs-lookup"><span data-stu-id="271c7-138">Request</span></span>

<span data-ttu-id="271c7-139">以下请求将指定的消息移动至删除项目文件夹，由其已知文件夹名称标识 `deleteditems` 。</span><span class="sxs-lookup"><span data-stu-id="271c7-139">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="271c7-140">响应</span><span class="sxs-lookup"><span data-stu-id="271c7-140">Response</span></span>

<span data-ttu-id="271c7-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="271c7-141">Here is an example of the response.</span></span>

> <span data-ttu-id="271c7-p106">**注释：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="271c7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
