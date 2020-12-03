---
title: 列出 cloudPcProvisioningPolicy
description: 查看所有云电脑设置策略的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 618d7f742d68bfb0b729152ef8acfd876cf1a809
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563884"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="ee402-103">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="ee402-103">List provisioningPolicies</span></span>

<span data-ttu-id="ee402-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee402-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee402-105">列出 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ee402-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ee402-106">权限</span><span class="sxs-lookup"><span data-stu-id="ee402-106">Permissions</span></span>

<span data-ttu-id="ee402-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee402-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee402-109">Permission type</span></span>|<span data-ttu-id="ee402-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ee402-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee402-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee402-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee402-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="ee402-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="ee402-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee402-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee402-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee402-114">Not supported.</span></span>|
|<span data-ttu-id="ee402-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee402-115">Application</span></span>|<span data-ttu-id="ee402-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee402-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee402-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee402-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee402-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ee402-118">Optional query parameters</span></span>

<span data-ttu-id="ee402-119">此方法支持 `$select` `$filter` 和 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ee402-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee402-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ee402-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee402-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee402-121">Request headers</span></span>

| <span data-ttu-id="ee402-122">名称</span><span class="sxs-lookup"><span data-stu-id="ee402-122">Name</span></span>          | <span data-ttu-id="ee402-123">说明</span><span class="sxs-lookup"><span data-stu-id="ee402-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ee402-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee402-124">Authorization</span></span> | <span data-ttu-id="ee402-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee402-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee402-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee402-127">Request body</span></span>

<span data-ttu-id="ee402-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee402-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee402-129">响应</span><span class="sxs-lookup"><span data-stu-id="ee402-129">Response</span></span>

<span data-ttu-id="ee402-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ee402-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee402-131">示例</span><span class="sxs-lookup"><span data-stu-id="ee402-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee402-132">请求</span><span class="sxs-lookup"><span data-stu-id="ee402-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ee402-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee402-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```
# <a name="c"></a>[<span data-ttu-id="ee402-134">C#</span><span class="sxs-lookup"><span data-stu-id="ee402-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcprovisioningpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee402-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee402-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcprovisioningpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee402-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee402-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcprovisioningpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee402-137">Java</span><span class="sxs-lookup"><span data-stu-id="ee402-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcprovisioningpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee402-138">响应</span><span class="sxs-lookup"><span data-stu-id="ee402-138">Response</span></span>

<span data-ttu-id="ee402-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee402-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
