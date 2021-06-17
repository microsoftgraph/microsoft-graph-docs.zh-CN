---
title: 获取 filesFolder
description: 检索频道的 filesFolder 导航路径。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8515b6ebb853c65ba44ce18c401179e115605689
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971284"
---
# <a name="get-filesfolder"></a><span data-ttu-id="4acb8-103">获取 filesFolder</span><span class="sxs-lookup"><span data-stu-id="4acb8-103">Get filesFolder</span></span>

<span data-ttu-id="4acb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4acb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4acb8-105">获取[频道](../resources/channel.md)的文件储存位置元数据。</span><span class="sxs-lookup"><span data-stu-id="4acb8-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4acb8-106">权限</span><span class="sxs-lookup"><span data-stu-id="4acb8-106">Permissions</span></span>
<span data-ttu-id="4acb8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4acb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4acb8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4acb8-109">Permission type</span></span>      | <span data-ttu-id="4acb8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4acb8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4acb8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4acb8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4acb8-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4acb8-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="4acb8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4acb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4acb8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4acb8-114">Not supported.</span></span>    |
|<span data-ttu-id="4acb8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4acb8-115">Application</span></span> | <span data-ttu-id="4acb8-116">File.Read.Group\*、Files.Read.All、Files.ReadWrite.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4acb8-116">File.Read.Group\*, Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="4acb8-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="4acb8-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="4acb8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4acb8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4acb8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4acb8-119">Optional query parameters</span></span>

<span data-ttu-id="4acb8-120">此运营商不支持通过 [OData 查询参数](/graph/query-parameters) 来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4acb8-120">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4acb8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4acb8-121">Request headers</span></span>
| <span data-ttu-id="4acb8-122">标头</span><span class="sxs-lookup"><span data-stu-id="4acb8-122">Header</span></span>       | <span data-ttu-id="4acb8-123">值</span><span class="sxs-lookup"><span data-stu-id="4acb8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4acb8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4acb8-124">Authorization</span></span>  | <span data-ttu-id="4acb8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4acb8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4acb8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4acb8-127">Request body</span></span>
<span data-ttu-id="4acb8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4acb8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4acb8-129">响应</span><span class="sxs-lookup"><span data-stu-id="4acb8-129">Response</span></span>

<span data-ttu-id="4acb8-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4acb8-130">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4acb8-131">示例</span><span class="sxs-lookup"><span data-stu-id="4acb8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4acb8-132">请求</span><span class="sxs-lookup"><span data-stu-id="4acb8-132">Request</span></span>
<span data-ttu-id="4acb8-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4acb8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4acb8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4acb8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/filesFolder
```
# <a name="c"></a>[<span data-ttu-id="4acb8-135">C#</span><span class="sxs-lookup"><span data-stu-id="4acb8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-filesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4acb8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4acb8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-filesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4acb8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4acb8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-filesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4acb8-138">Java</span><span class="sxs-lookup"><span data-stu-id="4acb8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-filesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4acb8-139">响应</span><span class="sxs-lookup"><span data-stu-id="4acb8-139">Response</span></span>
<span data-ttu-id="4acb8-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4acb8-140">The following is an example of the response.</span></span> 

><span data-ttu-id="4acb8-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4acb8-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/channels('19%3Af253e46c035b42308e9a4a22a87037af%40thread.skype')/filesFolder/$entity",
    "id": "01H7CFEKENJSSIUHGADZBKODARINQC5JMD",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    "lastEditedDateTime": null,
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    },
    "folder": {
        "childCount": 7
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get filesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



