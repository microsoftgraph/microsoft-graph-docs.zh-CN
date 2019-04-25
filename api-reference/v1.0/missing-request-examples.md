---
title: 将 /me 定义为单一实例
description: 必须在文档中添加以下内容, 以确保 Markdown-扫描程序
localization_priority: Normal
ms.openlocfilehash: da71bfcb25efbebdf4e6a111f23d8d16e3aca342
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569527"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="310d3-103">帮助程序（未包含在文档中的示例）</span><span class="sxs-lookup"><span data-stu-id="310d3-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="310d3-104">这些内容必须添加到文档中以确保 Markdown 扫描程序工具能够正确地处理 Graph 文档。</span><span class="sxs-lookup"><span data-stu-id="310d3-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="310d3-105">将 /me 定义为单一实例</span><span class="sxs-lookup"><span data-stu-id="310d3-105">Define the /me as singleton</span></span>

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


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="310d3-106">将驱动器定义为可查询实体集</span><span class="sxs-lookup"><span data-stu-id="310d3-106">Define drives as an queryable entityset</span></span>
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


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="310d3-107">将用户定义为可查询实体集</span><span class="sxs-lookup"><span data-stu-id="310d3-107">define users as an queryable entityset</span></span>

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
