---
title: cloudPcAuditEvent：getAuditActivityTypes
description: 按租户 ID 获取审核活动类型。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a6e5fd01d0b2100affa6b5d89c43a50cddbaa533
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211221"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a><span data-ttu-id="5db30-103">cloudPcAuditEvent：getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="5db30-103">cloudPcAuditEvent: getAuditActivityTypes</span></span>

<span data-ttu-id="5db30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5db30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db30-105">按租户 ID 获取审核活动类型。</span><span class="sxs-lookup"><span data-stu-id="5db30-105">Get audit activity types by tenant ID.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="5db30-106">权限</span><span class="sxs-lookup"><span data-stu-id="5db30-106">Permissions</span></span>

<span data-ttu-id="5db30-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5db30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5db30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5db30-109">Permission type</span></span>| <span data-ttu-id="5db30-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5db30-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="5db30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5db30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5db30-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db30-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="5db30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5db30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5db30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5db30-114">Not supported.</span></span>|
|<span data-ttu-id="5db30-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5db30-115">Application</span></span>|<span data-ttu-id="5db30-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db30-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5db30-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5db30-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="5db30-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5db30-118">Request headers</span></span>

| <span data-ttu-id="5db30-119">名称</span><span class="sxs-lookup"><span data-stu-id="5db30-119">Name</span></span>          | <span data-ttu-id="5db30-120">说明</span><span class="sxs-lookup"><span data-stu-id="5db30-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5db30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5db30-121">Authorization</span></span> | <span data-ttu-id="5db30-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5db30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5db30-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5db30-124">Request body</span></span>

<span data-ttu-id="5db30-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5db30-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5db30-126">响应</span><span class="sxs-lookup"><span data-stu-id="5db30-126">Response</span></span>

<span data-ttu-id="5db30-127">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="5db30-127">If successful, this method returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5db30-128">示例</span><span class="sxs-lookup"><span data-stu-id="5db30-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5db30-129">请求</span><span class="sxs-lookup"><span data-stu-id="5db30-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

### <a name="response"></a><span data-ttu-id="5db30-130">响应</span><span class="sxs-lookup"><span data-stu-id="5db30-130">Response</span></span>


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
