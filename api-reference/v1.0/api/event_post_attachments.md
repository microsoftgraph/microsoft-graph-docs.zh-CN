# <a name="add-attachment"></a><span data-ttu-id="a1f6a-101">Add attachment</span><span class="sxs-lookup"><span data-stu-id="a1f6a-101">Add attachment</span></span>

<span data-ttu-id="a1f6a-p101">使用此 API 将 [附件](../resources/attachment.md) 添加到事件。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-p101">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1f6a-104">权限</span><span class="sxs-lookup"><span data-stu-id="a1f6a-104">Permissions</span></span>
<span data-ttu-id="a1f6a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1f6a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1f6a-107">Permission type</span></span>      | <span data-ttu-id="a1f6a-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1f6a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1f6a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1f6a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a1f6a-110">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1f6a-110">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a1f6a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1f6a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1f6a-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1f6a-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a1f6a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1f6a-113">Application</span></span> | <span data-ttu-id="a1f6a-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1f6a-114">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1f6a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1f6a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a1f6a-116">用户或组的默认 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-116">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
POST /groups/{id}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
```
<span data-ttu-id="a1f6a-117">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="a1f6a-118">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="a1f6a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1f6a-119">Request headers</span></span>
| <span data-ttu-id="a1f6a-120">名称</span><span class="sxs-lookup"><span data-stu-id="a1f6a-120">Name</span></span>       | <span data-ttu-id="a1f6a-121">类型</span><span class="sxs-lookup"><span data-stu-id="a1f6a-121">Type</span></span> | <span data-ttu-id="a1f6a-122">说明</span><span class="sxs-lookup"><span data-stu-id="a1f6a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1f6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1f6a-123">Authorization</span></span>  | <span data-ttu-id="a1f6a-124">string</span><span class="sxs-lookup"><span data-stu-id="a1f6a-124">string</span></span>  | <span data-ttu-id="a1f6a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1f6a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1f6a-127">Content-Type</span></span> | <span data-ttu-id="a1f6a-128">string</span><span class="sxs-lookup"><span data-stu-id="a1f6a-128">string</span></span>  | <span data-ttu-id="a1f6a-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1f6a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1f6a-131">Request body</span></span>
<span data-ttu-id="a1f6a-132">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a1f6a-133">响应</span><span class="sxs-lookup"><span data-stu-id="a1f6a-133">Response</span></span>

<span data-ttu-id="a1f6a-134">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-134">If successful, this method returns `201, Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a1f6a-135">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="a1f6a-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a1f6a-136">请求</span><span class="sxs-lookup"><span data-stu-id="a1f6a-136">Request</span></span>
<span data-ttu-id="a1f6a-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments 
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```

<span data-ttu-id="a1f6a-138">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a1f6a-139">响应</span><span class="sxs-lookup"><span data-stu-id="a1f6a-139">Response</span></span>
<span data-ttu-id="a1f6a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="a1f6a-141">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="a1f6a-141">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a1f6a-142">请求</span><span class="sxs-lookup"><span data-stu-id="a1f6a-142">Request</span></span>

<span data-ttu-id="a1f6a-143">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-143">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
Content-type: application/json
Content-length: 600

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
        "@odata.type": "microsoft.graph.event",
        "subject": "Discuss gifts for children",
        "body": {
            "contentType": "HTML",
            "content": "Let's look for funding!"
         },
         "start": {
             "dateTime": "2016-12-02T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2016-12-02T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```

##### <a name="response"></a><span data-ttu-id="a1f6a-144">响应</span><span class="sxs-lookup"><span data-stu-id="a1f6a-144">Response</span></span>
<span data-ttu-id="a1f6a-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a1f6a-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/api/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/api/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
