---
title: 获取 "获取"
description: 检索频道的 "工作"。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0190f09eacb08dccdb5f8297fb3e7011cacaa0a0
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845664"
---
# <a name="get-filesfolder"></a><span data-ttu-id="946c1-103">获取 "获取"</span><span class="sxs-lookup"><span data-stu-id="946c1-103">Get filesFolder</span></span>

<span data-ttu-id="946c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="946c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="946c1-105">获取存储[通道](../resources/channel.md)文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="946c1-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="946c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="946c1-106">Permissions</span></span>
<span data-ttu-id="946c1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="946c1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="946c1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="946c1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="946c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="946c1-109">Permission type</span></span>      | <span data-ttu-id="946c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="946c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="946c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="946c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="946c1-112">文件. All、Group. all、Group、Group。全部。</span><span class="sxs-lookup"><span data-stu-id="946c1-112">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="946c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="946c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="946c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="946c1-114">Not supported.</span></span>    |
|<span data-ttu-id="946c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="946c1-115">Application</span></span> | <span data-ttu-id="946c1-116">文件. All、Group. all、Group、Group。全部。</span><span class="sxs-lookup"><span data-stu-id="946c1-116">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>     |


## <a name="http-request"></a><span data-ttu-id="946c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="946c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder

```

## <a name="optional-query-parameters"></a><span data-ttu-id="946c1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="946c1-118">Optional query parameters</span></span>

<span data-ttu-id="946c1-119">此方法不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="946c1-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="946c1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="946c1-120">Request headers</span></span>
| <span data-ttu-id="946c1-121">标头</span><span class="sxs-lookup"><span data-stu-id="946c1-121">Header</span></span>       | <span data-ttu-id="946c1-122">值</span><span class="sxs-lookup"><span data-stu-id="946c1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="946c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="946c1-123">Authorization</span></span>  | <span data-ttu-id="946c1-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="946c1-124">Bearer {token}.</span></span> <span data-ttu-id="946c1-125">Required.</span><span class="sxs-lookup"><span data-stu-id="946c1-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="946c1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="946c1-126">Request body</span></span>
<span data-ttu-id="946c1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="946c1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="946c1-128">响应</span><span class="sxs-lookup"><span data-stu-id="946c1-128">Response</span></span>

<span data-ttu-id="946c1-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="946c1-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="946c1-130">示例</span><span class="sxs-lookup"><span data-stu-id="946c1-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="946c1-131">请求</span><span class="sxs-lookup"><span data-stu-id="946c1-131">Request</span></span>

<span data-ttu-id="946c1-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="946c1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/filesFolder
```
### <a name="response"></a><span data-ttu-id="946c1-133">响应</span><span class="sxs-lookup"><span data-stu-id="946c1-133">Response</span></span>

<span data-ttu-id="946c1-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="946c1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="946c1-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="946c1-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="946c1-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="946c1-136">All the properties will be returned from an actual call.</span></span>
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
