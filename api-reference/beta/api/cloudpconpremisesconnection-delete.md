---
title: 删除 cloudPcOnPremisesConnection
description: 删除 cloudPcOnPremisesConnection 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 01f9b5a7e4091492be7aa8eae0f0d3f8354169e6
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872763"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="0be76-103">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="0be76-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="0be76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0be76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0be76-105">删除特定的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0be76-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="0be76-106">删除连接时，将从指定的 Azure 资源中删除对服务的权限。</span><span class="sxs-lookup"><span data-stu-id="0be76-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="0be76-107">一旦内部部署连接通过运行状况检查（由属性指示）后，将无法 `healthCheckStatus` 删除该连接。</span><span class="sxs-lookup"><span data-stu-id="0be76-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="0be76-108">如果连接在使用中，则不能删除该连接，如属性 `inUse` 所指示。</span><span class="sxs-lookup"><span data-stu-id="0be76-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="0be76-109">权限</span><span class="sxs-lookup"><span data-stu-id="0be76-109">Permissions</span></span>

<span data-ttu-id="0be76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0be76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be76-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0be76-112">Permission type</span></span>|<span data-ttu-id="0be76-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0be76-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0be76-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0be76-114">Delegated (work or school account)</span></span>|<span data-ttu-id="0be76-115">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be76-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="0be76-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0be76-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0be76-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0be76-117">Not supported.</span></span>|
|<span data-ttu-id="0be76-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0be76-118">Application</span></span>|<span data-ttu-id="0be76-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0be76-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0be76-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0be76-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0be76-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0be76-121">Request headers</span></span>

|<span data-ttu-id="0be76-122">名称</span><span class="sxs-lookup"><span data-stu-id="0be76-122">Name</span></span>|<span data-ttu-id="0be76-123">说明</span><span class="sxs-lookup"><span data-stu-id="0be76-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0be76-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0be76-124">Authorization</span></span>|<span data-ttu-id="0be76-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0be76-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be76-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0be76-127">Request body</span></span>

<span data-ttu-id="0be76-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0be76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0be76-129">响应</span><span class="sxs-lookup"><span data-stu-id="0be76-129">Response</span></span>

<span data-ttu-id="0be76-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0be76-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0be76-131">示例</span><span class="sxs-lookup"><span data-stu-id="0be76-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0be76-132">请求</span><span class="sxs-lookup"><span data-stu-id="0be76-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0be76-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0be76-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="0be76-134">C#</span><span class="sxs-lookup"><span data-stu-id="0be76-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesconnections-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0be76-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0be76-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesconnections-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0be76-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0be76-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesconnections-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0be76-137">Java</span><span class="sxs-lookup"><span data-stu-id="0be76-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesconnections-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0be76-138">响应</span><span class="sxs-lookup"><span data-stu-id="0be76-138">Response</span></span>

<span data-ttu-id="0be76-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0be76-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
