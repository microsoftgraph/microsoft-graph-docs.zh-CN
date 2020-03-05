---
title: 获取参与者
description: 检索**参与者**对象的属性和关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 643bcdb06c69f7d0c80f7ba18a6020258630b507
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455982"
---
# <a name="get-participant"></a><span data-ttu-id="23c0a-103">获取参与者</span><span class="sxs-lookup"><span data-stu-id="23c0a-103">Get participant</span></span>

<span data-ttu-id="23c0a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="23c0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23c0a-105">检索**参与者**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23c0a-105">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23c0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="23c0a-106">Permissions</span></span>

| <span data-ttu-id="23c0a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="23c0a-107">Permission type</span></span> | <span data-ttu-id="23c0a-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23c0a-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="23c0a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23c0a-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="23c0a-110">不支持</span><span class="sxs-lookup"><span data-stu-id="23c0a-110">Not Supported</span></span>        |
| <span data-ttu-id="23c0a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23c0a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23c0a-112">不支持</span><span class="sxs-lookup"><span data-stu-id="23c0a-112">Not Supported</span></span>        |
| <span data-ttu-id="23c0a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="23c0a-113">Application</span></span>     | <span data-ttu-id="23c0a-114">无</span><span class="sxs-lookup"><span data-stu-id="23c0a-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="23c0a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23c0a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="23c0a-116">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="23c0a-116">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="23c0a-117">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="23c0a-117">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="23c0a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23c0a-118">Optional query parameters</span></span>
<span data-ttu-id="23c0a-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23c0a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23c0a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="23c0a-120">Request headers</span></span>
| <span data-ttu-id="23c0a-121">名称</span><span class="sxs-lookup"><span data-stu-id="23c0a-121">Name</span></span>          | <span data-ttu-id="23c0a-122">说明</span><span class="sxs-lookup"><span data-stu-id="23c0a-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="23c0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23c0a-123">Authorization</span></span> | <span data-ttu-id="23c0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23c0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23c0a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="23c0a-126">Request body</span></span>
<span data-ttu-id="23c0a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23c0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23c0a-128">响应</span><span class="sxs-lookup"><span data-stu-id="23c0a-128">Response</span></span>
<span data-ttu-id="23c0a-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[参与者](../resources/participant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23c0a-129">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23c0a-130">示例</span><span class="sxs-lookup"><span data-stu-id="23c0a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23c0a-131">请求</span><span class="sxs-lookup"><span data-stu-id="23c0a-131">Request</span></span>
<span data-ttu-id="23c0a-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="23c0a-132">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23c0a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="23c0a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="c"></a>[<span data-ttu-id="23c0a-134">C#</span><span class="sxs-lookup"><span data-stu-id="23c0a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23c0a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23c0a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23c0a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23c0a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23c0a-137">响应</span><span class="sxs-lookup"><span data-stu-id="23c0a-137">Response</span></span>

> <span data-ttu-id="23c0a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="23c0a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "id":"278405a3-f568-4b3e-b684-009193463064",
            "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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
   "metadata":null,
   "recordingInfo":null
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
