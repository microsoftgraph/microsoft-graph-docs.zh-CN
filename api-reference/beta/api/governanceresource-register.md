---
title: governanceResource： register
description: 在 PIM 中注册 governanceResource 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 207a733e72dcf7c05c6cdf81dddb3cecf37e3bdd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991171"
---
# <a name="governanceresource-register"></a><span data-ttu-id="35e18-103">governanceResource： register</span><span class="sxs-lookup"><span data-stu-id="35e18-103">governanceResource: register</span></span>

<span data-ttu-id="35e18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35e18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35e18-105">在特权标识管理中注册 [governanceResource](../resources/governanceresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35e18-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="35e18-106">权限</span><span class="sxs-lookup"><span data-stu-id="35e18-106">Permissions</span></span>

<span data-ttu-id="35e18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35e18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="35e18-109">**注意：** 此 API 还要求请求者在资源上至少有一个活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="35e18-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="35e18-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35e18-110">Permission type</span></span> | <span data-ttu-id="35e18-111">权限</span><span class="sxs-lookup"><span data-stu-id="35e18-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="35e18-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35e18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35e18-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="35e18-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="35e18-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35e18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35e18-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35e18-115">Not supported.</span></span> |
| <span data-ttu-id="35e18-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="35e18-116">Application</span></span> | <span data-ttu-id="35e18-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="35e18-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35e18-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35e18-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35e18-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35e18-119">Optional query parameters</span></span>

<span data-ttu-id="35e18-120">此方法 **仅** 支持 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35e18-120">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35e18-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="35e18-121">Request headers</span></span>

| <span data-ttu-id="35e18-122">名称</span><span class="sxs-lookup"><span data-stu-id="35e18-122">Name</span></span> | <span data-ttu-id="35e18-123">说明</span><span class="sxs-lookup"><span data-stu-id="35e18-123">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="35e18-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="35e18-124">Authorization</span></span> | <span data-ttu-id="35e18-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="35e18-125">Bearer {token}</span></span> |
| <span data-ttu-id="35e18-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="35e18-126">Content-type</span></span> | <span data-ttu-id="35e18-127">application/json</span><span class="sxs-lookup"><span data-stu-id="35e18-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="35e18-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="35e18-128">Request body</span></span>

| <span data-ttu-id="35e18-129">属性</span><span class="sxs-lookup"><span data-stu-id="35e18-129">Properties</span></span> | <span data-ttu-id="35e18-130">类型</span><span class="sxs-lookup"><span data-stu-id="35e18-130">Type</span></span> | <span data-ttu-id="35e18-131">说明</span><span class="sxs-lookup"><span data-stu-id="35e18-131">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="35e18-132">externalId</span><span class="sxs-lookup"><span data-stu-id="35e18-132">externalId</span></span> | <span data-ttu-id="35e18-133">String</span><span class="sxs-lookup"><span data-stu-id="35e18-133">String</span></span> | <span data-ttu-id="35e18-134">要在 PIM 中注册的资源的外部标识符。</span><span class="sxs-lookup"><span data-stu-id="35e18-134">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="35e18-135">如果注册订阅，则标识符为预置的订阅标识符 `/subscriptions/` 。</span><span class="sxs-lookup"><span data-stu-id="35e18-135">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="35e18-136">例如，`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`。</span><span class="sxs-lookup"><span data-stu-id="35e18-136">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="35e18-137">响应</span><span class="sxs-lookup"><span data-stu-id="35e18-137">Response</span></span>

<span data-ttu-id="35e18-138">如果成功，此方法将返回 `200 OK` 响应。</span><span class="sxs-lookup"><span data-stu-id="35e18-138">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="35e18-139">示例</span><span class="sxs-lookup"><span data-stu-id="35e18-139">Example</span></span>

<span data-ttu-id="35e18-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="35e18-140">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="35e18-141">请求</span><span class="sxs-lookup"><span data-stu-id="35e18-141">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="35e18-142">响应</span><span class="sxs-lookup"><span data-stu-id="35e18-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


