# <a name="send-a-sharing-invitation"></a><span data-ttu-id="8b465-101">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="8b465-101">Send a sharing invitation</span></span>

<span data-ttu-id="8b465-p101">发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。</span><span class="sxs-lookup"><span data-stu-id="8b465-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b465-104">权限</span><span class="sxs-lookup"><span data-stu-id="8b465-104">Permissions</span></span>
<span data-ttu-id="8b465-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8b465-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b465-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b465-107">Permission type</span></span>      | <span data-ttu-id="8b465-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b465-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b465-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b465-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8b465-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b465-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b465-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b465-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b465-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b465-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b465-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b465-113">Application</span></span> | <span data-ttu-id="8b465-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b465-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b465-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b465-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a><span data-ttu-id="8b465-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b465-116">Request body</span></span>
<span data-ttu-id="8b465-117">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8b465-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b465-118">参数</span><span class="sxs-lookup"><span data-stu-id="8b465-118">Parameter</span></span>        | <span data-ttu-id="8b465-119">类型</span><span class="sxs-lookup"><span data-stu-id="8b465-119">Type</span></span>                                            | <span data-ttu-id="8b465-120">说明</span><span class="sxs-lookup"><span data-stu-id="8b465-120">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8b465-121">recipients</span><span class="sxs-lookup"><span data-stu-id="8b465-121">recipients</span></span>       | <span data-ttu-id="8b465-122">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="8b465-122">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="8b465-123">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="8b465-123">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="8b465-124">message</span><span class="sxs-lookup"><span data-stu-id="8b465-124">message</span></span>          | <span data-ttu-id="8b465-125">String</span><span class="sxs-lookup"><span data-stu-id="8b465-125">String</span></span>                                          | <span data-ttu-id="8b465-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="8b465-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="8b465-128">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="8b465-128">requireSignIn</span></span>    | <span data-ttu-id="8b465-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b465-129">Boolean</span></span>                                         | <span data-ttu-id="8b465-130">指定邀请的收件人要查看共享项目的登录位置。</span><span class="sxs-lookup"><span data-stu-id="8b465-130">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="8b465-131">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="8b465-131">sendInvitation</span></span>   | <span data-ttu-id="8b465-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b465-132">Boolean</span></span>                                         | <span data-ttu-id="8b465-133">指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。</span><span class="sxs-lookup"><span data-stu-id="8b465-133">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="8b465-134">roles</span><span class="sxs-lookup"><span data-stu-id="8b465-134">roles</span></span>            | <span data-ttu-id="8b465-135">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="8b465-135">Collection(String)</span></span>                              | <span data-ttu-id="8b465-136">指定授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="8b465-136">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="8b465-137">响应</span><span class="sxs-lookup"><span data-stu-id="8b465-137">Response</span></span>

<span data-ttu-id="8b465-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="8b465-138">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b465-139">示例</span><span class="sxs-lookup"><span data-stu-id="8b465-139">Example</span></span>
<span data-ttu-id="8b465-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8b465-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8b465-141">请求</span><span class="sxs-lookup"><span data-stu-id="8b465-141">Request</span></span>
<span data-ttu-id="8b465-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b465-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a><span data-ttu-id="8b465-143">响应</span><span class="sxs-lookup"><span data-stu-id="8b465-143">Response</span></span>
<span data-ttu-id="8b465-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b465-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="8b465-145">注解</span><span class="sxs-lookup"><span data-stu-id="8b465-145">Remarks</span></span>

* <span data-ttu-id="8b465-146">具有 `personal` **driveType**（OneDrive 个人版）的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="8b465-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="8b465-147">如需可用角色的列表，请参阅 [角色枚举](../resources/permission.md#roles-enumeration)。</span><span class="sxs-lookup"><span data-stu-id="8b465-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
