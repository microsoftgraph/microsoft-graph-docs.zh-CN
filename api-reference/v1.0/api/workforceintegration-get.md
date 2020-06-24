---
title: 获取 workforceIntegration
description: 检索 workforceIntegration 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa08c99cdca34a9561c81e0f90ac4f61fdb15871
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845755"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="59732-103">获取 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="59732-103">Get workforceIntegration</span></span>

<span data-ttu-id="59732-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59732-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59732-105">检索[workforceIntegration](../resources/workforceintegration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59732-105">Retrieve the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59732-106">权限</span><span class="sxs-lookup"><span data-stu-id="59732-106">Permissions</span></span>

<span data-ttu-id="59732-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="59732-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="59732-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59732-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59732-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="59732-109">Permission type</span></span>                        | <span data-ttu-id="59732-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59732-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59732-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59732-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="59732-112">WorkforceIntegration、WorkforceIntegration 和所有</span><span class="sxs-lookup"><span data-stu-id="59732-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="59732-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59732-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59732-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="59732-114">Not supported.</span></span> |
| <span data-ttu-id="59732-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="59732-115">Application</span></span>                            | <span data-ttu-id="59732-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59732-116">Not supported.</span></span> |

> <span data-ttu-id="59732-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="59732-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="59732-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="59732-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="59732-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59732-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59732-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59732-120">Optional query parameters</span></span>

<span data-ttu-id="59732-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59732-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="59732-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="59732-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="59732-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="59732-123">Request headers</span></span>

| <span data-ttu-id="59732-124">名称</span><span class="sxs-lookup"><span data-stu-id="59732-124">Name</span></span>      |<span data-ttu-id="59732-125">说明</span><span class="sxs-lookup"><span data-stu-id="59732-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59732-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="59732-126">Authorization</span></span> | <span data-ttu-id="59732-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="59732-127">Bearer {token}.</span></span> <span data-ttu-id="59732-128">Required.</span><span class="sxs-lookup"><span data-stu-id="59732-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59732-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="59732-129">Request body</span></span>

<span data-ttu-id="59732-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59732-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59732-131">响应</span><span class="sxs-lookup"><span data-stu-id="59732-131">Response</span></span>

<span data-ttu-id="59732-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59732-132">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59732-133">示例</span><span class="sxs-lookup"><span data-stu-id="59732-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59732-134">请求</span><span class="sxs-lookup"><span data-stu-id="59732-134">Request</span></span>

<span data-ttu-id="59732-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59732-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="59732-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="59732-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="59732-137">C#</span><span class="sxs-lookup"><span data-stu-id="59732-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59732-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59732-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59732-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59732-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59732-140">Java</span><span class="sxs-lookup"><span data-stu-id="59732-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="59732-141">响应</span><span class="sxs-lookup"><span data-stu-id="59732-141">Response</span></span>

<span data-ttu-id="59732-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="59732-142">The following is an example of the response.</span></span>

> <span data-ttu-id="59732-143">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="59732-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59732-144">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="59732-144">All the properties will be returned from an actual call.</span></span>

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
