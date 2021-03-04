---
title: custodian： release
description: 从案例释放保管人。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: baf0eb188e0419ca5b7a34e8274515b47d3daafd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446051"
---
# <a name="custodian-release"></a><span data-ttu-id="24ed1-103">custodian： release</span><span class="sxs-lookup"><span data-stu-id="24ed1-103">custodian: release</span></span>

<span data-ttu-id="24ed1-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="24ed1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24ed1-105">从案例释放保管人。</span><span class="sxs-lookup"><span data-stu-id="24ed1-105">Release a custodian from a case.</span></span> <span data-ttu-id="24ed1-106">有关详细信息，请参阅["从案例释放保管人"。](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case)</span><span class="sxs-lookup"><span data-stu-id="24ed1-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="24ed1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="24ed1-107">Permissions</span></span>

<span data-ttu-id="24ed1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24ed1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24ed1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="24ed1-110">Permission type</span></span>|<span data-ttu-id="24ed1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24ed1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24ed1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24ed1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24ed1-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ed1-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="24ed1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24ed1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24ed1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24ed1-115">Not supported.</span></span>|
|<span data-ttu-id="24ed1-116">Application</span><span class="sxs-lookup"><span data-stu-id="24ed1-116">Application</span></span>|<span data-ttu-id="24ed1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="24ed1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24ed1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24ed1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="24ed1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="24ed1-119">Request headers</span></span>

|<span data-ttu-id="24ed1-120">名称</span><span class="sxs-lookup"><span data-stu-id="24ed1-120">Name</span></span>|<span data-ttu-id="24ed1-121">说明</span><span class="sxs-lookup"><span data-stu-id="24ed1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24ed1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24ed1-122">Authorization</span></span>|<span data-ttu-id="24ed1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24ed1-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="24ed1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24ed1-125">Content-Type</span></span>|<span data-ttu-id="24ed1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="24ed1-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24ed1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="24ed1-128">Request body</span></span>

<span data-ttu-id="24ed1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24ed1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24ed1-130">响应</span><span class="sxs-lookup"><span data-stu-id="24ed1-130">Response</span></span>

<span data-ttu-id="24ed1-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="24ed1-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="24ed1-132">示例</span><span class="sxs-lookup"><span data-stu-id="24ed1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24ed1-133">请求</span><span class="sxs-lookup"><span data-stu-id="24ed1-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="24ed1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="24ed1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```
# <a name="c"></a>[<span data-ttu-id="24ed1-135">C#</span><span class="sxs-lookup"><span data-stu-id="24ed1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24ed1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24ed1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24ed1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24ed1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24ed1-138">Java</span><span class="sxs-lookup"><span data-stu-id="24ed1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24ed1-139">响应</span><span class="sxs-lookup"><span data-stu-id="24ed1-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
