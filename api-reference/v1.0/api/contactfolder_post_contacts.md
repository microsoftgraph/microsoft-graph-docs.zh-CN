# <a name="create-contact"></a><span data-ttu-id="a0a5f-101">创建联系人</span><span class="sxs-lookup"><span data-stu-id="a0a5f-101">Create Contact</span></span>

<span data-ttu-id="a0a5f-102">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-102">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0a5f-103">权限</span><span class="sxs-lookup"><span data-stu-id="a0a5f-103">Permissions</span></span>
<span data-ttu-id="a0a5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a0a5f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0a5f-106">Permission type</span></span>      | <span data-ttu-id="a0a5f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0a5f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0a5f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0a5f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a0a5f-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0a5f-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a0a5f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0a5f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0a5f-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0a5f-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a0a5f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0a5f-112">Application</span></span> | <span data-ttu-id="a0a5f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0a5f-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0a5f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0a5f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="a0a5f-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0a5f-115">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="a0a5f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0a5f-116">Request headers</span></span>
| <span data-ttu-id="a0a5f-117">标头</span><span class="sxs-lookup"><span data-stu-id="a0a5f-117">Header</span></span>       | <span data-ttu-id="a0a5f-118">值</span><span class="sxs-lookup"><span data-stu-id="a0a5f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0a5f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0a5f-119">Authorization</span></span>  | <span data-ttu-id="a0a5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0a5f-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0a5f-122">Content-Type</span></span>  | <span data-ttu-id="a0a5f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a0a5f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0a5f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0a5f-125">Request body</span></span>
<span data-ttu-id="a0a5f-126">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0a5f-127">响应</span><span class="sxs-lookup"><span data-stu-id="a0a5f-127">Response</span></span>

<span data-ttu-id="a0a5f-128">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Contact](../resources/contact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-128">If successful, this method returns `201, Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0a5f-129">示例</span><span class="sxs-lookup"><span data-stu-id="a0a5f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0a5f-130">请求</span><span class="sxs-lookup"><span data-stu-id="a0a5f-130">Request</span></span>
<span data-ttu-id="a0a5f-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="a0a5f-132">在请求正文中，提供 [Contact](../resources/contact.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0a5f-133">响应</span><span class="sxs-lookup"><span data-stu-id="a0a5f-133">Response</span></span>
<span data-ttu-id="a0a5f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0a5f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->