---
title: 列表 trendingAround
description: 返回用户周围趋势分析的项的列表的计算的洞察。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 625ae9d66ce1b891ebdba3209d92bd0e88b06a94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507626"
---
# <a name="list-trendingaround"></a><span data-ttu-id="7c262-103">列表 trendingAround</span><span class="sxs-lookup"><span data-stu-id="7c262-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c262-104">返回用户周围趋势分析的项的列表的计算的洞察。</span><span class="sxs-lookup"><span data-stu-id="7c262-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="7c262-105">**注意：** 此 API 将弃用，替换为[趋势 API](../resources/insights-trending.md)。</span><span class="sxs-lookup"><span data-stu-id="7c262-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c262-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c262-106">Permissions</span></span>
<span data-ttu-id="7c262-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c262-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c262-109">Permission type</span></span>      | <span data-ttu-id="7c262-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c262-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c262-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c262-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7c262-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c262-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="7c262-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c262-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c262-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c262-114">Not supported.</span></span>    |
|<span data-ttu-id="7c262-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c262-115">Application</span></span> | <span data-ttu-id="7c262-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c262-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c262-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c262-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7c262-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7c262-118">Optional query parameters</span></span>
<span data-ttu-id="7c262-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7c262-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c262-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c262-120">Request headers</span></span>
| <span data-ttu-id="7c262-121">标头</span><span class="sxs-lookup"><span data-stu-id="7c262-121">Header</span></span>         | <span data-ttu-id="7c262-122">值</span><span class="sxs-lookup"><span data-stu-id="7c262-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="7c262-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c262-123">Authorization</span></span>  | <span data-ttu-id="7c262-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c262-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7c262-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c262-126">Content-Type</span></span>   | <span data-ttu-id="7c262-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c262-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="7c262-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c262-128">Request body</span></span>
<span data-ttu-id="7c262-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c262-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c262-130">响应</span><span class="sxs-lookup"><span data-stu-id="7c262-130">Response</span></span>

<span data-ttu-id="7c262-131">如果成功，此方法将在响应正文中返回的 200 OK 响应代码和[driveItem](../resources/driveitem.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="7c262-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c262-132">示例</span><span class="sxs-lookup"><span data-stu-id="7c262-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c262-133">请求</span><span class="sxs-lookup"><span data-stu-id="7c262-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="7c262-134">响应</span><span class="sxs-lookup"><span data-stu-id="7c262-134">Response</span></span>
<span data-ttu-id="7c262-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c262-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-trendingaround.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
