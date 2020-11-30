---
title: 列出 cloudPCs
description: 列出 cloudPC 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: cb7b5e79d3fd490fc574fbfbb8c08988321bc86d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378314"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="906e0-103">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="906e0-103">List cloudPCs</span></span>

<span data-ttu-id="906e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="906e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="906e0-105">列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="906e0-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="906e0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="906e0-106">Permissions</span></span>

<span data-ttu-id="906e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="906e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="906e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="906e0-109">Permission type</span></span>|<span data-ttu-id="906e0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="906e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="906e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="906e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="906e0-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="906e0-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="906e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="906e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="906e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="906e0-114">Not supported.</span></span>|
|<span data-ttu-id="906e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="906e0-115">Application</span></span>|<span data-ttu-id="906e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="906e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="906e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="906e0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="906e0-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="906e0-118">Optional query parameters</span></span>

<span data-ttu-id="906e0-119">此方法支持 `$select` `$filter` 和 `$count` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="906e0-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="906e0-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="906e0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="906e0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="906e0-121">Request headers</span></span>

| <span data-ttu-id="906e0-122">名称</span><span class="sxs-lookup"><span data-stu-id="906e0-122">Name</span></span>          | <span data-ttu-id="906e0-123">说明</span><span class="sxs-lookup"><span data-stu-id="906e0-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="906e0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="906e0-124">Authorization</span></span> | <span data-ttu-id="906e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="906e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="906e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="906e0-127">Request body</span></span>

<span data-ttu-id="906e0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="906e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="906e0-129">响应</span><span class="sxs-lookup"><span data-stu-id="906e0-129">Response</span></span>

<span data-ttu-id="906e0-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPC](../resources/cloudpc.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="906e0-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="906e0-131">示例</span><span class="sxs-lookup"><span data-stu-id="906e0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="906e0-132">请求</span><span class="sxs-lookup"><span data-stu-id="906e0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```

### <a name="response"></a><span data-ttu-id="906e0-133">响应</span><span class="sxs-lookup"><span data-stu-id="906e0-133">Response</span></span>

<span data-ttu-id="906e0-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="906e0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPC)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPC",
      "id": "662009bc-7732-4f6f-8726-25883518ffff",
      "displayName": "Display Name value",
      "imageDisplayName": "Image Display Name value",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "Managed Device Name value",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "User Principal Name value",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null
    }
  ]
}
```
