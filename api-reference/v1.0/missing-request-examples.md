---
title: 将 /me 定义为单一实例
description: 必须在文档中添加以下内容, 以确保 Markdown-扫描程序
localization_priority: Normal
ms.openlocfilehash: 4ccdfdd669efe83d779cc3294b6372c4294d5179
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459515"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="b199c-103">帮助程序（未包含在文档中的示例）</span><span class="sxs-lookup"><span data-stu-id="b199c-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="b199c-104">这些内容必须添加到文档中以确保 Markdown 扫描程序工具能够正确地处理 Graph 文档。</span><span class="sxs-lookup"><span data-stu-id="b199c-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="b199c-105">将 /me 定义为单一实例</span><span class="sxs-lookup"><span data-stu-id="b199c-105">Define the /me as singleton</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b199c-106">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b199c-106">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b199c-107">C#</span><span class="sxs-lookup"><span data-stu-id="b199c-107">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-current-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b199c-108">Javascript</span><span class="sxs-lookup"><span data-stu-id="b199c-108">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-current-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b199c-109">目标-C</span><span class="sxs-lookup"><span data-stu-id="b199c-109">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-current-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="b199c-110">将驱动器定义为可查询实体集</span><span class="sxs-lookup"><span data-stu-id="b199c-110">Define drives as an queryable entityset</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b199c-111">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b199c-111">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b199c-112">C#</span><span class="sxs-lookup"><span data-stu-id="b199c-112">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-from-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b199c-113">Javascript</span><span class="sxs-lookup"><span data-stu-id="b199c-113">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-from-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b199c-114">目标-C</span><span class="sxs-lookup"><span data-stu-id="b199c-114">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-from-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="b199c-115">将用户定义为可查询实体集</span><span class="sxs-lookup"><span data-stu-id="b199c-115">define users as an queryable entityset</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b199c-116">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b199c-116">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b199c-117">C#</span><span class="sxs-lookup"><span data-stu-id="b199c-117">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b199c-118">Javascript</span><span class="sxs-lookup"><span data-stu-id="b199c-118">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b199c-119">目标-C</span><span class="sxs-lookup"><span data-stu-id="b199c-119">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d73
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Missing Requests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
