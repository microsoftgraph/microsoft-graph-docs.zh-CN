# <a name="accessing-shared-driveitems"></a><span data-ttu-id="4e05c-101">访问共享 DriveItem</span><span class="sxs-lookup"><span data-stu-id="4e05c-101">Accessing shared DriveItems</span></span>

<span data-ttu-id="4e05c-102">通过使用 **shareId** 或共享 URL 访问共享 [DriveItem](../resources/driveitem.md) 或共享项目集合。</span><span class="sxs-lookup"><span data-stu-id="4e05c-102">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="4e05c-103">要与此 API 一起使用共享 URL，应用需要[将此 URL 转换为共享令牌](#transform-a-sharing-url)。</span><span class="sxs-lookup"><span data-stu-id="4e05c-103">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#transform-a-sharing-url).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e05c-104">权限</span><span class="sxs-lookup"><span data-stu-id="4e05c-104">Permissions</span></span>

<span data-ttu-id="4e05c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4e05c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4e05c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e05c-107">Permission type</span></span>      | <span data-ttu-id="4e05c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e05c-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4e05c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e05c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4e05c-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e05c-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4e05c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e05c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e05c-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e05c-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4e05c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e05c-113">Application</span></span> | <span data-ttu-id="4e05c-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e05c-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4e05c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e05c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /shares/{sharingIdOrUrl}
```

## <a name="request-body"></a><span data-ttu-id="4e05c-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e05c-116">Request body</span></span>
<span data-ttu-id="4e05c-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e05c-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e05c-118">响应</span><span class="sxs-lookup"><span data-stu-id="4e05c-118">Response</span></span>

<span data-ttu-id="4e05c-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sharedDriveItem](../resources/shareddriveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="4e05c-119">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e05c-120">示例</span><span class="sxs-lookup"><span data-stu-id="4e05c-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4e05c-121">请求</span><span class="sxs-lookup"><span data-stu-id="4e05c-121">Request</span></span>

<span data-ttu-id="4e05c-122">下面是一个请求检索共享项目的示例：</span><span class="sxs-lookup"><span data-stu-id="4e05c-122">Here is an example of the request to retrieve a shared item:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_shares_by_url"
}-->
```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}
```
##### <a name="response"></a><span data-ttu-id="4e05c-123">响应</span><span class="sxs-lookup"><span data-stu-id="4e05c-123">Response</span></span>

<span data-ttu-id="4e05c-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e05c-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="4e05c-125">直接访问共享项目</span><span class="sxs-lookup"><span data-stu-id="4e05c-125">Access the shared item directly</span></span>

<span data-ttu-id="4e05c-p102">虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。</span><span class="sxs-lookup"><span data-stu-id="4e05c-p102">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="4e05c-128">示例（单个文件）</span><span class="sxs-lookup"><span data-stu-id="4e05c-128">Example (single file)</span></span>

##### <a name="request"></a><span data-ttu-id="4e05c-129">请求</span><span class="sxs-lookup"><span data-stu-id="4e05c-129">Request</span></span>

<span data-ttu-id="4e05c-130">通过请求**根**关系，将返回共享的 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="4e05c-130">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a><span data-ttu-id="4e05c-131">响应</span><span class="sxs-lookup"><span data-stu-id="4e05c-131">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="4e05c-132">示例（共享文件夹）</span><span class="sxs-lookup"><span data-stu-id="4e05c-132">Example (shared folder)</span></span>

##### <a name="request"></a><span data-ttu-id="4e05c-133">请求</span><span class="sxs-lookup"><span data-stu-id="4e05c-133">Request</span></span>

<span data-ttu-id="4e05c-134">通过请求**根**关系并展开**子**集合，将同时返回共享的 **DriveItem** 以及共享文件夹内的文件。</span><span class="sxs-lookup"><span data-stu-id="4e05c-134">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a><span data-ttu-id="4e05c-135">响应</span><span class="sxs-lookup"><span data-stu-id="4e05c-135">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a><span data-ttu-id="4e05c-136">转换共享 URL</span><span class="sxs-lookup"><span data-stu-id="4e05c-136">Transform a sharing URL</span></span>

<span data-ttu-id="4e05c-137">若要使用**共享** API 访问共享 URL，需要将 URL 转换为共享令牌。</span><span class="sxs-lookup"><span data-stu-id="4e05c-137">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="4e05c-138">要将 URL 转换为共享令牌：</span><span class="sxs-lookup"><span data-stu-id="4e05c-138">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="4e05c-139">Base64 编码共享 URL。</span><span class="sxs-lookup"><span data-stu-id="4e05c-139">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="4e05c-140">通过以下方法，将 base64 编码数据转换成[未填充的 base64url 格式](https://en.wikipedia.org/wiki/Base64)：</span><span class="sxs-lookup"><span data-stu-id="4e05c-140">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="4e05c-141">剪裁掉字符串最后的 `=` 字符</span><span class="sxs-lookup"><span data-stu-id="4e05c-141">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="4e05c-142">将不安全的 URL 字符替换成等效字符；将 `/` 替换成 `_`，将 `+` 替换成 `-`。</span><span class="sxs-lookup"><span data-stu-id="4e05c-142">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="4e05c-143">将 `u!` 追加到字符串的开头。</span><span class="sxs-lookup"><span data-stu-id="4e05c-143">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="4e05c-144">例如，以下 C# 方法将输入字符串转换为共享令牌：</span><span class="sxs-lookup"><span data-stu-id="4e05c-144">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
