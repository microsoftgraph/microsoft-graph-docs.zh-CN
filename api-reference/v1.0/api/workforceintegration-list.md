---
title: 列出 workforceIntegrations
description: 检索 workforceIntegration 对象的列表。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5e37feb028e5929bdb48ccf54b62083de9cbc9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154043"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="8b557-103">列出 workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="8b557-103">List workforceIntegrations</span></span>

<span data-ttu-id="8b557-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b557-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b557-105">检索[workforceIntegration](../resources/workforceintegration.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8b557-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b557-106">权限</span><span class="sxs-lookup"><span data-stu-id="8b557-106">Permissions</span></span>

<span data-ttu-id="8b557-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b557-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b557-109">Permission type</span></span>                        | <span data-ttu-id="8b557-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b557-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b557-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b557-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="8b557-112">WorkforceIntegration、WorkforceIntegration 和所有</span><span class="sxs-lookup"><span data-stu-id="8b557-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="8b557-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b557-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b557-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b557-114">Not supported.</span></span> |
| <span data-ttu-id="8b557-115">Application</span><span class="sxs-lookup"><span data-stu-id="8b557-115">Application</span></span>                            | <span data-ttu-id="8b557-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b557-116">Not supported.</span></span> |

> <span data-ttu-id="8b557-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="8b557-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8b557-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="8b557-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="8b557-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b557-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b557-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8b557-120">Optional query parameters</span></span>

<span data-ttu-id="8b557-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8b557-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8b557-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8b557-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b557-123">请求头</span><span class="sxs-lookup"><span data-stu-id="8b557-123">Request headers</span></span>

| <span data-ttu-id="8b557-124">名称</span><span class="sxs-lookup"><span data-stu-id="8b557-124">Name</span></span>      |<span data-ttu-id="8b557-125">说明</span><span class="sxs-lookup"><span data-stu-id="8b557-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b557-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b557-126">Authorization</span></span> | <span data-ttu-id="8b557-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b557-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b557-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b557-129">Request body</span></span>

<span data-ttu-id="8b557-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b557-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b557-131">响应</span><span class="sxs-lookup"><span data-stu-id="8b557-131">Response</span></span>

<span data-ttu-id="8b557-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workforceIntegration](../resources/workforceintegration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8b557-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b557-133">示例</span><span class="sxs-lookup"><span data-stu-id="8b557-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b557-134">请求</span><span class="sxs-lookup"><span data-stu-id="8b557-134">Request</span></span>

<span data-ttu-id="8b557-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8b557-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```

---


### <a name="response"></a><span data-ttu-id="8b557-136">响应</span><span class="sxs-lookup"><span data-stu-id="8b557-136">Response</span></span>

<span data-ttu-id="8b557-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8b557-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8b557-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8b557-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supportedEntities": "supportedEntities-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
