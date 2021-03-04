---
title: custodian： activate
description: 在案例内重新激活保管人。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 82f79abee2fe7cc64ce7f4efb4f7c950a29b7b88
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446064"
---
# <a name="custodian-activate"></a><span data-ttu-id="6e562-103">custodian： activate</span><span class="sxs-lookup"><span data-stu-id="6e562-103">custodian: activate</span></span>

<span data-ttu-id="6e562-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6e562-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e562-105">激活从案例释放的保管人，使其再次成为案例的一部分。</span><span class="sxs-lookup"><span data-stu-id="6e562-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="6e562-106">有关详细信息，请参阅 ["管理高级电子数据展示"案例中的保管人](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian)。</span><span class="sxs-lookup"><span data-stu-id="6e562-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e562-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e562-107">Permissions</span></span>

<span data-ttu-id="6e562-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e562-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e562-110">Permission type</span></span>|<span data-ttu-id="6e562-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e562-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e562-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e562-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e562-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e562-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6e562-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e562-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e562-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e562-115">Not supported.</span></span>|
|<span data-ttu-id="6e562-116">Application</span><span class="sxs-lookup"><span data-stu-id="6e562-116">Application</span></span>|<span data-ttu-id="6e562-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e562-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e562-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e562-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="6e562-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e562-119">Request headers</span></span>

|<span data-ttu-id="6e562-120">名称</span><span class="sxs-lookup"><span data-stu-id="6e562-120">Name</span></span>|<span data-ttu-id="6e562-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e562-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e562-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e562-122">Authorization</span></span>|<span data-ttu-id="6e562-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e562-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6e562-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e562-125">Content-Type</span></span>|<span data-ttu-id="6e562-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6e562-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e562-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e562-128">Request body</span></span>

<span data-ttu-id="6e562-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e562-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e562-130">响应</span><span class="sxs-lookup"><span data-stu-id="6e562-130">Response</span></span>

<span data-ttu-id="6e562-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6e562-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6e562-132">示例</span><span class="sxs-lookup"><span data-stu-id="6e562-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e562-133">请求</span><span class="sxs-lookup"><span data-stu-id="6e562-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6e562-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e562-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```
# <a name="c"></a>[<span data-ttu-id="6e562-135">C#</span><span class="sxs-lookup"><span data-stu-id="6e562-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-activate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e562-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e562-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-activate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e562-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e562-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-activate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e562-138">Java</span><span class="sxs-lookup"><span data-stu-id="6e562-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-activate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e562-139">响应</span><span class="sxs-lookup"><span data-stu-id="6e562-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
