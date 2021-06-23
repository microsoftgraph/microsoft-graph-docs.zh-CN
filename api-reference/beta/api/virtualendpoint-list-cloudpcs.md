---
title: 列出 cloudPCs
description: 列出 cloudPC 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 49cdea1b601e33210bc2861ee350086377fe05f8
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082382"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="20bfc-103">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="20bfc-103">List cloudPCs</span></span>

<span data-ttu-id="20bfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20bfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20bfc-105">列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="20bfc-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="20bfc-106">权限</span><span class="sxs-lookup"><span data-stu-id="20bfc-106">Permissions</span></span>

<span data-ttu-id="20bfc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20bfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20bfc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20bfc-109">Permission type</span></span>|<span data-ttu-id="20bfc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20bfc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20bfc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20bfc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20bfc-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20bfc-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="20bfc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20bfc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20bfc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20bfc-114">Not supported.</span></span>|
|<span data-ttu-id="20bfc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20bfc-115">Application</span></span>|<span data-ttu-id="20bfc-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20bfc-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20bfc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20bfc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20bfc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20bfc-118">Optional query parameters</span></span>

<span data-ttu-id="20bfc-119">此方法支持 `$select` 、 `$filter` 和 `$count` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="20bfc-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="20bfc-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="20bfc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20bfc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="20bfc-121">Request headers</span></span>

| <span data-ttu-id="20bfc-122">名称</span><span class="sxs-lookup"><span data-stu-id="20bfc-122">Name</span></span>          | <span data-ttu-id="20bfc-123">说明</span><span class="sxs-lookup"><span data-stu-id="20bfc-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="20bfc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="20bfc-124">Authorization</span></span> | <span data-ttu-id="20bfc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20bfc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20bfc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="20bfc-127">Request body</span></span>

<span data-ttu-id="20bfc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20bfc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20bfc-129">响应</span><span class="sxs-lookup"><span data-stu-id="20bfc-129">Response</span></span>

<span data-ttu-id="20bfc-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPC](../resources/cloudpc.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="20bfc-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20bfc-131">示例</span><span class="sxs-lookup"><span data-stu-id="20bfc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20bfc-132">请求</span><span class="sxs-lookup"><span data-stu-id="20bfc-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="20bfc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="20bfc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```
# <a name="c"></a>[<span data-ttu-id="20bfc-134">C#</span><span class="sxs-lookup"><span data-stu-id="20bfc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20bfc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20bfc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20bfc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20bfc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20bfc-137">Java</span><span class="sxs-lookup"><span data-stu-id="20bfc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20bfc-138">响应</span><span class="sxs-lookup"><span data-stu-id="20bfc-138">Response</span></span>

<span data-ttu-id="20bfc-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="20bfc-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName": "Demo-1",
      "imageDisplayName": "Windows-10 19h1-evd",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "A00002GI001",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "provisioningPolicyName": "HR provisioning policy",
      "onPremisesConnectionName": "on-Premises connection for HR",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "pmitchell@cpccustomer001.onmicrosoft.com",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null,
      "gracePeriodEndDateTime": "2020-11-010T20:00:34Z"
    }
  ]
}
```
