---
title: 获取参与者
description: 检索**参与者**对象的属性和关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ec9f7393db1101d529d92635159fc27ca7aeb8fe
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913434"
---
# <a name="get-participant"></a><span data-ttu-id="e2072-103">获取参与者</span><span class="sxs-lookup"><span data-stu-id="e2072-103">Get participant</span></span>

<span data-ttu-id="e2072-104">检索**参与者**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2072-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2072-105">权限</span><span class="sxs-lookup"><span data-stu-id="e2072-105">Permissions</span></span>

| <span data-ttu-id="e2072-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2072-106">Permission type</span></span> | <span data-ttu-id="e2072-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2072-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e2072-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2072-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2072-109">不支持</span><span class="sxs-lookup"><span data-stu-id="e2072-109">Not Supported</span></span>        |
| <span data-ttu-id="e2072-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2072-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2072-111">不支持</span><span class="sxs-lookup"><span data-stu-id="e2072-111">Not Supported</span></span>        |
| <span data-ttu-id="e2072-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2072-112">Application</span></span>     | <span data-ttu-id="e2072-113">无</span><span class="sxs-lookup"><span data-stu-id="e2072-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e2072-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2072-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2072-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2072-115">Optional query parameters</span></span>
<span data-ttu-id="e2072-116">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2072-116">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2072-117">请求头</span><span class="sxs-lookup"><span data-stu-id="e2072-117">Request headers</span></span>
| <span data-ttu-id="e2072-118">名称</span><span class="sxs-lookup"><span data-stu-id="e2072-118">Name</span></span>          | <span data-ttu-id="e2072-119">说明</span><span class="sxs-lookup"><span data-stu-id="e2072-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e2072-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2072-120">Authorization</span></span> | <span data-ttu-id="e2072-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2072-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2072-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2072-123">Request body</span></span>
<span data-ttu-id="e2072-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2072-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2072-125">响应</span><span class="sxs-lookup"><span data-stu-id="e2072-125">Response</span></span>
<span data-ttu-id="e2072-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[参与者](../resources/participant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2072-126">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2072-127">示例</span><span class="sxs-lookup"><span data-stu-id="e2072-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2072-128">请求</span><span class="sxs-lookup"><span data-stu-id="e2072-128">Request</span></span>
<span data-ttu-id="e2072-129">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2072-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2072-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2072-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2072-131">C#</span><span class="sxs-lookup"><span data-stu-id="e2072-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2072-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2072-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2072-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2072-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2072-134">Java</span><span class="sxs-lookup"><span data-stu-id="e2072-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2072-135">响应</span><span class="sxs-lookup"><span data-stu-id="e2072-135">Response</span></span>

> <span data-ttu-id="e2072-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e2072-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type":"#microsoft.graph.participant",
   "info":{
      "@odata.type":"#microsoft.graph.participantInfo",
      "identity":{
         "@odata.type":"#microsoft.graph.identitySet",
         "application":{
            "@odata.type":"#microsoft.graph.identity",
            "displayName":"Display Name",
            "id":"278405a3-f568-4b3e-b684-009193463064"
            },
         "user":null,
         "device":null,
         "phone":null
      },
      "id":null
   },
   "mediaStreams":[
      {
         "@odata.type":"#microsoft.graph.mediaStream",
         "mediaType":"audio",
         "sourceId":"1",
         "direction":"sendReceive",
         "serverMuted":false,
         "label":null
      }
   ],
   "isMuted":false,
   "isInLobby":false,
   "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/participants/$entity",
   "metadata":null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
