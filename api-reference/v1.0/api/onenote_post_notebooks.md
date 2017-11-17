# <a name="create-notebook"></a><span data-ttu-id="efb56-101">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="efb56-101">Create notebook</span></span>

<span data-ttu-id="efb56-102">新建 OneNote [笔记本](../resources/notebook.md)。</span><span class="sxs-lookup"><span data-stu-id="efb56-102">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="efb56-103">权限</span><span class="sxs-lookup"><span data-stu-id="efb56-103">Permissions</span></span>
<span data-ttu-id="efb56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="efb56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="efb56-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="efb56-106">Permission type</span></span>      | <span data-ttu-id="efb56-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efb56-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efb56-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efb56-108">Delegated (work or school account)</span></span> | <span data-ttu-id="efb56-109">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb56-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="efb56-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efb56-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb56-111">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb56-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="efb56-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="efb56-112">Application</span></span> | <span data-ttu-id="efb56-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb56-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efb56-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efb56-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="efb56-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="efb56-115">Request headers</span></span>
| <span data-ttu-id="efb56-116">名称</span><span class="sxs-lookup"><span data-stu-id="efb56-116">Name</span></span>       | <span data-ttu-id="efb56-117">类型</span><span class="sxs-lookup"><span data-stu-id="efb56-117">Type</span></span> | <span data-ttu-id="efb56-118">说明</span><span class="sxs-lookup"><span data-stu-id="efb56-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efb56-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb56-119">Authorization</span></span>  | <span data-ttu-id="efb56-120">string</span><span class="sxs-lookup"><span data-stu-id="efb56-120">string</span></span>  | <span data-ttu-id="efb56-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efb56-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efb56-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efb56-123">Content-Type</span></span> | <span data-ttu-id="efb56-124">string</span><span class="sxs-lookup"><span data-stu-id="efb56-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="efb56-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="efb56-125">Request body</span></span>
<span data-ttu-id="efb56-126">在请求正文中，提供笔记本名称。</span><span class="sxs-lookup"><span data-stu-id="efb56-126">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="efb56-p103">笔记本名称必须是唯一的。该名称不能超过 128 个字符，也不能包含以下字符：?*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="efb56-p103">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="efb56-129">响应</span><span class="sxs-lookup"><span data-stu-id="efb56-129">Response</span></span>

<span data-ttu-id="efb56-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新的 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efb56-130">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb56-131">示例</span><span class="sxs-lookup"><span data-stu-id="efb56-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efb56-132">请求</span><span class="sxs-lookup"><span data-stu-id="efb56-132">Request</span></span>
<span data-ttu-id="efb56-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efb56-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="efb56-134">响应</span><span class="sxs-lookup"><span data-stu-id="efb56-134">Response</span></span>
<span data-ttu-id="efb56-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efb56-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->