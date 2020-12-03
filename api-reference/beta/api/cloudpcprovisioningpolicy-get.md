---
title: 获取 cloudPcProvisioningPolicy
description: 读取 cloudPcProvisioningPolicy 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3f1ea40d146381e2f810a67776ef41e8539ea115
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563378"
---
# <a name="get-cloudpcprovisioningpolicy"></a><span data-ttu-id="f03da-103">获取 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="f03da-103">Get cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="f03da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f03da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f03da-105">读取 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f03da-105">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f03da-106">权限</span><span class="sxs-lookup"><span data-stu-id="f03da-106">Permissions</span></span>

<span data-ttu-id="f03da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f03da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f03da-109">Permission type</span></span>|<span data-ttu-id="f03da-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f03da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f03da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f03da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f03da-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="f03da-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="f03da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f03da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f03da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03da-114">Not supported.</span></span>|
|<span data-ttu-id="f03da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f03da-115">Application</span></span>|<span data-ttu-id="f03da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f03da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f03da-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f03da-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f03da-118">Optional query parameters</span></span>

<span data-ttu-id="f03da-119">此方法支持 `$select` 和 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f03da-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f03da-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f03da-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f03da-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f03da-121">Request headers</span></span>

| <span data-ttu-id="f03da-122">名称</span><span class="sxs-lookup"><span data-stu-id="f03da-122">Name</span></span>          | <span data-ttu-id="f03da-123">说明</span><span class="sxs-lookup"><span data-stu-id="f03da-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f03da-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03da-124">Authorization</span></span> | <span data-ttu-id="f03da-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f03da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f03da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f03da-127">Request body</span></span>

<span data-ttu-id="f03da-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f03da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f03da-129">响应</span><span class="sxs-lookup"><span data-stu-id="f03da-129">Response</span></span>

<span data-ttu-id="f03da-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f03da-130">If successful, this method returns a `200 OK` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f03da-131">示例</span><span class="sxs-lookup"><span data-stu-id="f03da-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-provisioning-policy"></a><span data-ttu-id="f03da-132">示例1：获取指定设置策略的属性</span><span class="sxs-lookup"><span data-stu-id="f03da-132">Example 1: Get the properties of the specified provisioning policy</span></span>

#### <a name="request"></a><span data-ttu-id="f03da-133">请求</span><span class="sxs-lookup"><span data-stu-id="f03da-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f03da-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f03da-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="f03da-135">C#</span><span class="sxs-lookup"><span data-stu-id="f03da-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f03da-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f03da-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f03da-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f03da-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f03da-138">Java</span><span class="sxs-lookup"><span data-stu-id="f03da-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f03da-139">响应</span><span class="sxs-lookup"><span data-stu-id="f03da-139">Response</span></span>

<span data-ttu-id="f03da-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f03da-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "description": "Description value",
    "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
    "imageId": "Image ID value",
    "imageDisplayName": "Image Display Name value",
    "imageType": "custom"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-provisioning-policy-and-expand-on-the-assignments"></a><span data-ttu-id="f03da-141">示例2：获取指定的设置策略的属性，并在工作分配上展开</span><span class="sxs-lookup"><span data-stu-id="f03da-141">Example 2: Get the properties of the specified provisioning policy and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="f03da-142">请求</span><span class="sxs-lookup"><span data-stu-id="f03da-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f03da-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f03da-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}?$expand=assignments
```
# <a name="c"></a>[<span data-ttu-id="f03da-144">C#</span><span class="sxs-lookup"><span data-stu-id="f03da-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f03da-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f03da-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f03da-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f03da-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f03da-147">Java</span><span class="sxs-lookup"><span data-stu-id="f03da-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f03da-148">响应</span><span class="sxs-lookup"><span data-stu-id="f03da-148">Response</span></span>

<span data-ttu-id="f03da-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f03da-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "description": "Description value",
    "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
    "imageId": "Image ID value",
    "imageDisplayName": "Image Display Name value",
    "imageType": "custom",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
