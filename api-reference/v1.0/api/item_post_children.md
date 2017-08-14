# <a name="create-a-new-folder"></a><span data-ttu-id="b759c-101">新建文件夹</span><span class="sxs-lookup"><span data-stu-id="b759c-101">Create a new folder</span></span>

<span data-ttu-id="b759c-102">使用指定的父项或路径在 [驱动器](../resources/drive.md) 中新建文件夹或 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b759c-102">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b759c-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="b759c-103">Prerequisites</span></span>
<span data-ttu-id="b759c-104">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="b759c-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="b759c-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b759c-105">Files.ReadWrite</span></span>
* <span data-ttu-id="b759c-106">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b759c-106">Files.ReadWrite.All</span></span>
* <span data-ttu-id="b759c-107">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b759c-107">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="b759c-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b759c-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/children
POST /me/drive/items/{parent-item-id}/children
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="b759c-109">请求正文</span><span class="sxs-lookup"><span data-stu-id="b759c-109">Request body</span></span>
<span data-ttu-id="b759c-110">在请求正文中，提供要创建的 [DriveItem](../resources/driveitem.md) 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b759c-110">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="b759c-111">响应</span><span class="sxs-lookup"><span data-stu-id="b759c-111">Response</span></span>

<span data-ttu-id="b759c-112">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="b759c-112">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b759c-113">示例</span><span class="sxs-lookup"><span data-stu-id="b759c-113">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b759c-114">请求</span><span class="sxs-lookup"><span data-stu-id="b759c-114">Request</span></span>
<span data-ttu-id="b759c-115">下面是在用户的 OneDrive 根目录下新建文件夹请求示例。</span><span class="sxs-lookup"><span data-stu-id="b759c-115">Here is an example of the request to create a new folder in the user's OneDrive root.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_from_item"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { }
}
```

##### <a name="response"></a><span data-ttu-id="b759c-116">响应</span><span class="sxs-lookup"><span data-stu-id="b759c-116">Response</span></span>

<span data-ttu-id="b759c-117">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b759c-117">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "20160920T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "20160920T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create children",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
