---
title: 列出域
description: 检索 domain 对象列表。
author: lleonard-msft
ms.openlocfilehash: ec8598daf47907dd409af0fa58af0dd7d7abf47c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308804"
---
# <a name="list-domains"></a><span data-ttu-id="65d4a-103">列出域</span><span class="sxs-lookup"><span data-stu-id="65d4a-103">List domains</span></span>

> <span data-ttu-id="65d4a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="65d4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65d4a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65d4a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65d4a-106">检索 domain 对象列表。</span><span class="sxs-lookup"><span data-stu-id="65d4a-106">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="65d4a-107">权限</span><span class="sxs-lookup"><span data-stu-id="65d4a-107">Permissions</span></span>
<span data-ttu-id="65d4a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65d4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d4a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="65d4a-110">Permission type</span></span>      | <span data-ttu-id="65d4a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65d4a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65d4a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65d4a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65d4a-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="65d4a-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="65d4a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65d4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d4a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65d4a-115">Not supported.</span></span>    |
|<span data-ttu-id="65d4a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65d4a-116">Application</span></span> | <span data-ttu-id="65d4a-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d4a-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65d4a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65d4a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65d4a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="65d4a-119">Optional query parameters</span></span>
<span data-ttu-id="65d4a-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="65d4a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65d4a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="65d4a-121">Request headers</span></span>
| <span data-ttu-id="65d4a-122">Name</span><span class="sxs-lookup"><span data-stu-id="65d4a-122">Name</span></span>      |<span data-ttu-id="65d4a-123">说明</span><span class="sxs-lookup"><span data-stu-id="65d4a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="65d4a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="65d4a-124">Authorization</span></span>  | <span data-ttu-id="65d4a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65d4a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="65d4a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="65d4a-127">Accept</span></span>         | <span data-ttu-id="65d4a-128">application/json；</span><span class="sxs-lookup"><span data-stu-id="65d4a-128">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="65d4a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="65d4a-129">Request body</span></span>
<span data-ttu-id="65d4a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65d4a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65d4a-131">响应</span><span class="sxs-lookup"><span data-stu-id="65d4a-131">Response</span></span>

<span data-ttu-id="65d4a-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="65d4a-132">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65d4a-133">示例</span><span class="sxs-lookup"><span data-stu-id="65d4a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65d4a-134">请求</span><span class="sxs-lookup"><span data-stu-id="65d4a-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
##### <a name="response"></a><span data-ttu-id="65d4a-135">响应</span><span class="sxs-lookup"><span data-stu-id="65d4a-135">Response</span></span>
<span data-ttu-id="65d4a-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65d4a-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->