# <a name="list-recent-files"></a><span data-ttu-id="e1388-101">列出最近使用的文件</span><span class="sxs-lookup"><span data-stu-id="e1388-101">List recent files</span></span>

<span data-ttu-id="e1388-p101">列出已登录用户最近使用的一组项目。此集合包含用户驱动器中的项目，以及他们有从其他驱动器进行访问的权限的项目。</span><span class="sxs-lookup"><span data-stu-id="e1388-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1388-104">权限</span><span class="sxs-lookup"><span data-stu-id="e1388-104">Permissions</span></span>
<span data-ttu-id="e1388-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e1388-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1388-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1388-107">Permission type</span></span>      | <span data-ttu-id="e1388-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1388-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1388-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1388-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e1388-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1388-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1388-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1388-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1388-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1388-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1388-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1388-113">Application</span></span> | <span data-ttu-id="e1388-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1388-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1388-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1388-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/recent
```

## <a name="request-body"></a><span data-ttu-id="e1388-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1388-116">Request body</span></span>
<span data-ttu-id="e1388-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1388-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="e1388-118">示例</span><span class="sxs-lookup"><span data-stu-id="e1388-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-recent", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/recent
```

## <a name="response"></a><span data-ttu-id="e1388-119">响应</span><span class="sxs-lookup"><span data-stu-id="e1388-119">Response</span></span>

<span data-ttu-id="e1388-p103">此方法返回驱动器所有者最近访问的项目的 [DriveItem](../resources/driveitem.md) 资源集合。用户驱动器外部的项目将包括 [RemoteItem](../resources/remoteitem.md) 方面，它们提供用来访问共享项目的信息。</span><span class="sxs-lookup"><span data-stu-id="e1388-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed. Items outside of the user's drive will include the [RemoteItem](../resources/remoteitem.md) facet, which provides information to access the shared item.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="e1388-122">注解</span><span class="sxs-lookup"><span data-stu-id="e1388-122">Remarks</span></span>

<span data-ttu-id="e1388-p104">从**最近**操作返回的部分 driveItem 将包括 **remoteItem** 方面，这表明它们是其他驱动器中的项目。若要访问原始的 driveItem 对象，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="e1388-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
