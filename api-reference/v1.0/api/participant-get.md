---
title: 获取参与者
description: 检索**参与者**对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b20bb7647ba88016fe10733ed0c5b61b0576d5df
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865813"
---
# <a name="get-participant"></a><span data-ttu-id="fb6ac-103">获取参与者</span><span class="sxs-lookup"><span data-stu-id="fb6ac-103">Get participant</span></span>

<span data-ttu-id="fb6ac-104">检索**参与者**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb6ac-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb6ac-105">Permissions</span></span>

| <span data-ttu-id="fb6ac-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb6ac-106">Permission type</span></span> | <span data-ttu-id="fb6ac-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb6ac-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="fb6ac-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb6ac-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb6ac-109">不支持</span><span class="sxs-lookup"><span data-stu-id="fb6ac-109">Not Supported</span></span>        |
| <span data-ttu-id="fb6ac-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb6ac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb6ac-111">不支持</span><span class="sxs-lookup"><span data-stu-id="fb6ac-111">Not Supported</span></span>        |
| <span data-ttu-id="fb6ac-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb6ac-112">Application</span></span>     | <span data-ttu-id="fb6ac-113">无</span><span class="sxs-lookup"><span data-stu-id="fb6ac-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="fb6ac-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb6ac-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb6ac-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb6ac-115">Optional query parameters</span></span>
<span data-ttu-id="fb6ac-116">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-116">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb6ac-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb6ac-117">Request headers</span></span>
| <span data-ttu-id="fb6ac-118">名称</span><span class="sxs-lookup"><span data-stu-id="fb6ac-118">Name</span></span>          | <span data-ttu-id="fb6ac-119">说明</span><span class="sxs-lookup"><span data-stu-id="fb6ac-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fb6ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb6ac-120">Authorization</span></span> | <span data-ttu-id="fb6ac-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb6ac-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb6ac-123">Request body</span></span>
<span data-ttu-id="fb6ac-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb6ac-125">响应</span><span class="sxs-lookup"><span data-stu-id="fb6ac-125">Response</span></span>
<span data-ttu-id="fb6ac-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[参与者](../resources/participant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-126">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb6ac-127">示例</span><span class="sxs-lookup"><span data-stu-id="fb6ac-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fb6ac-128">请求</span><span class="sxs-lookup"><span data-stu-id="fb6ac-128">Request</span></span>
<span data-ttu-id="fb6ac-129">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb6ac-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb6ac-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb6ac-131">C#</span><span class="sxs-lookup"><span data-stu-id="fb6ac-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb6ac-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb6ac-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb6ac-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb6ac-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fb6ac-134">Java</span><span class="sxs-lookup"><span data-stu-id="fb6ac-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fb6ac-135">响应</span><span class="sxs-lookup"><span data-stu-id="fb6ac-135">Response</span></span>

> <span data-ttu-id="fb6ac-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fb6ac-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
