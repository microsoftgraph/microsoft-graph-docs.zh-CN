---
title: 列出 TrendingAround
description: 计算得出的见解，可返回用户周围的项目趋势列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 139416e3b21166f50e2f9fed529a7efe6b4dbd3e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720674"
---
# <a name="list-trendingaround"></a><span data-ttu-id="8d961-103">列出 TrendingAround</span><span class="sxs-lookup"><span data-stu-id="8d961-103">List trendingAround</span></span>

<span data-ttu-id="8d961-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d961-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d961-105">计算得出的见解，可返回用户周围的项目趋势列表。</span><span class="sxs-lookup"><span data-stu-id="8d961-105">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="8d961-106">**注意：** 此 API 将被弃用，并替换为趋势 [API。](../resources/insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="8d961-106">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d961-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8d961-107">Permissions</span></span>
<span data-ttu-id="8d961-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d961-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d961-110">Permission type</span></span>      | <span data-ttu-id="8d961-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d961-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d961-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d961-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d961-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d961-113">Sites.Read.All</span></span>    |
|<span data-ttu-id="8d961-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d961-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d961-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d961-115">Not supported.</span></span>    |
|<span data-ttu-id="8d961-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d961-116">Application</span></span> | <span data-ttu-id="8d961-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d961-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d961-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d961-118">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d961-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d961-119">Optional query parameters</span></span>
<span data-ttu-id="8d961-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d961-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d961-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d961-121">Request headers</span></span>
| <span data-ttu-id="8d961-122">标头</span><span class="sxs-lookup"><span data-stu-id="8d961-122">Header</span></span>         | <span data-ttu-id="8d961-123">值</span><span class="sxs-lookup"><span data-stu-id="8d961-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="8d961-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d961-124">Authorization</span></span>  | <span data-ttu-id="8d961-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d961-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8d961-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d961-127">Content-Type</span></span>   | <span data-ttu-id="8d961-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8d961-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="8d961-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d961-129">Request body</span></span>
<span data-ttu-id="8d961-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d961-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d961-131">响应</span><span class="sxs-lookup"><span data-stu-id="8d961-131">Response</span></span>

<span data-ttu-id="8d961-132">如果成功，此方法在响应正文中返回 200 OK 响应代码和 [driveItem](../resources/driveitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d961-132">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d961-133">示例</span><span class="sxs-lookup"><span data-stu-id="8d961-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d961-134">请求</span><span class="sxs-lookup"><span data-stu-id="8d961-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="8d961-135">响应</span><span class="sxs-lookup"><span data-stu-id="8d961-135">Response</span></span>
<span data-ttu-id="8d961-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d961-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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