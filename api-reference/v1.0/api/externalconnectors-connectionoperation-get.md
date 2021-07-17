---
title: 获取 connectionOperation
description: 读取 connectionOperation 对象的属性和关系。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7a5e5849e91b0d7816ba6b293838eb434e05c900
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467296"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="0c4c5-103">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="0c4c5-103">Get connectionOperation</span></span>

<span data-ttu-id="0c4c5-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="0c4c5-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="0c4c5-105">读取 [connectionOperation](../resources/externalconnectors-connectionoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-105">Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c4c5-106">Permissions</span></span>
<span data-ttu-id="0c4c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c4c5-109">Permission type</span></span>|<span data-ttu-id="0c4c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c4c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c4c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c4c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c4c5-112">不适用</span><span class="sxs-lookup"><span data-stu-id="0c4c5-112">Not applicable</span></span>|
|<span data-ttu-id="0c4c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c4c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c4c5-114">不适用</span><span class="sxs-lookup"><span data-stu-id="0c4c5-114">Not applicable</span></span>|
|<span data-ttu-id="0c4c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c4c5-115">Application</span></span>| <span data-ttu-id="0c4c5-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0c4c5-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c4c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/operations/{connectionOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c4c5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c4c5-118">Optional query parameters</span></span>
<span data-ttu-id="0c4c5-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0c4c5-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c4c5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c4c5-121">Request headers</span></span>
|<span data-ttu-id="0c4c5-122">名称</span><span class="sxs-lookup"><span data-stu-id="0c4c5-122">Name</span></span>|<span data-ttu-id="0c4c5-123">说明</span><span class="sxs-lookup"><span data-stu-id="0c4c5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c4c5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c4c5-124">Authorization</span></span>|<span data-ttu-id="0c4c5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4c5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c4c5-127">Request body</span></span>
<span data-ttu-id="0c4c5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4c5-129">响应</span><span class="sxs-lookup"><span data-stu-id="0c4c5-129">Response</span></span>

<span data-ttu-id="0c4c5-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [connectionOperation](../resources/externalconnectors-connectionoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-130">If successful, this method returns a `200 OK` response code and a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c4c5-131">示例</span><span class="sxs-lookup"><span data-stu-id="0c4c5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c4c5-132">请求</span><span class="sxs-lookup"><span data-stu-id="0c4c5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```


### <a name="response"></a><span data-ttu-id="0c4c5-133">响应</span><span class="sxs-lookup"><span data-stu-id="0c4c5-133">Response</span></span>
<span data-ttu-id="0c4c5-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0c4c5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

