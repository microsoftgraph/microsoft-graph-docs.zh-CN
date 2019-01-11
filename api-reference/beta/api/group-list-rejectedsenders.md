---
title: 列出 rejectedSender
description: '获取此组 rejectedSenders 列表中的用户或组列表。 '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 2ce1f5244997e9ef38c9e57b020fa1f0bfb22e37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849138"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="2ec0f-103">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="2ec0f-103">List rejectedSenders</span></span>

> <span data-ttu-id="2ec0f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ec0f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ec0f-106">获取此组 rejectedSenders 列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-106">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="2ec0f-p102">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-p102">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ec0f-109">权限</span><span class="sxs-lookup"><span data-stu-id="2ec0f-109">Permissions</span></span>
<span data-ttu-id="2ec0f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ec0f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ec0f-112">Permission type</span></span>      | <span data-ttu-id="2ec0f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ec0f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ec0f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ec0f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2ec0f-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ec0f-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ec0f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ec0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec0f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-117">Not supported.</span></span>    |
|<span data-ttu-id="2ec0f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ec0f-118">Application</span></span> | <span data-ttu-id="2ec0f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ec0f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ec0f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ec0f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ec0f-121">Optional query parameters</span></span>
<span data-ttu-id="2ec0f-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ec0f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ec0f-123">Request headers</span></span>
| <span data-ttu-id="2ec0f-124">标头</span><span class="sxs-lookup"><span data-stu-id="2ec0f-124">Header</span></span>       | <span data-ttu-id="2ec0f-125">值</span><span class="sxs-lookup"><span data-stu-id="2ec0f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ec0f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ec0f-126">Authorization</span></span>  | <span data-ttu-id="2ec0f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ec0f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ec0f-129">Request body</span></span>
<span data-ttu-id="2ec0f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ec0f-131">响应</span><span class="sxs-lookup"><span data-stu-id="2ec0f-131">Response</span></span>
<span data-ttu-id="2ec0f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ec0f-133">示例</span><span class="sxs-lookup"><span data-stu-id="2ec0f-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2ec0f-134">请求</span><span class="sxs-lookup"><span data-stu-id="2ec0f-134">Request</span></span>
<span data-ttu-id="2ec0f-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="2ec0f-136">响应</span><span class="sxs-lookup"><span data-stu-id="2ec0f-136">Response</span></span>
<span data-ttu-id="2ec0f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-137">The following is an example of the response.</span></span>
><span data-ttu-id="2ec0f-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2ec0f-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ec0f-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
