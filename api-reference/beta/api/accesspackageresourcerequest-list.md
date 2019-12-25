---
title: 列出 accessPackageResourceRequests
description: 检索 accessPackageResourceRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9cc83456021c3e10db5fbe1666d7696e8270507
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871746"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="b4297-103">列出 accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="b4297-103">List accessPackageResourceRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4297-104">检索[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b4297-104">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4297-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4297-105">Permissions</span></span>

<span data-ttu-id="b4297-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4297-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4297-108">Permission type</span></span>                        | <span data-ttu-id="b4297-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4297-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4297-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4297-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="b4297-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4297-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b4297-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4297-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4297-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4297-113">Not supported.</span></span> |
| <span data-ttu-id="b4297-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4297-114">Application</span></span>                            | <span data-ttu-id="b4297-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4297-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4297-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4297-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4297-117">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="b4297-117">Optional query parameters</span></span>

<span data-ttu-id="b4297-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4297-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b4297-119">例如，若要检索请求将资源添加到目录中的谁，请在`$expand=requestor`查询中加入。</span><span class="sxs-lookup"><span data-stu-id="b4297-119">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="b4297-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b4297-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4297-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4297-121">Request headers</span></span>

| <span data-ttu-id="b4297-122">名称</span><span class="sxs-lookup"><span data-stu-id="b4297-122">Name</span></span>      |<span data-ttu-id="b4297-123">说明</span><span class="sxs-lookup"><span data-stu-id="b4297-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4297-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4297-124">Authorization</span></span> | <span data-ttu-id="b4297-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4297-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4297-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4297-127">Request body</span></span>

<span data-ttu-id="b4297-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4297-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4297-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4297-129">Response</span></span>

<span data-ttu-id="b4297-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b4297-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4297-131">示例</span><span class="sxs-lookup"><span data-stu-id="b4297-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4297-132">请求</span><span class="sxs-lookup"><span data-stu-id="b4297-132">Request</span></span>

<span data-ttu-id="b4297-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4297-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```

### <a name="response"></a><span data-ttu-id="b4297-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4297-134">Response</span></span>

<span data-ttu-id="b4297-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4297-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b4297-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4297-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
