---
title: 创建架构
description: 为连接创建Microsoft 搜索架构。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 98c4c83ff8a8712905ace9fa80ec4fdae0de7180
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467283"
---
# <a name="create-schema"></a><span data-ttu-id="1ff7f-103">创建架构</span><span class="sxs-lookup"><span data-stu-id="1ff7f-103">Create schema</span></span>
<span data-ttu-id="1ff7f-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="1ff7f-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="1ff7f-105">创建新的 [架构](../resources/externalconnectors-schema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-105">Create a new [schema](../resources/externalconnectors-schema.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ff7f-106">权限</span><span class="sxs-lookup"><span data-stu-id="1ff7f-106">Permissions</span></span>
<span data-ttu-id="1ff7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff7f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ff7f-109">Permission type</span></span>|<span data-ttu-id="1ff7f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ff7f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ff7f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff7f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ff7f-112">不适用</span><span class="sxs-lookup"><span data-stu-id="1ff7f-112">Not applicable</span></span>|
|<span data-ttu-id="1ff7f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ff7f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ff7f-114">不适用</span><span class="sxs-lookup"><span data-stu-id="1ff7f-114">Not applicable</span></span>|
|<span data-ttu-id="1ff7f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ff7f-115">Application</span></span>| <span data-ttu-id="1ff7f-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1ff7f-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff7f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ff7f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /external/connections/{id}/schema
```
<span data-ttu-id="1ff7f-118">在请求正文中，提供架构对象的 JSON [表示](../resources/externalconnectors-schema.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-118">In the request body, supply a JSON representation of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

<span data-ttu-id="1ff7f-119">注册自定义项架构时， `schema` 对象必须将 `baseType` 属性设置为 `microsoft.graph.externalItem` ，并且必须包含 `properties` 属性。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-119">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="1ff7f-120">`properties`对象必须至少包含一个属性，最多包含 64 个属性。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-120">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="1ff7f-121">响应</span><span class="sxs-lookup"><span data-stu-id="1ff7f-121">Response</span></span>

<span data-ttu-id="1ff7f-122">在请求中包含 标头后，如果成功，此方法在响应标头中返回 响应代码和 `Prefer: respond-async` `202 Accepted` URL，可用于 `Location` [获取操作状态](../api/externalconnectors-connectionoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-122">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/externalconnectors-connectionoperation-get.md).</span></span>

<span data-ttu-id="1ff7f-123">如果请求中不包含 标头，如果成功，此方法在响应正文中返回 响应 `Prefer: respond-async` `201 Created` 代码和新[](../resources/externalconnectors-schema.md)架构对象。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-123">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="1ff7f-124">创建架构是一个长时间运行的过程，容易出现网关超时。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-124">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="1ff7f-125">我们建议使用 `Prefer: respond-async` 标头以避免超时错误。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-125">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="1ff7f-126">示例</span><span class="sxs-lookup"><span data-stu-id="1ff7f-126">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="1ff7f-127">示例：异步注册自定义架构</span><span class="sxs-lookup"><span data-stu-id="1ff7f-127">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="1ff7f-128">请求</span><span class="sxs-lookup"><span data-stu-id="1ff7f-128">Request</span></span>

<span data-ttu-id="1ff7f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff7f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff7f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}-->

```http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="1ff7f-131">响应</span><span class="sxs-lookup"><span data-stu-id="1ff7f-131">Response</span></span>

<span data-ttu-id="1ff7f-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ff7f-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```
