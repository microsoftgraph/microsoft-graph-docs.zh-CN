---
title: 获取 continuousAccessEvaluationPolicy
description: 读取 continuousAccessEvaluationPolicy 对象的属性。
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bea54ea801ee9d41314f1fbd2c87070ac4e92773
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023433"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="bf291-103">获取 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="bf291-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="bf291-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf291-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf291-105">读取 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf291-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf291-106">权限</span><span class="sxs-lookup"><span data-stu-id="bf291-106">Permissions</span></span>
<span data-ttu-id="bf291-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf291-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf291-109">Permission type</span></span>|<span data-ttu-id="bf291-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf291-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf291-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf291-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf291-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf291-112">Policy.Read.All</span></span> |
|<span data-ttu-id="bf291-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf291-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf291-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf291-114">Not supported.</span></span> |
|<span data-ttu-id="bf291-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf291-115">Application</span></span>                            | <span data-ttu-id="bf291-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf291-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf291-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf291-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf291-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bf291-118">Optional query parameters</span></span>
<span data-ttu-id="bf291-119">此方法支持 "$select" OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bf291-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="bf291-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bf291-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf291-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf291-121">Request headers</span></span>
|<span data-ttu-id="bf291-122">名称</span><span class="sxs-lookup"><span data-stu-id="bf291-122">Name</span></span>|<span data-ttu-id="bf291-123">说明</span><span class="sxs-lookup"><span data-stu-id="bf291-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf291-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf291-124">Authorization</span></span>|<span data-ttu-id="bf291-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf291-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf291-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf291-127">Request body</span></span>
<span data-ttu-id="bf291-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf291-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf291-129">响应</span><span class="sxs-lookup"><span data-stu-id="bf291-129">Response</span></span>

<span data-ttu-id="bf291-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf291-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf291-131">示例</span><span class="sxs-lookup"><span data-stu-id="bf291-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf291-132">请求</span><span class="sxs-lookup"><span data-stu-id="bf291-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```


### <a name="response"></a><span data-ttu-id="bf291-133">响应</span><span class="sxs-lookup"><span data-stu-id="bf291-133">Response</span></span>

<span data-ttu-id="bf291-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf291-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
