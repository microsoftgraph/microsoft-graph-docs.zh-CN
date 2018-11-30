---
title: 列表 trendingAround
description: 返回用户周围趋势分析的项的列表的计算的洞察。
ms.openlocfilehash: 769c6a20105442129a6c4993a58bf6dbddce1b61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042058"
---
# <a name="list-trendingaround"></a><span data-ttu-id="1c89e-103">列表 trendingAround</span><span class="sxs-lookup"><span data-stu-id="1c89e-103">List trendingAround</span></span>

> <span data-ttu-id="1c89e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c89e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c89e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c89e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c89e-106">返回用户周围趋势分析的项的列表的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="1c89e-106">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="1c89e-107">**注意：** 此 API 将弃用，替换为[趋势 API](../resources/insights-trending.md)。</span><span class="sxs-lookup"><span data-stu-id="1c89e-107">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c89e-108">权限</span><span class="sxs-lookup"><span data-stu-id="1c89e-108">Permissions</span></span>
<span data-ttu-id="1c89e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c89e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c89e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c89e-111">Permission type</span></span>      | <span data-ttu-id="1c89e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c89e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c89e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c89e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c89e-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c89e-114">Sites.Read.All</span></span>    |
|<span data-ttu-id="1c89e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c89e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c89e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c89e-116">Not supported.</span></span>    |
|<span data-ttu-id="1c89e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c89e-117">Application</span></span> | <span data-ttu-id="1c89e-118">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c89e-118">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c89e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c89e-119">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c89e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1c89e-120">Optional query parameters</span></span>
<span data-ttu-id="1c89e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1c89e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c89e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c89e-122">Request headers</span></span>
| <span data-ttu-id="1c89e-123">标头</span><span class="sxs-lookup"><span data-stu-id="1c89e-123">Header</span></span>         | <span data-ttu-id="1c89e-124">值</span><span class="sxs-lookup"><span data-stu-id="1c89e-124">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="1c89e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c89e-125">Authorization</span></span>  | <span data-ttu-id="1c89e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c89e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1c89e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c89e-128">Content-Type</span></span>   | <span data-ttu-id="1c89e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1c89e-129">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="1c89e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c89e-130">Request body</span></span>
<span data-ttu-id="1c89e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c89e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c89e-132">响应</span><span class="sxs-lookup"><span data-stu-id="1c89e-132">Response</span></span>

<span data-ttu-id="1c89e-133">如果成功，此方法将在响应正文中返回的 200 OK 响应代码和[driveItem](../resources/driveitem.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1c89e-133">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c89e-134">示例</span><span class="sxs-lookup"><span data-stu-id="1c89e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c89e-135">请求</span><span class="sxs-lookup"><span data-stu-id="1c89e-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="1c89e-136">响应</span><span class="sxs-lookup"><span data-stu-id="1c89e-136">Response</span></span>
<span data-ttu-id="1c89e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c89e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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