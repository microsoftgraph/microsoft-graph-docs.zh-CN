---
title: 获取 filesFolder
description: 检索频道的 filesFolder。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 32272d197ff46545a7152f72f660a6132486d6c0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039893"
---
# <a name="get-filesfolder"></a><span data-ttu-id="3e871-103">获取 filesFolder</span><span class="sxs-lookup"><span data-stu-id="3e871-103">Get filesFolder</span></span>

<span data-ttu-id="3e871-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e871-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e871-105">获取[频道](../resources/channel.md)的文件储存位置元数据。</span><span class="sxs-lookup"><span data-stu-id="3e871-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3e871-106">权限</span><span class="sxs-lookup"><span data-stu-id="3e871-106">Permissions</span></span>
<span data-ttu-id="3e871-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e871-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e871-109">Permission type</span></span>      | <span data-ttu-id="3e871-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e871-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e871-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e871-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e871-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e871-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="3e871-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e871-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e871-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e871-114">Not supported.</span></span>    |
|<span data-ttu-id="3e871-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e871-115">Application</span></span> | <span data-ttu-id="3e871-116">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e871-116">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3e871-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e871-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e871-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3e871-118">Optional query parameters</span></span>

<span data-ttu-id="3e871-119">此运营商不支持通过 [OData 查询参数](/graph/query-parameters) 来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3e871-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e871-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e871-120">Request headers</span></span>
| <span data-ttu-id="3e871-121">标头</span><span class="sxs-lookup"><span data-stu-id="3e871-121">Header</span></span>       | <span data-ttu-id="3e871-122">值</span><span class="sxs-lookup"><span data-stu-id="3e871-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e871-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e871-123">Authorization</span></span>  | <span data-ttu-id="3e871-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e871-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e871-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e871-126">Request body</span></span>
<span data-ttu-id="3e871-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e871-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e871-128">响应</span><span class="sxs-lookup"><span data-stu-id="3e871-128">Response</span></span>

<span data-ttu-id="3e871-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e871-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e871-130">示例</span><span class="sxs-lookup"><span data-stu-id="3e871-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e871-131">请求</span><span class="sxs-lookup"><span data-stu-id="3e871-131">Request</span></span>

<span data-ttu-id="3e871-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e871-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e871-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e871-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/filesFolder
```
# <a name="c"></a>[<span data-ttu-id="3e871-134">C#</span><span class="sxs-lookup"><span data-stu-id="3e871-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-filesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e871-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e871-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-filesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e871-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e871-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-filesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e871-137">Java</span><span class="sxs-lookup"><span data-stu-id="3e871-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-filesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3e871-138">响应</span><span class="sxs-lookup"><span data-stu-id="3e871-138">Response</span></span>

<span data-ttu-id="3e871-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e871-139">The following is an example of the response.</span></span> 

><span data-ttu-id="3e871-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3e871-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/channels('19%3Af253e46c035b42308e9a4a22a87037af%40thread.skype')/filesFolder/$entity",
    "id": "01H7CFEKENJSSIUHGADZBKODARINQC5JMD",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z"
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

