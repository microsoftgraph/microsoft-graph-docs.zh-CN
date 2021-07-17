---
title: 创建 externalItem
description: 创建新的 externalItem。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: eba04bf339eeed41f9fe59831773d413bbed3111
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467212"
---
# <a name="create-externalitem"></a><span data-ttu-id="6617d-103">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="6617d-103">Create externalItem</span></span>

<span data-ttu-id="6617d-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="6617d-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="6617d-105">创建新的 [externalItem](../resources/externalconnectors-externalitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6617d-105">Create a new [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6617d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6617d-106">Permissions</span></span>
<span data-ttu-id="6617d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6617d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6617d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6617d-109">Permission type</span></span>|<span data-ttu-id="6617d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6617d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6617d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6617d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6617d-112">不适用</span><span class="sxs-lookup"><span data-stu-id="6617d-112">Not applicable</span></span>|
|<span data-ttu-id="6617d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6617d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6617d-114">不适用</span><span class="sxs-lookup"><span data-stu-id="6617d-114">Not applicable</span></span>|
|<span data-ttu-id="6617d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6617d-115">Application</span></span>| <span data-ttu-id="6617d-116">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6617d-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6617d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6617d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/items
```

## <a name="request-headers"></a><span data-ttu-id="6617d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6617d-118">Request headers</span></span>
|<span data-ttu-id="6617d-119">名称</span><span class="sxs-lookup"><span data-stu-id="6617d-119">Name</span></span>|<span data-ttu-id="6617d-120">说明</span><span class="sxs-lookup"><span data-stu-id="6617d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6617d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6617d-121">Authorization</span></span>|<span data-ttu-id="6617d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6617d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6617d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6617d-124">Content-Type</span></span>|<span data-ttu-id="6617d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6617d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6617d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6617d-127">Request body</span></span>
<span data-ttu-id="6617d-128">在请求正文中，提供 [externalItem](../resources/externalconnectors-externalitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6617d-128">In the request body, supply a JSON representation of the [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

<span data-ttu-id="6617d-129">下表显示创建 [externalItem 时所需的属性](../resources/externalconnectors-externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6617d-129">The following table shows the properties that are required when you create the [externalItem](../resources/externalconnectors-externalitem.md).</span></span>

|<span data-ttu-id="6617d-130">属性</span><span class="sxs-lookup"><span data-stu-id="6617d-130">Property</span></span>|<span data-ttu-id="6617d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6617d-131">Type</span></span>| <span data-ttu-id="6617d-132">必需 (Y/N) </span><span class="sxs-lookup"><span data-stu-id="6617d-132">Required (Y/N)</span></span> | <span data-ttu-id="6617d-133">说明</span><span class="sxs-lookup"><span data-stu-id="6617d-133">Description</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="6617d-134">id</span><span class="sxs-lookup"><span data-stu-id="6617d-134">id</span></span>|<span data-ttu-id="6617d-135">String</span><span class="sxs-lookup"><span data-stu-id="6617d-135">String</span></span>|<span data-ttu-id="6617d-136">Y</span><span class="sxs-lookup"><span data-stu-id="6617d-136">Y</span></span>|<span data-ttu-id="6617d-137">项目 ID</span><span class="sxs-lookup"><span data-stu-id="6617d-137">The item ID</span></span>|
|<span data-ttu-id="6617d-138">properties</span><span class="sxs-lookup"><span data-stu-id="6617d-138">properties</span></span>|[<span data-ttu-id="6617d-139">microsoft.graph.externalConnectors.properties</span><span class="sxs-lookup"><span data-stu-id="6617d-139">microsoft.graph.externalConnectors.properties</span></span>](../resources/externalconnectors-properties.md)|<span data-ttu-id="6617d-140">Y</span><span class="sxs-lookup"><span data-stu-id="6617d-140">Y</span></span>|<span data-ttu-id="6617d-141">项目属性。</span><span class="sxs-lookup"><span data-stu-id="6617d-141">The item properties.</span></span> <span data-ttu-id="6617d-142">`properties`对象必须至少包含一个属性。</span><span class="sxs-lookup"><span data-stu-id="6617d-142">The `properties` object must contain at least one property.</span></span> <span data-ttu-id="6617d-143">所有 `DateTime` 类型属性都必须采用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="6617d-143">All `DateTime` type properties must be in ISO 8601 format.</span></span>|
|<span data-ttu-id="6617d-144">content</span><span class="sxs-lookup"><span data-stu-id="6617d-144">content</span></span>|[<span data-ttu-id="6617d-145">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="6617d-145">microsoft.graph.externalConnectors.externalItemContent</span></span>](../resources/externalconnectors-externalitemcontent.md)|<span data-ttu-id="6617d-146">N</span><span class="sxs-lookup"><span data-stu-id="6617d-146">N</span></span>|<span data-ttu-id="6617d-147">外部项内容</span><span class="sxs-lookup"><span data-stu-id="6617d-147">The external item content</span></span>|
|<span data-ttu-id="6617d-148">acl</span><span class="sxs-lookup"><span data-stu-id="6617d-148">acl</span></span>|<span data-ttu-id="6617d-149">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6617d-149">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) collection</span></span>|<span data-ttu-id="6617d-150">Y</span><span class="sxs-lookup"><span data-stu-id="6617d-150">Y</span></span>|<span data-ttu-id="6617d-151">访问控制列表</span><span class="sxs-lookup"><span data-stu-id="6617d-151">The access control list</span></span>|

<span data-ttu-id="6617d-152">在下列 `externalItem` 情况下，上的 属性应在有效负载中使用类型说明符：</span><span class="sxs-lookup"><span data-stu-id="6617d-152">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="6617d-153">对于 `String` 类型属性，如果值包含非 ASCII 字符。</span><span class="sxs-lookup"><span data-stu-id="6617d-153">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="6617d-154">对于所有集合类型。</span><span class="sxs-lookup"><span data-stu-id="6617d-154">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="6617d-155">当包含 类型的 属性 `Collection(DateTime)` 时，必须使用类型说明器 `Collection(DateTimeOffset)` 。</span><span class="sxs-lookup"><span data-stu-id="6617d-155">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="6617d-156">响应</span><span class="sxs-lookup"><span data-stu-id="6617d-156">Response</span></span> 

<span data-ttu-id="6617d-157">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6617d-157">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6617d-158">示例</span><span class="sxs-lookup"><span data-stu-id="6617d-158">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="6617d-159">示例：创建自定义项</span><span class="sxs-lookup"><span data-stu-id="6617d-159">Example: Create a custom item</span></span>

### <a name="request"></a><span data-ttu-id="6617d-160">请求</span><span class="sxs-lookup"><span data-stu-id="6617d-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```


### <a name="response"></a><span data-ttu-id="6617d-161">响应</span><span class="sxs-lookup"><span data-stu-id="6617d-161">Response</span></span>

<span data-ttu-id="6617d-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6617d-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

