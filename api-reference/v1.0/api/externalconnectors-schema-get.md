---
title: 获取架构
description: 读取架构对象的属性和关系。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f76eb8f174958d8698528e49fffda105c54cc7f4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467282"
---
# <a name="get-schema"></a><span data-ttu-id="6b6c3-103">获取架构</span><span class="sxs-lookup"><span data-stu-id="6b6c3-103">Get schema</span></span>
<span data-ttu-id="6b6c3-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="6b6c3-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="6b6c3-105">读取架构 [对象的属性和](../resources/externalconnectors-schema.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-105">Read the properties and relationships of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b6c3-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b6c3-106">Permissions</span></span>
<span data-ttu-id="6b6c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b6c3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b6c3-109">Permission type</span></span>|<span data-ttu-id="6b6c3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b6c3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b6c3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b6c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b6c3-112">不适用</span><span class="sxs-lookup"><span data-stu-id="6b6c3-112">Not applicable</span></span>|
|<span data-ttu-id="6b6c3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b6c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b6c3-114">不适用</span><span class="sxs-lookup"><span data-stu-id="6b6c3-114">Not applicable</span></span>|
|<span data-ttu-id="6b6c3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b6c3-115">Application</span></span>| <span data-ttu-id="6b6c3-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="6b6c3-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b6c3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b6c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b6c3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6b6c3-118">Optional query parameters</span></span>
<span data-ttu-id="6b6c3-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6b6c3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b6c3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b6c3-121">Request headers</span></span>
|<span data-ttu-id="6b6c3-122">名称</span><span class="sxs-lookup"><span data-stu-id="6b6c3-122">Name</span></span>|<span data-ttu-id="6b6c3-123">说明</span><span class="sxs-lookup"><span data-stu-id="6b6c3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6b6c3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b6c3-124">Authorization</span></span>|<span data-ttu-id="6b6c3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b6c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b6c3-127">Request body</span></span>
<span data-ttu-id="6b6c3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b6c3-129">响应</span><span class="sxs-lookup"><span data-stu-id="6b6c3-129">Response</span></span>

<span data-ttu-id="6b6c3-130">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/externalconnectors-schema.md) 代码和 schema 对象。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-130">If successful, this method returns a `200 OK` response code and a [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b6c3-131">示例</span><span class="sxs-lookup"><span data-stu-id="6b6c3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b6c3-132">请求</span><span class="sxs-lookup"><span data-stu-id="6b6c3-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schema"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr/schema
```


### <a name="response"></a><span data-ttu-id="6b6c3-133">响应</span><span class="sxs-lookup"><span data-stu-id="6b6c3-133">Response</span></span>
<span data-ttu-id="6b6c3-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b6c3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "baseType": "String",
    "properties": [
      {
        "name": "ticketTitle",
        "type": "string",
        "isSearchable": true,
        "isRetrievable": true,
        "labels": [
          "title"
        ]
      },
      {
        "name": "priority",
        "type": "string",
        "isQueryable": true,
        "isRetrievable": true,
        "isRefinable": true,
        "isSearchable": false
      },
      {
        "name": "assignee",
        "type": "string",
        "isRetrievable": true
      }
    ]
  }
}
```

