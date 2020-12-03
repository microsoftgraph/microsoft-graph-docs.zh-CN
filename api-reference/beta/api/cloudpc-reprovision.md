---
title: cloudPC：重新设置
description: 重新设置特定云电脑。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6fe8b4a4a588c3ce469f300b397c767f33eed221
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563350"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="4ab4f-103">cloudPC：重新设置</span><span class="sxs-lookup"><span data-stu-id="4ab4f-103">cloudPC: reprovision</span></span>

<span data-ttu-id="4ab4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ab4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ab4f-105">重新设置特定云电脑。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-105">Reprovision a specific cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="4ab4f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ab4f-106">Permissions</span></span>

<span data-ttu-id="4ab4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab4f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ab4f-109">Permission type</span></span>|<span data-ttu-id="4ab4f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ab4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ab4f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ab4f-112">CloudPC</span><span class="sxs-lookup"><span data-stu-id="4ab4f-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="4ab4f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ab4f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-114">Not supported.</span></span>|
|<span data-ttu-id="4ab4f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ab4f-115">Application</span></span>|<span data-ttu-id="4ab4f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ab4f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ab4f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="4ab4f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ab4f-118">Request headers</span></span>

|<span data-ttu-id="4ab4f-119">名称</span><span class="sxs-lookup"><span data-stu-id="4ab4f-119">Name</span></span>|<span data-ttu-id="4ab4f-120">说明</span><span class="sxs-lookup"><span data-stu-id="4ab4f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ab4f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab4f-121">Authorization</span></span>|<span data-ttu-id="4ab4f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ab4f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ab4f-124">Request body</span></span>

<span data-ttu-id="4ab4f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab4f-126">响应</span><span class="sxs-lookup"><span data-stu-id="4ab4f-126">Response</span></span>

<span data-ttu-id="4ab4f-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4ab4f-128">示例</span><span class="sxs-lookup"><span data-stu-id="4ab4f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ab4f-129">请求</span><span class="sxs-lookup"><span data-stu-id="4ab4f-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4ab4f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ab4f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```
# <a name="c"></a>[<span data-ttu-id="4ab4f-131">C#</span><span class="sxs-lookup"><span data-stu-id="4ab4f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ab4f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ab4f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ab4f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ab4f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ab4f-134">Java</span><span class="sxs-lookup"><span data-stu-id="4ab4f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ab4f-135">响应</span><span class="sxs-lookup"><span data-stu-id="4ab4f-135">Response</span></span>

<span data-ttu-id="4ab4f-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ab4f-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
