# <a name="delete-directoryobject"></a><span data-ttu-id="7d531-101">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="7d531-101">Delete directoryObject</span></span>

<span data-ttu-id="7d531-102">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="7d531-102">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d531-103">权限</span><span class="sxs-lookup"><span data-stu-id="7d531-103">Permissions</span></span>
<span data-ttu-id="7d531-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7d531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7d531-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d531-106">Permission type</span></span>      | <span data-ttu-id="7d531-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d531-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d531-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d531-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7d531-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d531-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d531-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d531-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d531-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d531-111">Not supported.</span></span>    |
|<span data-ttu-id="7d531-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d531-112">Application</span></span> | <span data-ttu-id="7d531-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d531-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d531-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d531-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7d531-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d531-115">Request headers</span></span>
| <span data-ttu-id="7d531-116">名称</span><span class="sxs-lookup"><span data-stu-id="7d531-116">Name</span></span>       | <span data-ttu-id="7d531-117">类型</span><span class="sxs-lookup"><span data-stu-id="7d531-117">Type</span></span> | <span data-ttu-id="7d531-118">说明</span><span class="sxs-lookup"><span data-stu-id="7d531-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d531-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d531-119">Authorization</span></span>  | <span data-ttu-id="7d531-120">string</span><span class="sxs-lookup"><span data-stu-id="7d531-120">string</span></span>  | <span data-ttu-id="7d531-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d531-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d531-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d531-123">Request body</span></span>
<span data-ttu-id="7d531-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d531-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d531-125">响应</span><span class="sxs-lookup"><span data-stu-id="7d531-125">Response</span></span>

<span data-ttu-id="7d531-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7d531-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d531-128">示例</span><span class="sxs-lookup"><span data-stu-id="7d531-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d531-129">请求</span><span class="sxs-lookup"><span data-stu-id="7d531-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="7d531-130">响应</span><span class="sxs-lookup"><span data-stu-id="7d531-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->