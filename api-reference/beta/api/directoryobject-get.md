---
title: 获取 directoryObject
description: 检索的属性和 directoryobject 对象的关系。
ms.openlocfilehash: ed1e765cb7cbde38cbb47a8dfdd58b018d142e7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046030"
---
# <a name="get-directoryobject"></a><span data-ttu-id="a55a3-103">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="a55a3-103">Get directoryObject</span></span>

> <span data-ttu-id="a55a3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a55a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a55a3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a55a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a55a3-106">检索的属性和 directoryobject 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a55a3-106">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a55a3-107">权限</span><span class="sxs-lookup"><span data-stu-id="a55a3-107">Permissions</span></span>
<span data-ttu-id="a55a3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a55a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a55a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a55a3-110">Permission type</span></span>      | <span data-ttu-id="a55a3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a55a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a55a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a55a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a55a3-113">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a55a3-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a55a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a55a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a55a3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a55a3-115">Not supported.</span></span>    |
|<span data-ttu-id="a55a3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a55a3-116">Application</span></span> | <span data-ttu-id="a55a3-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a55a3-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a55a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a55a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a55a3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a55a3-119">Optional query parameters</span></span>
<span data-ttu-id="a55a3-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a55a3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a55a3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a55a3-121">Request headers</span></span>
| <span data-ttu-id="a55a3-122">名称</span><span class="sxs-lookup"><span data-stu-id="a55a3-122">Name</span></span>       | <span data-ttu-id="a55a3-123">类型</span><span class="sxs-lookup"><span data-stu-id="a55a3-123">Type</span></span> | <span data-ttu-id="a55a3-124">说明</span><span class="sxs-lookup"><span data-stu-id="a55a3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a55a3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a55a3-125">Authorization</span></span>  | <span data-ttu-id="a55a3-126">string</span><span class="sxs-lookup"><span data-stu-id="a55a3-126">string</span></span>  | <span data-ttu-id="a55a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a55a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a55a3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a55a3-129">Request body</span></span>
<span data-ttu-id="a55a3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a55a3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a55a3-131">响应</span><span class="sxs-lookup"><span data-stu-id="a55a3-131">Response</span></span>

<span data-ttu-id="a55a3-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a55a3-132">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a55a3-133">示例</span><span class="sxs-lookup"><span data-stu-id="a55a3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a55a3-134">请求</span><span class="sxs-lookup"><span data-stu-id="a55a3-134">Request</span></span>
<span data-ttu-id="a55a3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a55a3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="a55a3-136">响应</span><span class="sxs-lookup"><span data-stu-id="a55a3-136">Response</span></span>
<span data-ttu-id="a55a3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a55a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
