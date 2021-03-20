---
author: swapnil1993
title: 更新 contentType
description: 更新内容类型
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: bb7b898a8eb05c70c4c9ec187d36d3d5a4ce69db
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946932"
---
# <a name="update-contenttype"></a><span data-ttu-id="5d0b8-103">更新 contentType</span><span class="sxs-lookup"><span data-stu-id="5d0b8-103">Update contentType</span></span>
<span data-ttu-id="5d0b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d0b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="5d0b8-105">更新内容 [类型][contentType]。</span><span class="sxs-lookup"><span data-stu-id="5d0b8-105">Update a [content type][contentType].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="5d0b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d0b8-106">Permissions</span></span>

  

<span data-ttu-id="5d0b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5d0b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="5d0b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d0b8-109">Permission type</span></span> | <span data-ttu-id="5d0b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d0b8-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d0b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d0b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d0b8-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5d0b8-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="5d0b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d0b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d0b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d0b8-114">Not supported.</span></span> |
|<span data-ttu-id="5d0b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d0b8-115">Application</span></span> |<span data-ttu-id="5d0b8-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5d0b8-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="5d0b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d0b8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="5d0b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d0b8-118">Request headers</span></span>
|<span data-ttu-id="5d0b8-119">名称</span><span class="sxs-lookup"><span data-stu-id="5d0b8-119">Name</span></span>|<span data-ttu-id="5d0b8-120">说明</span><span class="sxs-lookup"><span data-stu-id="5d0b8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d0b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0b8-121">Authorization</span></span>|<span data-ttu-id="5d0b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d0b8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d0b8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d0b8-124">Content-Type</span></span>|<span data-ttu-id="5d0b8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5d0b8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d0b8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d0b8-127">Request body</span></span>

<span data-ttu-id="5d0b8-128">在请求正文中，提供要更新的 [contentType][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d0b8-128">In the request body, supply a JSON representation of the [contentType][] resource to update.</span></span>  

## <a name="response"></a><span data-ttu-id="5d0b8-129">响应</span><span class="sxs-lookup"><span data-stu-id="5d0b8-129">Response</span></span>

<span data-ttu-id="5d0b8-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [contentType][] 对象。</span><span class="sxs-lookup"><span data-stu-id="5d0b8-130">If successful, this method returns a `200 OK` response code and an updated [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0b8-131">示例</span><span class="sxs-lookup"><span data-stu-id="5d0b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d0b8-132">请求</span><span class="sxs-lookup"><span data-stu-id="5d0b8-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d0b8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d0b8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype"
}
-->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
Content-Type: application/json

{
    "name": "updatedCt",
    "documentSet": {
        "shouldPrefixNameToFile": true,
        "allowedContentTypes": [{
            "id": "0x0101",
            "name": "Document"
        }],
        "defaultContents": [{
                "fileName": "a.txt",
                "contentType": {
                    "id": "0x0101"
                }
            },
            {
                "fileName": "b.txt",
                "contentType": {
                    "id": "0x0101"
                }
            }
        ],
        "sharedColumns": [{
                "name": "Description",
                "id": "cbb92da4-fd46-4c7d-af6c-3128c2a5576e"
            },
            {
                "name": "Address",
                "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50"
            }
        ],
        "welcomePageColumns": [{
            "name": "Address",
            "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50"
        }]
    }
}

```
# <a name="javascript"></a>[<span data-ttu-id="5d0b8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d0b8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d0b8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d0b8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d0b8-136">响应</span><span class="sxs-lookup"><span data-stu-id="5d0b8-136">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0x0101009B237E76EF94DC49B4E58139041E7C60",
    "description": "",
    "eTag": "\"7\"",
    "group": "Custom Content Types",
    "hidden": false,
    "name": "testdoc",
    "parentId": "0x0101",
    "base": {
        "id": "0x0101",
        "name": "Document"
    }
}

```

[contentType]: ../resources/contentType.md
