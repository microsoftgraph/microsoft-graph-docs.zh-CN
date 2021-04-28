---
title: 获取参与者
description: 检索参与者对象的属性 **和** 关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1d09c3bf78d604905a634245e45216fa94312c7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054509"
---
# <a name="get-participant"></a><span data-ttu-id="1cfe3-103">获取参与者</span><span class="sxs-lookup"><span data-stu-id="1cfe3-103">Get participant</span></span>

<span data-ttu-id="1cfe3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cfe3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1cfe3-105">检索参与者对象的属性 **和** 关系。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-105">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cfe3-106">权限</span><span class="sxs-lookup"><span data-stu-id="1cfe3-106">Permissions</span></span>

| <span data-ttu-id="1cfe3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cfe3-107">Permission type</span></span> | <span data-ttu-id="1cfe3-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1cfe3-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1cfe3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cfe3-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cfe3-110">不支持</span><span class="sxs-lookup"><span data-stu-id="1cfe3-110">Not Supported</span></span>        |
| <span data-ttu-id="1cfe3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cfe3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cfe3-112">不支持</span><span class="sxs-lookup"><span data-stu-id="1cfe3-112">Not Supported</span></span>        |
| <span data-ttu-id="1cfe3-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cfe3-113">Application</span></span>     | <span data-ttu-id="1cfe3-114">无</span><span class="sxs-lookup"><span data-stu-id="1cfe3-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="1cfe3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cfe3-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cfe3-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1cfe3-116">Optional query parameters</span></span>
<span data-ttu-id="1cfe3-117">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-117">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cfe3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cfe3-118">Request headers</span></span>
| <span data-ttu-id="1cfe3-119">名称</span><span class="sxs-lookup"><span data-stu-id="1cfe3-119">Name</span></span>          | <span data-ttu-id="1cfe3-120">说明</span><span class="sxs-lookup"><span data-stu-id="1cfe3-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1cfe3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cfe3-121">Authorization</span></span> | <span data-ttu-id="1cfe3-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cfe3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cfe3-124">Request body</span></span>
<span data-ttu-id="1cfe3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cfe3-126">响应</span><span class="sxs-lookup"><span data-stu-id="1cfe3-126">Response</span></span>
<span data-ttu-id="1cfe3-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/participant.md)代码和 participant 对象。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-127">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cfe3-128">示例</span><span class="sxs-lookup"><span data-stu-id="1cfe3-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1cfe3-129">请求</span><span class="sxs-lookup"><span data-stu-id="1cfe3-129">Request</span></span>
<span data-ttu-id="1cfe3-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cfe3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfe3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="c"></a>[<span data-ttu-id="1cfe3-132">C#</span><span class="sxs-lookup"><span data-stu-id="1cfe3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cfe3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cfe3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cfe3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cfe3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cfe3-135">Java</span><span class="sxs-lookup"><span data-stu-id="1cfe3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1cfe3-136">响应</span><span class="sxs-lookup"><span data-stu-id="1cfe3-136">Response</span></span>

> <span data-ttu-id="1cfe3-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1cfe3-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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

