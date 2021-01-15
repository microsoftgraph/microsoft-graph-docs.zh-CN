---
title: custodian： release
description: 从案例释放保管人。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 3b3fc0633672785e6a1f8aacc350fd9a8d34d4d7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872497"
---
# <a name="custodian-release"></a><span data-ttu-id="fa981-103">custodian： release</span><span class="sxs-lookup"><span data-stu-id="fa981-103">custodian: release</span></span>

<span data-ttu-id="fa981-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa981-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa981-105">从案例释放保管人。</span><span class="sxs-lookup"><span data-stu-id="fa981-105">Release a custodian from a case.</span></span> <span data-ttu-id="fa981-106">有关详细信息，请参阅["从案例释放保管人"。](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case)</span><span class="sxs-lookup"><span data-stu-id="fa981-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa981-107">权限</span><span class="sxs-lookup"><span data-stu-id="fa981-107">Permissions</span></span>

<span data-ttu-id="fa981-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa981-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa981-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa981-110">Permission type</span></span>|<span data-ttu-id="fa981-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa981-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa981-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa981-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa981-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="fa981-113">User.Read</span></span>|
|<span data-ttu-id="fa981-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa981-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa981-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa981-115">Not supported.</span></span>|
|<span data-ttu-id="fa981-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa981-116">Application</span></span>|<span data-ttu-id="fa981-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa981-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa981-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa981-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="fa981-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa981-119">Request headers</span></span>

|<span data-ttu-id="fa981-120">名称</span><span class="sxs-lookup"><span data-stu-id="fa981-120">Name</span></span>|<span data-ttu-id="fa981-121">说明</span><span class="sxs-lookup"><span data-stu-id="fa981-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa981-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa981-122">Authorization</span></span>|<span data-ttu-id="fa981-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa981-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fa981-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa981-125">Content-Type</span></span>|<span data-ttu-id="fa981-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fa981-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa981-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa981-128">Request body</span></span>

<span data-ttu-id="fa981-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa981-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa981-130">响应</span><span class="sxs-lookup"><span data-stu-id="fa981-130">Response</span></span>

<span data-ttu-id="fa981-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fa981-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fa981-132">示例</span><span class="sxs-lookup"><span data-stu-id="fa981-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa981-133">请求</span><span class="sxs-lookup"><span data-stu-id="fa981-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fa981-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa981-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```
# <a name="c"></a>[<span data-ttu-id="fa981-135">C#</span><span class="sxs-lookup"><span data-stu-id="fa981-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa981-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa981-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa981-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa981-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa981-138">Java</span><span class="sxs-lookup"><span data-stu-id="fa981-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa981-139">响应</span><span class="sxs-lookup"><span data-stu-id="fa981-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
