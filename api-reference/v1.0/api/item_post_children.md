# <a name="create-a-new-folder"></a><span data-ttu-id="4a315-101">新建文件夹</span><span class="sxs-lookup"><span data-stu-id="4a315-101">Create a new folder</span></span>

<span data-ttu-id="4a315-102">使用指定的父项或路径在[驱动器](../resources/drive.md)中新建文件夹或 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4a315-102">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a315-103">权限</span><span class="sxs-lookup"><span data-stu-id="4a315-103">Permissions</span></span>
<span data-ttu-id="4a315-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4a315-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a315-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a315-106">Permission type</span></span>      | <span data-ttu-id="4a315-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a315-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4a315-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a315-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a315-109">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a315-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4a315-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a315-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a315-111">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a315-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4a315-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a315-112">Application</span></span> | <span data-ttu-id="4a315-113">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a315-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a315-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a315-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/children
POST /me/drive/items/{parent-item-id}/children
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="4a315-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a315-115">Request body</span></span>
<span data-ttu-id="4a315-116">在请求正文中，提供要创建的 [DriveItem](../resources/driveitem.md) 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a315-116">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="4a315-117">响应</span><span class="sxs-lookup"><span data-stu-id="4a315-117">Response</span></span>

<span data-ttu-id="4a315-118">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="4a315-118">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a315-119">示例</span><span class="sxs-lookup"><span data-stu-id="4a315-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4a315-120">请求</span><span class="sxs-lookup"><span data-stu-id="4a315-120">Request</span></span>
<span data-ttu-id="4a315-121">下面是在用户的 OneDrive 根目录下新建文件夹请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a315-121">Here is an example of the request to create a new folder in the user's OneDrive root.</span></span>

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

##### <a name="response"></a><span data-ttu-id="4a315-122">响应</span><span class="sxs-lookup"><span data-stu-id="4a315-122">Response</span></span>

<span data-ttu-id="4a315-123">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a315-123">Here is an example of the response.</span></span>
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
