---
title: 获取 cloudPcProvisioningPolicy
description: 读取 cloudPcProvisioningPolicy 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fa46603bddde0e12e34ad1abccf5afaa74861971
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378297"
---
# <a name="get-cloudpcprovisioningpolicy"></a><span data-ttu-id="0cf33-103">获取 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="0cf33-103">Get cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="0cf33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf33-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cf33-105">读取 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0cf33-105">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cf33-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0cf33-106">Permissions</span></span>

<span data-ttu-id="0cf33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cf33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf33-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cf33-109">Permission type</span></span>|<span data-ttu-id="0cf33-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0cf33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cf33-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cf33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0cf33-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="0cf33-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="0cf33-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cf33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cf33-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cf33-114">Not supported.</span></span>|
|<span data-ttu-id="0cf33-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cf33-115">Application</span></span>|<span data-ttu-id="0cf33-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cf33-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cf33-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cf33-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cf33-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="0cf33-118">Optional query parameters</span></span>

<span data-ttu-id="0cf33-119">此方法支持 `$select` 和 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0cf33-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0cf33-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0cf33-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cf33-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cf33-121">Request headers</span></span>

| <span data-ttu-id="0cf33-122">名称</span><span class="sxs-lookup"><span data-stu-id="0cf33-122">Name</span></span>          | <span data-ttu-id="0cf33-123">说明</span><span class="sxs-lookup"><span data-stu-id="0cf33-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0cf33-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cf33-124">Authorization</span></span> | <span data-ttu-id="0cf33-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0cf33-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cf33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cf33-127">Request body</span></span>

<span data-ttu-id="0cf33-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0cf33-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cf33-129">响应</span><span class="sxs-lookup"><span data-stu-id="0cf33-129">Response</span></span>

<span data-ttu-id="0cf33-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0cf33-130">If successful, this method returns a `200 OK` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cf33-131">示例</span><span class="sxs-lookup"><span data-stu-id="0cf33-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-provisioning-policy"></a><span data-ttu-id="0cf33-132">示例1：获取指定设置策略的属性</span><span class="sxs-lookup"><span data-stu-id="0cf33-132">Example 1: Get the properties of the specified provisioning policy</span></span>

#### <a name="request"></a><span data-ttu-id="0cf33-133">请求</span><span class="sxs-lookup"><span data-stu-id="0cf33-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

#### <a name="response"></a><span data-ttu-id="0cf33-134">响应</span><span class="sxs-lookup"><span data-stu-id="0cf33-134">Response</span></span>

<span data-ttu-id="0cf33-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0cf33-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-properties-of-the-specified-provisioning-policy-and-expand-on-the-assignments"></a><span data-ttu-id="0cf33-136">示例2：获取指定的设置策略的属性，并在工作分配上展开</span><span class="sxs-lookup"><span data-stu-id="0cf33-136">Example 2: Get the properties of the specified provisioning policy and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="0cf33-137">请求</span><span class="sxs-lookup"><span data-stu-id="0cf33-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}?$expand=assignments
```

#### <a name="response"></a><span data-ttu-id="0cf33-138">响应</span><span class="sxs-lookup"><span data-stu-id="0cf33-138">Response</span></span>

<span data-ttu-id="0cf33-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0cf33-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
