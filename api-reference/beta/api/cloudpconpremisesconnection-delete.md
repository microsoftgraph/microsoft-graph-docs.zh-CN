---
title: 删除 cloudPcOnPremisesConnection
description: 删除 cloudPcOnPremisesConnection 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 73c3f899a3c7fbc862ddb68a243dbddd33205ba4
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378275"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="d82c6-103">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="d82c6-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="d82c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d82c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d82c6-105">删除特定的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d82c6-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="d82c6-106">删除连接时，将从指定的 Azure 资源中删除对该服务的权限。</span><span class="sxs-lookup"><span data-stu-id="d82c6-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="d82c6-107">在通过运行状况检查（由属性指示）后，不能删除本地连接 `healthCheckStatus` 。</span><span class="sxs-lookup"><span data-stu-id="d82c6-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="d82c6-108">您无法删除正在使用的连接，如属性所示 `inUse` 。</span><span class="sxs-lookup"><span data-stu-id="d82c6-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

## <a name="permissions"></a><span data-ttu-id="d82c6-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="d82c6-109">Permissions</span></span>

<span data-ttu-id="d82c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d82c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d82c6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d82c6-112">Permission type</span></span>|<span data-ttu-id="d82c6-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d82c6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d82c6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d82c6-114">Delegated (work or school account)</span></span>|<span data-ttu-id="d82c6-115">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d82c6-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d82c6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d82c6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d82c6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d82c6-117">Not supported.</span></span>|
|<span data-ttu-id="d82c6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d82c6-118">Application</span></span>|<span data-ttu-id="d82c6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d82c6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d82c6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d82c6-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d82c6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d82c6-121">Request headers</span></span>

|<span data-ttu-id="d82c6-122">名称</span><span class="sxs-lookup"><span data-stu-id="d82c6-122">Name</span></span>|<span data-ttu-id="d82c6-123">说明</span><span class="sxs-lookup"><span data-stu-id="d82c6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d82c6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d82c6-124">Authorization</span></span>|<span data-ttu-id="d82c6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d82c6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d82c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d82c6-127">Request body</span></span>

<span data-ttu-id="d82c6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d82c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d82c6-129">响应</span><span class="sxs-lookup"><span data-stu-id="d82c6-129">Response</span></span>

<span data-ttu-id="d82c6-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d82c6-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d82c6-131">示例</span><span class="sxs-lookup"><span data-stu-id="d82c6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d82c6-132">请求</span><span class="sxs-lookup"><span data-stu-id="d82c6-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

### <a name="response"></a><span data-ttu-id="d82c6-133">响应</span><span class="sxs-lookup"><span data-stu-id="d82c6-133">Response</span></span>

<span data-ttu-id="d82c6-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d82c6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
