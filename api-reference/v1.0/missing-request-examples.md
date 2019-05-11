---
title: 将 /me 定义为单一实例
description: 必须在文档中添加以下内容, 以确保 Markdown-扫描程序
localization_priority: Normal
ms.openlocfilehash: d3130362ea0790a91c4a6f6a3f1e7465584872d8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951240"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="63ddd-103">帮助程序（未包含在文档中的示例）</span><span class="sxs-lookup"><span data-stu-id="63ddd-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="63ddd-104">这些内容必须添加到文档中以确保 Markdown 扫描程序工具能够正确地处理 Graph 文档。</span><span class="sxs-lookup"><span data-stu-id="63ddd-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="63ddd-105">将 /me 定义为单一实例</span><span class="sxs-lookup"><span data-stu-id="63ddd-105">Define the /me as singleton</span></span>

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="63ddd-106">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="63ddd-106">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="63ddd-107">C#</span><span class="sxs-lookup"><span data-stu-id="63ddd-107">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_current_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63ddd-108">Javascript</span><span class="sxs-lookup"><span data-stu-id="63ddd-108">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_current_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="63ddd-109">将驱动器定义为可查询实体集</span><span class="sxs-lookup"><span data-stu-id="63ddd-109">Define drives as an queryable entityset</span></span>
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="63ddd-110">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="63ddd-110">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="63ddd-111">C#</span><span class="sxs-lookup"><span data-stu-id="63ddd-111">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_drive_from_id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63ddd-112">Javascript</span><span class="sxs-lookup"><span data-stu-id="63ddd-112">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_drive_from_id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="63ddd-113">将用户定义为可查询实体集</span><span class="sxs-lookup"><span data-stu-id="63ddd-113">define users as an queryable entityset</span></span>

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="63ddd-114">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="63ddd-114">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="63ddd-115">C#</span><span class="sxs-lookup"><span data-stu-id="63ddd-115">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63ddd-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="63ddd-116">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d73
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Missing Requests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /missing-request-examples.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /missing-request-examples.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->