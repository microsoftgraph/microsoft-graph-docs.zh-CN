---
title: 列出 acceptedSender
description: 获取此组 acceptedSenders 列表中的用户或组列表。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b073ea0a6173c86b298628c7e78baaaf0512eaac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892398"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="1ea7e-103">列出 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="1ea7e-103">List acceptedSenders</span></span>

> <span data-ttu-id="1ea7e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ea7e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ea7e-106">获取此组 acceptedSenders 列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-106">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="1ea7e-p102">接受的发件人列表中的用户可以发布到组对话（在 GET 请求 URL 中标识）。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-p102">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ea7e-109">权限</span><span class="sxs-lookup"><span data-stu-id="1ea7e-109">Permissions</span></span>
<span data-ttu-id="1ea7e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ea7e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ea7e-112">Permission type</span></span>      | <span data-ttu-id="1ea7e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ea7e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ea7e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ea7e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1ea7e-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ea7e-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ea7e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ea7e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ea7e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-117">Not supported.</span></span>    |
|<span data-ttu-id="1ea7e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ea7e-118">Application</span></span> | <span data-ttu-id="1ea7e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ea7e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ea7e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ea7e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ea7e-121">Optional query parameters</span></span>
<span data-ttu-id="1ea7e-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ea7e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ea7e-123">Request headers</span></span>
| <span data-ttu-id="1ea7e-124">标头</span><span class="sxs-lookup"><span data-stu-id="1ea7e-124">Header</span></span>       | <span data-ttu-id="1ea7e-125">值</span><span class="sxs-lookup"><span data-stu-id="1ea7e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ea7e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ea7e-126">Authorization</span></span>  | <span data-ttu-id="1ea7e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ea7e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ea7e-129">Request body</span></span>
<span data-ttu-id="1ea7e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ea7e-131">响应</span><span class="sxs-lookup"><span data-stu-id="1ea7e-131">Response</span></span>
<span data-ttu-id="1ea7e-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ea7e-133">示例</span><span class="sxs-lookup"><span data-stu-id="1ea7e-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1ea7e-134">请求</span><span class="sxs-lookup"><span data-stu-id="1ea7e-134">Request</span></span>
<span data-ttu-id="1ea7e-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```

#### <a name="response"></a><span data-ttu-id="1ea7e-136">响应</span><span class="sxs-lookup"><span data-stu-id="1ea7e-136">Response</span></span>
<span data-ttu-id="1ea7e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-137">The following is an example of the response.</span></span>
><span data-ttu-id="1ea7e-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ea7e-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ea7e-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
