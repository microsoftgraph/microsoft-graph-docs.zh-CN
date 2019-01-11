---
title: 列表 workingWith
description: 计算的洞察力进行的用户使用的用户列表。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: df7f84bf42887d9052cb9d81042b5735af7bd2b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870334"
---
# <a name="list-workingwith"></a><span data-ttu-id="fe020-103">列表 workingWith</span><span class="sxs-lookup"><span data-stu-id="fe020-103">List workingWith</span></span>

> <span data-ttu-id="fe020-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe020-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe020-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe020-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe020-106">计算的洞察力进行的用户使用的用户列表。</span><span class="sxs-lookup"><span data-stu-id="fe020-106">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe020-107">权限</span><span class="sxs-lookup"><span data-stu-id="fe020-107">Permissions</span></span>
<span data-ttu-id="fe020-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe020-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe020-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe020-110">Permission type</span></span>      | <span data-ttu-id="fe020-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe020-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe020-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe020-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe020-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe020-113">User.Read.All</span></span>    |
|<span data-ttu-id="fe020-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe020-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe020-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe020-115">Not supported.</span></span>    |
|<span data-ttu-id="fe020-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe020-116">Application</span></span> | <span data-ttu-id="fe020-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe020-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe020-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe020-118">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe020-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe020-119">Optional query parameters</span></span>
<span data-ttu-id="fe020-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe020-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe020-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe020-121">Request headers</span></span>
| <span data-ttu-id="fe020-122">标头</span><span class="sxs-lookup"><span data-stu-id="fe020-122">Header</span></span>         | <span data-ttu-id="fe020-123">值</span><span class="sxs-lookup"><span data-stu-id="fe020-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="fe020-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe020-124">Authorization</span></span>  | <span data-ttu-id="fe020-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe020-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe020-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe020-127">Content-Type</span></span>   | <span data-ttu-id="fe020-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fe020-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="fe020-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe020-129">Request body</span></span>
<span data-ttu-id="fe020-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe020-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe020-131">响应</span><span class="sxs-lookup"><span data-stu-id="fe020-131">Response</span></span>

<span data-ttu-id="fe020-132">如果成功，此方法将在响应正文中返回的 200 OK 响应代码和[用户](../resources/user.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="fe020-132">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe020-133">示例</span><span class="sxs-lookup"><span data-stu-id="fe020-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe020-134">请求</span><span class="sxs-lookup"><span data-stu-id="fe020-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="fe020-135">响应</span><span class="sxs-lookup"><span data-stu-id="fe020-135">Response</span></span>
<span data-ttu-id="fe020-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe020-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```
