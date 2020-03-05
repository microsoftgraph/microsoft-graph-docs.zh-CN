---
title: 列出 workingWith
description: 对用户使用的用户列表计算出的洞察力。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cd962184bc655a9df36d6a9b24876a9c1651bcac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451729"
---
# <a name="list-workingwith"></a><span data-ttu-id="82644-103">列出 workingWith</span><span class="sxs-lookup"><span data-stu-id="82644-103">List workingWith</span></span>

<span data-ttu-id="82644-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82644-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82644-105">对用户使用的用户列表计算出的洞察力。</span><span class="sxs-lookup"><span data-stu-id="82644-105">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="82644-106">权限</span><span class="sxs-lookup"><span data-stu-id="82644-106">Permissions</span></span>
<span data-ttu-id="82644-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82644-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82644-109">Permission type</span></span>      | <span data-ttu-id="82644-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82644-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82644-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82644-111">Delegated (work or school account)</span></span> | <span data-ttu-id="82644-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="82644-112">User.Read.All</span></span>    |
|<span data-ttu-id="82644-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82644-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82644-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="82644-114">Not supported.</span></span>    |
|<span data-ttu-id="82644-115">Application</span><span class="sxs-lookup"><span data-stu-id="82644-115">Application</span></span> | <span data-ttu-id="82644-116">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="82644-116">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82644-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82644-117">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82644-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82644-118">Optional query parameters</span></span>
<span data-ttu-id="82644-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82644-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82644-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="82644-120">Request headers</span></span>
| <span data-ttu-id="82644-121">标头</span><span class="sxs-lookup"><span data-stu-id="82644-121">Header</span></span>         | <span data-ttu-id="82644-122">值</span><span class="sxs-lookup"><span data-stu-id="82644-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="82644-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82644-123">Authorization</span></span>  | <span data-ttu-id="82644-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82644-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82644-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82644-126">Content-Type</span></span>   | <span data-ttu-id="82644-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82644-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="82644-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="82644-128">Request body</span></span>
<span data-ttu-id="82644-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82644-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82644-130">响应</span><span class="sxs-lookup"><span data-stu-id="82644-130">Response</span></span>

<span data-ttu-id="82644-131">如果成功，此方法在响应正文中返回 200 OK 响应代码和[User](../resources/user.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="82644-131">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82644-132">示例</span><span class="sxs-lookup"><span data-stu-id="82644-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82644-133">请求</span><span class="sxs-lookup"><span data-stu-id="82644-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="82644-134">响应</span><span class="sxs-lookup"><span data-stu-id="82644-134">Response</span></span>
<span data-ttu-id="82644-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82644-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
