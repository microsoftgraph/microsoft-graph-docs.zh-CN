---
title: 列出 trendingAround
description: 计算得出的见解，可返回用户热门项目列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b1594d031f9ff007a87243ccf0cf481022b48d89
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052584"
---
# <a name="list-trendingaround"></a><span data-ttu-id="8dd24-103">列出 trendingAround</span><span class="sxs-lookup"><span data-stu-id="8dd24-103">List trendingAround</span></span>

<span data-ttu-id="8dd24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dd24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dd24-105">计算得出的见解，可返回用户热门项目列表。</span><span class="sxs-lookup"><span data-stu-id="8dd24-105">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="8dd24-106">**注意：** 此 API 将被弃用，并替换为趋势 [API。](../resources/insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="8dd24-106">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8dd24-107">权限</span><span class="sxs-lookup"><span data-stu-id="8dd24-107">Permissions</span></span>
<span data-ttu-id="8dd24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8dd24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dd24-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8dd24-110">Permission type</span></span>      | <span data-ttu-id="8dd24-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8dd24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dd24-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8dd24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8dd24-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dd24-113">Sites.Read.All</span></span>    |
|<span data-ttu-id="8dd24-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8dd24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dd24-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8dd24-115">Not supported.</span></span>    |
|<span data-ttu-id="8dd24-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8dd24-116">Application</span></span> | <span data-ttu-id="8dd24-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dd24-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dd24-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8dd24-118">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8dd24-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8dd24-119">Optional query parameters</span></span>
<span data-ttu-id="8dd24-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8dd24-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dd24-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8dd24-121">Request headers</span></span>
| <span data-ttu-id="8dd24-122">标头</span><span class="sxs-lookup"><span data-stu-id="8dd24-122">Header</span></span>         | <span data-ttu-id="8dd24-123">值</span><span class="sxs-lookup"><span data-stu-id="8dd24-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="8dd24-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dd24-124">Authorization</span></span>  | <span data-ttu-id="8dd24-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8dd24-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8dd24-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dd24-127">Content-Type</span></span>   | <span data-ttu-id="8dd24-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8dd24-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="8dd24-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8dd24-129">Request body</span></span>
<span data-ttu-id="8dd24-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8dd24-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dd24-131">响应</span><span class="sxs-lookup"><span data-stu-id="8dd24-131">Response</span></span>

<span data-ttu-id="8dd24-132">如果成功，此方法在响应正文中返回 200 OK 响应代码和 [driveItem](../resources/driveitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8dd24-132">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dd24-133">示例</span><span class="sxs-lookup"><span data-stu-id="8dd24-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8dd24-134">请求</span><span class="sxs-lookup"><span data-stu-id="8dd24-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="8dd24-135">响应</span><span class="sxs-lookup"><span data-stu-id="8dd24-135">Response</span></span>
<span data-ttu-id="8dd24-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8dd24-136">Here is an example of the response.</span></span> <span data-ttu-id="8dd24-137">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8dd24-137">Note: The response object shown here might be shortened for readability.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```