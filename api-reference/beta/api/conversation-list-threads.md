---
title: 列出线程
description: 获取组对话中的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0a45dc93952108860771d9cc22f38565937cf896
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985072"
---
# <a name="list-threads"></a><span data-ttu-id="9699c-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="9699c-103">List threads</span></span>

> <span data-ttu-id="9699c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9699c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9699c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9699c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9699c-106">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="9699c-106">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="9699c-107">注意：还可以 [获取组的所有线程](group-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="9699c-107">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9699c-108">权限</span><span class="sxs-lookup"><span data-stu-id="9699c-108">Permissions</span></span>
<span data-ttu-id="9699c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9699c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9699c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9699c-111">Permission type</span></span>      | <span data-ttu-id="9699c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9699c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9699c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9699c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9699c-114">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9699c-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="9699c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9699c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9699c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9699c-116">Not supported.</span></span>    |
|<span data-ttu-id="9699c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9699c-117">Application</span></span> | <span data-ttu-id="9699c-118">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9699c-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9699c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9699c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9699c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9699c-120">Optional query parameters</span></span>
<span data-ttu-id="9699c-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9699c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9699c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9699c-122">Request headers</span></span>
| <span data-ttu-id="9699c-123">标头</span><span class="sxs-lookup"><span data-stu-id="9699c-123">Header</span></span>       | <span data-ttu-id="9699c-124">值</span><span class="sxs-lookup"><span data-stu-id="9699c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9699c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9699c-125">Authorization</span></span>  | <span data-ttu-id="9699c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9699c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9699c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9699c-128">Request body</span></span>
<span data-ttu-id="9699c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9699c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9699c-130">响应</span><span class="sxs-lookup"><span data-stu-id="9699c-130">Response</span></span>

<span data-ttu-id="9699c-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9699c-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9699c-132">示例</span><span class="sxs-lookup"><span data-stu-id="9699c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9699c-133">请求</span><span class="sxs-lookup"><span data-stu-id="9699c-133">Request</span></span>
<span data-ttu-id="9699c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9699c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="9699c-135">响应</span><span class="sxs-lookup"><span data-stu-id="9699c-135">Response</span></span>
<span data-ttu-id="9699c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9699c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
