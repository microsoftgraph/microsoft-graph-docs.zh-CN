---
title: 删除 cloudPcOnPremisesConnection
description: 删除 cloudPcOnPremisesConnection 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 55e80278d76b36c7a0b17528878d4673a1626b5c
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563394"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="d33ca-103">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="d33ca-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="d33ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d33ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d33ca-105">删除特定的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d33ca-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="d33ca-106">删除连接时，将从指定的 Azure 资源中删除对该服务的权限。</span><span class="sxs-lookup"><span data-stu-id="d33ca-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="d33ca-107">在通过运行状况检查（由属性指示）后，不能删除本地连接 `healthCheckStatus` 。</span><span class="sxs-lookup"><span data-stu-id="d33ca-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="d33ca-108">您无法删除正在使用的连接，如属性所示 `inUse` 。</span><span class="sxs-lookup"><span data-stu-id="d33ca-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="d33ca-109">权限</span><span class="sxs-lookup"><span data-stu-id="d33ca-109">Permissions</span></span>

<span data-ttu-id="d33ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d33ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d33ca-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d33ca-112">Permission type</span></span>|<span data-ttu-id="d33ca-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d33ca-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d33ca-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d33ca-114">Delegated (work or school account)</span></span>|<span data-ttu-id="d33ca-115">CloudPC</span><span class="sxs-lookup"><span data-stu-id="d33ca-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d33ca-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d33ca-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d33ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d33ca-117">Not supported.</span></span>|
|<span data-ttu-id="d33ca-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d33ca-118">Application</span></span>|<span data-ttu-id="d33ca-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d33ca-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d33ca-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d33ca-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d33ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d33ca-121">Request headers</span></span>

|<span data-ttu-id="d33ca-122">名称</span><span class="sxs-lookup"><span data-stu-id="d33ca-122">Name</span></span>|<span data-ttu-id="d33ca-123">说明</span><span class="sxs-lookup"><span data-stu-id="d33ca-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d33ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d33ca-124">Authorization</span></span>|<span data-ttu-id="d33ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d33ca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d33ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d33ca-127">Request body</span></span>

<span data-ttu-id="d33ca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d33ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d33ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="d33ca-129">Response</span></span>

<span data-ttu-id="d33ca-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d33ca-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d33ca-131">示例</span><span class="sxs-lookup"><span data-stu-id="d33ca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d33ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="d33ca-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d33ca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d33ca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="d33ca-134">C#</span><span class="sxs-lookup"><span data-stu-id="d33ca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesconnections-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d33ca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d33ca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesconnections-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d33ca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d33ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesconnections-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d33ca-137">Java</span><span class="sxs-lookup"><span data-stu-id="d33ca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesconnections-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d33ca-138">响应</span><span class="sxs-lookup"><span data-stu-id="d33ca-138">Response</span></span>

<span data-ttu-id="d33ca-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d33ca-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
