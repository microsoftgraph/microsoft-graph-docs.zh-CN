---
title: 获取 workforceIntegration
description: 检索 workforceintegration 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2738959b356faba1d6d27ae48fa94dcf6f28dbe9
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895579"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="720b5-103">获取 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="720b5-103">Get workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="720b5-104">检索[workforceintegration](../resources/workforceintegration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="720b5-104">Retrieve the properties and relationships of [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="720b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="720b5-105">Permissions</span></span>

<span data-ttu-id="720b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="720b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="720b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="720b5-108">Permission type</span></span>                        | <span data-ttu-id="720b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="720b5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="720b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="720b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="720b5-111">WorkforceIntegration、WorkforceIntegration 和所有</span><span class="sxs-lookup"><span data-stu-id="720b5-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="720b5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="720b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="720b5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="720b5-113">Not supported.</span></span> |
| <span data-ttu-id="720b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="720b5-114">Application</span></span>                            | <span data-ttu-id="720b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="720b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="720b5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="720b5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="720b5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="720b5-117">Optional query parameters</span></span>

<span data-ttu-id="720b5-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="720b5-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="720b5-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="720b5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="720b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="720b5-120">Request headers</span></span>

| <span data-ttu-id="720b5-121">名称</span><span class="sxs-lookup"><span data-stu-id="720b5-121">Name</span></span>      |<span data-ttu-id="720b5-122">说明</span><span class="sxs-lookup"><span data-stu-id="720b5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="720b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="720b5-123">Authorization</span></span> | <span data-ttu-id="720b5-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="720b5-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="720b5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="720b5-125">Request body</span></span>

<span data-ttu-id="720b5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="720b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="720b5-127">响应</span><span class="sxs-lookup"><span data-stu-id="720b5-127">Response</span></span>

<span data-ttu-id="720b5-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="720b5-128">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="720b5-129">示例</span><span class="sxs-lookup"><span data-stu-id="720b5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="720b5-130">请求</span><span class="sxs-lookup"><span data-stu-id="720b5-130">Request</span></span>

<span data-ttu-id="720b5-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="720b5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```

### <a name="response"></a><span data-ttu-id="720b5-132">响应</span><span class="sxs-lookup"><span data-stu-id="720b5-132">Response</span></span>

<span data-ttu-id="720b5-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="720b5-133">The following is an example of the response.</span></span>

> <span data-ttu-id="720b5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="720b5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "supports": "shift"
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