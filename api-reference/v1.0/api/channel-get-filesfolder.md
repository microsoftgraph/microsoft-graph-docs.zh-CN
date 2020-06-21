---
title: 获取 "获取"
description: 检索频道的 "工作"。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3701c0fde058f0040f1d4a25f882516a022893ea
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788436"
---
# <a name="get-filesfolder"></a><span data-ttu-id="0b6c6-103">获取 "获取"</span><span class="sxs-lookup"><span data-stu-id="0b6c6-103">Get filesFolder</span></span>

<span data-ttu-id="0b6c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b6c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b6c6-105">检索文件导航路径（用于[存储通道文件](../resources/channel.md)的位置的元数据）的文件。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-105">Retrieve the filesFolder navigation path, which is the metadata for the location where the channel files are stored, for a [channel](../resources/channel.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0b6c6-106">权限</span><span class="sxs-lookup"><span data-stu-id="0b6c6-106">Permissions</span></span>
<span data-ttu-id="0b6c6-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0b6c6-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0b6c6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b6c6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b6c6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b6c6-109">Permission type</span></span>      | <span data-ttu-id="0b6c6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b6c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b6c6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b6c6-112">文件. All、Group. all、Group、Group。全部。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-112">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b6c6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b6c6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-114">Not supported.</span></span>    |
|<span data-ttu-id="0b6c6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b6c6-115">Application</span></span> | <span data-ttu-id="0b6c6-116">文件. All、Group. all、Group、Group。全部。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-116">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>     |


## <a name="http-request"></a><span data-ttu-id="0b6c6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b6c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder

```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b6c6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b6c6-118">Optional query parameters</span></span>

<span data-ttu-id="0b6c6-119">此方法不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b6c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b6c6-120">Request headers</span></span>
| <span data-ttu-id="0b6c6-121">标头</span><span class="sxs-lookup"><span data-stu-id="0b6c6-121">Header</span></span>       | <span data-ttu-id="0b6c6-122">值</span><span class="sxs-lookup"><span data-stu-id="0b6c6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b6c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b6c6-123">Authorization</span></span>  | <span data-ttu-id="0b6c6-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0b6c6-124">Bearer {token}.</span></span> <span data-ttu-id="0b6c6-125">Required.</span><span class="sxs-lookup"><span data-stu-id="0b6c6-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b6c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b6c6-126">Request body</span></span>
<span data-ttu-id="0b6c6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b6c6-128">响应</span><span class="sxs-lookup"><span data-stu-id="0b6c6-128">Response</span></span>

<span data-ttu-id="0b6c6-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b6c6-130">示例</span><span class="sxs-lookup"><span data-stu-id="0b6c6-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b6c6-131">请求</span><span class="sxs-lookup"><span data-stu-id="0b6c6-131">Request</span></span>

<span data-ttu-id="0b6c6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/filesFolder
```
### <a name="response"></a><span data-ttu-id="0b6c6-133">响应</span><span class="sxs-lookup"><span data-stu-id="0b6c6-133">Response</span></span>

<span data-ttu-id="0b6c6-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b6c6-134">The following is an example of the response.</span></span> 

><span data-ttu-id="0b6c6-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0b6c6-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b6c6-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0b6c6-136">All the properties will be returned from an actual call.</span></span>
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
