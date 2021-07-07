---
title: cloudPcAuditEvent：getAuditActivityTypes
description: 按租户 ID 获取审核活动类型。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7ea6612160474c2fbbfde792f3565f1100dac146
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316967"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a><span data-ttu-id="030d0-103">cloudPcAuditEvent：getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="030d0-103">cloudPcAuditEvent: getAuditActivityTypes</span></span>

<span data-ttu-id="030d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="030d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="030d0-105">按租户 ID 获取审核活动类型。</span><span class="sxs-lookup"><span data-stu-id="030d0-105">Get audit activity types by tenant ID.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="030d0-106">权限</span><span class="sxs-lookup"><span data-stu-id="030d0-106">Permissions</span></span>

<span data-ttu-id="030d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="030d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="030d0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="030d0-109">Permission type</span></span>| <span data-ttu-id="030d0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="030d0-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="030d0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="030d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="030d0-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="030d0-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="030d0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="030d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="030d0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="030d0-114">Not supported.</span></span>|
|<span data-ttu-id="030d0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="030d0-115">Application</span></span>|<span data-ttu-id="030d0-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="030d0-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="030d0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="030d0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="030d0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="030d0-118">Request headers</span></span>

| <span data-ttu-id="030d0-119">名称</span><span class="sxs-lookup"><span data-stu-id="030d0-119">Name</span></span>          | <span data-ttu-id="030d0-120">说明</span><span class="sxs-lookup"><span data-stu-id="030d0-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="030d0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="030d0-121">Authorization</span></span> | <span data-ttu-id="030d0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="030d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="030d0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="030d0-124">Request body</span></span>

<span data-ttu-id="030d0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="030d0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="030d0-126">响应</span><span class="sxs-lookup"><span data-stu-id="030d0-126">Response</span></span>

<span data-ttu-id="030d0-127">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="030d0-127">If successful, this method returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="030d0-128">示例</span><span class="sxs-lookup"><span data-stu-id="030d0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="030d0-129">请求</span><span class="sxs-lookup"><span data-stu-id="030d0-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="030d0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="030d0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```
# <a name="c"></a>[<span data-ttu-id="030d0-131">C#</span><span class="sxs-lookup"><span data-stu-id="030d0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcauditevent-getauditactivitytypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="030d0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="030d0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcauditevent-getauditactivitytypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="030d0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="030d0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcauditevent-getauditactivitytypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="030d0-134">Java</span><span class="sxs-lookup"><span data-stu-id="030d0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcauditevent-getauditactivitytypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="030d0-135">响应</span><span class="sxs-lookup"><span data-stu-id="030d0-135">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```
