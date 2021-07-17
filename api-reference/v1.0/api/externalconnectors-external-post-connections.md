---
title: 创建 externalConnection
description: 创建新的 externalConnection 对象。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d556b4925625ac929c1b13f6559c048de1b55366
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467213"
---
# <a name="create-externalconnection"></a><span data-ttu-id="b34ff-103">创建 externalConnection</span><span class="sxs-lookup"><span data-stu-id="b34ff-103">Create externalConnection</span></span>
<span data-ttu-id="b34ff-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b34ff-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="b34ff-105">创建新的 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="b34ff-105">Create a new externalConnection object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b34ff-106">权限</span><span class="sxs-lookup"><span data-stu-id="b34ff-106">Permissions</span></span>
<span data-ttu-id="b34ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b34ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b34ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b34ff-109">Permission type</span></span>|<span data-ttu-id="b34ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b34ff-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b34ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b34ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b34ff-112">不适用</span><span class="sxs-lookup"><span data-stu-id="b34ff-112">Not applicable</span></span>|
|<span data-ttu-id="b34ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b34ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b34ff-114">不适用</span><span class="sxs-lookup"><span data-stu-id="b34ff-114">Not applicable</span></span>|
|<span data-ttu-id="b34ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b34ff-115">Application</span></span>| <span data-ttu-id="b34ff-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b34ff-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="b34ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b34ff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="b34ff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b34ff-118">Request headers</span></span>
|<span data-ttu-id="b34ff-119">名称</span><span class="sxs-lookup"><span data-stu-id="b34ff-119">Name</span></span>|<span data-ttu-id="b34ff-120">说明</span><span class="sxs-lookup"><span data-stu-id="b34ff-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b34ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b34ff-121">Authorization</span></span>|<span data-ttu-id="b34ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b34ff-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b34ff-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b34ff-124">Content-Type</span></span>|<span data-ttu-id="b34ff-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b34ff-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b34ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b34ff-127">Request body</span></span>
<span data-ttu-id="b34ff-128">在请求正文中，提供 [externalConnection](../resources/externalconnectors-externalconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b34ff-128">In the request body, supply a JSON representation of the [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

<span data-ttu-id="b34ff-129">下表显示创建 [externalConnection](../resources/externalconnectors-externalconnection.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b34ff-129">The following table shows the properties that are required when you create the [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

|<span data-ttu-id="b34ff-130">属性</span><span class="sxs-lookup"><span data-stu-id="b34ff-130">Property</span></span>|<span data-ttu-id="b34ff-131">类型</span><span class="sxs-lookup"><span data-stu-id="b34ff-131">Type</span></span>|<span data-ttu-id="b34ff-132">必需 (Y/N) </span><span class="sxs-lookup"><span data-stu-id="b34ff-132">Required (Y/N)</span></span> |<span data-ttu-id="b34ff-133">说明</span><span class="sxs-lookup"><span data-stu-id="b34ff-133">Description</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="b34ff-134">id</span><span class="sxs-lookup"><span data-stu-id="b34ff-134">id</span></span>|<span data-ttu-id="b34ff-135">String</span><span class="sxs-lookup"><span data-stu-id="b34ff-135">String</span></span>|<span data-ttu-id="b34ff-136">Y</span><span class="sxs-lookup"><span data-stu-id="b34ff-136">Y</span></span>|<span data-ttu-id="b34ff-137">连接 ID</span><span class="sxs-lookup"><span data-stu-id="b34ff-137">The connection ID</span></span>|
|<span data-ttu-id="b34ff-138">name</span><span class="sxs-lookup"><span data-stu-id="b34ff-138">name</span></span>|<span data-ttu-id="b34ff-139">String</span><span class="sxs-lookup"><span data-stu-id="b34ff-139">String</span></span>|<span data-ttu-id="b34ff-140">Y</span><span class="sxs-lookup"><span data-stu-id="b34ff-140">Y</span></span>|<span data-ttu-id="b34ff-141">连接名称</span><span class="sxs-lookup"><span data-stu-id="b34ff-141">The connection name</span></span>|
|<span data-ttu-id="b34ff-142">说明</span><span class="sxs-lookup"><span data-stu-id="b34ff-142">description</span></span>|<span data-ttu-id="b34ff-143">String</span><span class="sxs-lookup"><span data-stu-id="b34ff-143">String</span></span>|<span data-ttu-id="b34ff-144">Y</span><span class="sxs-lookup"><span data-stu-id="b34ff-144">Y</span></span>|<span data-ttu-id="b34ff-145">连接说明</span><span class="sxs-lookup"><span data-stu-id="b34ff-145">The connection description</span></span>|
|<span data-ttu-id="b34ff-146">configuration</span><span class="sxs-lookup"><span data-stu-id="b34ff-146">configuration</span></span>|[<span data-ttu-id="b34ff-147">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="b34ff-147">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md)|<span data-ttu-id="b34ff-148">N</span><span class="sxs-lookup"><span data-stu-id="b34ff-148">N</span></span>|<span data-ttu-id="b34ff-149">连接配置</span><span class="sxs-lookup"><span data-stu-id="b34ff-149">The connection configurations</span></span>|



## <a name="response"></a><span data-ttu-id="b34ff-150">响应</span><span class="sxs-lookup"><span data-stu-id="b34ff-150">Response</span></span>

<span data-ttu-id="b34ff-151">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [externalConnection](../resources/externalconnectors-externalconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b34ff-151">If successful, this method returns a `201 Created` response code and an [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b34ff-152">示例</span><span class="sxs-lookup"><span data-stu-id="b34ff-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b34ff-153">请求</span><span class="sxs-lookup"><span data-stu-id="b34ff-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_externalconnection_from_connections"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/external/connections
Content-Type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```


### <a name="response"></a><span data-ttu-id="b34ff-154">响应</span><span class="sxs-lookup"><span data-stu-id="b34ff-154">Response</span></span>
<span data-ttu-id="b34ff-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b34ff-155">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 200 Created
Content-Type: application/json

{
  "id": "0a4f4e74-4e74-0a4f-744e-4f0a744e4f0a",
  "name": "String",
  "description": "String",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

