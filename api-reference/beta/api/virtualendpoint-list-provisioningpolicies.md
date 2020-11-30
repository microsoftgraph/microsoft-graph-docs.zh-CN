---
title: 列出 cloudPcProvisioningPolicy
description: 查看所有云电脑设置策略的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b9d62152228518aa856b48e3fc064ce77fd1801f
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378311"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="82f99-103">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="82f99-103">List provisioningPolicies</span></span>

<span data-ttu-id="82f99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82f99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82f99-105">列出 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82f99-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="82f99-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="82f99-106">Permissions</span></span>

<span data-ttu-id="82f99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f99-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82f99-109">Permission type</span></span>|<span data-ttu-id="82f99-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82f99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f99-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82f99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82f99-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="82f99-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="82f99-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82f99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f99-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="82f99-114">Not supported.</span></span>|
|<span data-ttu-id="82f99-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82f99-115">Application</span></span>|<span data-ttu-id="82f99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="82f99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f99-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82f99-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82f99-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="82f99-118">Optional query parameters</span></span>

<span data-ttu-id="82f99-119">此方法支持 `$select` `$filter` 和 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82f99-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="82f99-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="82f99-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82f99-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="82f99-121">Request headers</span></span>

| <span data-ttu-id="82f99-122">名称</span><span class="sxs-lookup"><span data-stu-id="82f99-122">Name</span></span>          | <span data-ttu-id="82f99-123">说明</span><span class="sxs-lookup"><span data-stu-id="82f99-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="82f99-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="82f99-124">Authorization</span></span> | <span data-ttu-id="82f99-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82f99-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82f99-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="82f99-127">Request body</span></span>

<span data-ttu-id="82f99-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82f99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82f99-129">响应</span><span class="sxs-lookup"><span data-stu-id="82f99-129">Response</span></span>

<span data-ttu-id="82f99-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82f99-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82f99-131">示例</span><span class="sxs-lookup"><span data-stu-id="82f99-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82f99-132">请求</span><span class="sxs-lookup"><span data-stu-id="82f99-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```

### <a name="response"></a><span data-ttu-id="82f99-133">响应</span><span class="sxs-lookup"><span data-stu-id="82f99-133">Response</span></span>

<span data-ttu-id="82f99-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82f99-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcProvisioningPolicy)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
      "id": "1d164206-bf41-4fd2-8424-a3192d392273",
      "displayName": "Display Name value",
      "description": "Description value",
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "imageId": "Image ID value",
      "imageDisplayName": "Image Display Name value",
      "imageType":"custom"
    }
  ]
}
```
