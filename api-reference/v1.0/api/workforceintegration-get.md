---
title: 获取工作人员集成
description: 检索 workforceIntegration 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 53cd0ca961a407c0cf8e20153e25a8bf2a3cf0f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049350"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="6cf70-103">获取工作人员集成</span><span class="sxs-lookup"><span data-stu-id="6cf70-103">Get workforceIntegration</span></span>

<span data-ttu-id="6cf70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cf70-105">检索 [workforceIntegration](../resources/workforceintegration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cf70-105">Retrieve the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cf70-106">权限</span><span class="sxs-lookup"><span data-stu-id="6cf70-106">Permissions</span></span>

<span data-ttu-id="6cf70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cf70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cf70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cf70-109">Permission type</span></span>                        | <span data-ttu-id="6cf70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cf70-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6cf70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cf70-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cf70-112">WorkforceIntegration.Read.All、WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf70-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="6cf70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cf70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cf70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cf70-114">Not supported.</span></span> |
| <span data-ttu-id="6cf70-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cf70-115">Application</span></span>                            | <span data-ttu-id="6cf70-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cf70-116">Not supported.</span></span> |

> <span data-ttu-id="6cf70-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6cf70-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6cf70-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="6cf70-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6cf70-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cf70-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cf70-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6cf70-120">Optional query parameters</span></span>

<span data-ttu-id="6cf70-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6cf70-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6cf70-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6cf70-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cf70-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cf70-123">Request headers</span></span>

| <span data-ttu-id="6cf70-124">名称</span><span class="sxs-lookup"><span data-stu-id="6cf70-124">Name</span></span>      |<span data-ttu-id="6cf70-125">说明</span><span class="sxs-lookup"><span data-stu-id="6cf70-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6cf70-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cf70-126">Authorization</span></span> | <span data-ttu-id="6cf70-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cf70-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cf70-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cf70-129">Request body</span></span>

<span data-ttu-id="6cf70-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cf70-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cf70-131">响应</span><span class="sxs-lookup"><span data-stu-id="6cf70-131">Response</span></span>

<span data-ttu-id="6cf70-132">如果成功，此方法在响应正文中返回 响应代码和请求 `200 OK` [的 workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6cf70-132">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cf70-133">示例</span><span class="sxs-lookup"><span data-stu-id="6cf70-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6cf70-134">请求</span><span class="sxs-lookup"><span data-stu-id="6cf70-134">Request</span></span>

<span data-ttu-id="6cf70-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6cf70-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6cf70-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf70-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="6cf70-137">C#</span><span class="sxs-lookup"><span data-stu-id="6cf70-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cf70-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cf70-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cf70-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cf70-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cf70-140">Java</span><span class="sxs-lookup"><span data-stu-id="6cf70-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6cf70-141">响应</span><span class="sxs-lookup"><span data-stu-id="6cf70-141">Response</span></span>

<span data-ttu-id="6cf70-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6cf70-142">The following is an example of the response.</span></span>

> <span data-ttu-id="6cf70-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6cf70-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supportedEntities": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

