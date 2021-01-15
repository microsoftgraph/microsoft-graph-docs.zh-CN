---
title: custodian： activate
description: 在案例内重新激活保管人。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 3058f0fc281a64f937f154dc712c58b568b20c60
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872644"
---
# <a name="custodian-activate"></a><span data-ttu-id="cd50e-103">custodian： activate</span><span class="sxs-lookup"><span data-stu-id="cd50e-103">custodian: activate</span></span>

<span data-ttu-id="cd50e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd50e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd50e-105">激活从案例释放的保管人，使其再次成为案例的一部分。</span><span class="sxs-lookup"><span data-stu-id="cd50e-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="cd50e-106">有关详细信息，请参阅 [管理高级电子数据展示案例中的保管人](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian)。</span><span class="sxs-lookup"><span data-stu-id="cd50e-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd50e-107">权限</span><span class="sxs-lookup"><span data-stu-id="cd50e-107">Permissions</span></span>

<span data-ttu-id="cd50e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd50e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd50e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd50e-110">Permission type</span></span>|<span data-ttu-id="cd50e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd50e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd50e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd50e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd50e-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="cd50e-113">User.Read</span></span>|
|<span data-ttu-id="cd50e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd50e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd50e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd50e-115">Not supported.</span></span>|
|<span data-ttu-id="cd50e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd50e-116">Application</span></span>|<span data-ttu-id="cd50e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd50e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd50e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd50e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="cd50e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd50e-119">Request headers</span></span>

|<span data-ttu-id="cd50e-120">名称</span><span class="sxs-lookup"><span data-stu-id="cd50e-120">Name</span></span>|<span data-ttu-id="cd50e-121">说明</span><span class="sxs-lookup"><span data-stu-id="cd50e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cd50e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd50e-122">Authorization</span></span>|<span data-ttu-id="cd50e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd50e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cd50e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd50e-125">Content-Type</span></span>|<span data-ttu-id="cd50e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cd50e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd50e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd50e-128">Request body</span></span>

<span data-ttu-id="cd50e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd50e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd50e-130">响应</span><span class="sxs-lookup"><span data-stu-id="cd50e-130">Response</span></span>

<span data-ttu-id="cd50e-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd50e-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cd50e-132">示例</span><span class="sxs-lookup"><span data-stu-id="cd50e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd50e-133">请求</span><span class="sxs-lookup"><span data-stu-id="cd50e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd50e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd50e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```
# <a name="c"></a>[<span data-ttu-id="cd50e-135">C#</span><span class="sxs-lookup"><span data-stu-id="cd50e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-activate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd50e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd50e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-activate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd50e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd50e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-activate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd50e-138">Java</span><span class="sxs-lookup"><span data-stu-id="cd50e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-activate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd50e-139">响应</span><span class="sxs-lookup"><span data-stu-id="cd50e-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
