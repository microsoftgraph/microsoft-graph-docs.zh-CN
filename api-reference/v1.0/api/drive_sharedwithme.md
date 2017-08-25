# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="9b916-101">列出与已登录用户共享的项目</span><span class="sxs-lookup"><span data-stu-id="9b916-101">List items shared with the signed-in user</span></span>

<span data-ttu-id="9b916-102">检索已与[驱动器](../resources/drive.md)所有者共享的 [DriveItem](../resources/driveitem.md) 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="9b916-102">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b916-103">权限</span><span class="sxs-lookup"><span data-stu-id="9b916-103">Permissions</span></span>
<span data-ttu-id="9b916-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9b916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9b916-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b916-106">Permission type</span></span>      | <span data-ttu-id="9b916-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b916-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9b916-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b916-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9b916-109">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b916-109">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="9b916-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b916-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b916-111">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b916-111">Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="9b916-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b916-112">Application</span></span> | <span data-ttu-id="9b916-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b916-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

<span data-ttu-id="9b916-114">此外，如果没有 **All** 范围之一，无法访问从此 API 返回的共享项。</span><span class="sxs-lookup"><span data-stu-id="9b916-114">Note: while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite scopes, some properties may be missing. Additionally, without one of the  **All** scopes, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="9b916-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b916-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/sharedWithMe
```

## <a name="request-body"></a><span data-ttu-id="9b916-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b916-116">Request body</span></span>
<span data-ttu-id="9b916-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b916-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="9b916-118">示例</span><span class="sxs-lookup"><span data-stu-id="9b916-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-sharedwithme", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="9b916-119">响应</span><span class="sxs-lookup"><span data-stu-id="9b916-119">Response</span></span>

<span data-ttu-id="9b916-p102">此方法返回 [DriveItem](../resources/driveitem.md) 资源的集合，这些资源包含已与驱动器所有者共享的 DriveItem 资源。在此示例中，由于此驱动器是用户的默认驱动器，此方法将返回与已登录用户共享的项目。</span><span class="sxs-lookup"><span data-stu-id="9b916-p102">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
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
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="9b916-122">注解</span><span class="sxs-lookup"><span data-stu-id="9b916-122">Remarks</span></span>

<span data-ttu-id="9b916-p103">从 **sharedWithMe** 操作返回的 driveItem 始终都将包括 [**remoteItem**](../resources/remoteitem.md) 方面，这表明它们是其他驱动器中的项目。若要访问共享的 DriveItem 资源，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：</span><span class="sxs-lookup"><span data-stu-id="9b916-p103">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
