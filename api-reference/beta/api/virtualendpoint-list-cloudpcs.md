---
title: 列出 cloudPCs
description: 列出 cloudPC 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3c2830f53c7060ff96e164c127afb83072b96c86
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785870"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="6c38c-103">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="6c38c-103">List cloudPCs</span></span>

<span data-ttu-id="6c38c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c38c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c38c-105">列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6c38c-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="6c38c-106">权限</span><span class="sxs-lookup"><span data-stu-id="6c38c-106">Permissions</span></span>

<span data-ttu-id="6c38c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c38c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c38c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c38c-109">Permission type</span></span>|<span data-ttu-id="6c38c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c38c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c38c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c38c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c38c-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c38c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="6c38c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c38c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c38c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c38c-114">Not supported.</span></span>|
|<span data-ttu-id="6c38c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c38c-115">Application</span></span>|<span data-ttu-id="6c38c-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c38c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c38c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c38c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c38c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c38c-118">Optional query parameters</span></span>

<span data-ttu-id="6c38c-119">此方法支持 `$select` 、 `$filter` 和 `$count` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c38c-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c38c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6c38c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c38c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c38c-121">Request headers</span></span>

| <span data-ttu-id="6c38c-122">名称</span><span class="sxs-lookup"><span data-stu-id="6c38c-122">Name</span></span>          | <span data-ttu-id="6c38c-123">说明</span><span class="sxs-lookup"><span data-stu-id="6c38c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6c38c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c38c-124">Authorization</span></span> | <span data-ttu-id="6c38c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c38c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c38c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c38c-127">Request body</span></span>

<span data-ttu-id="6c38c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c38c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c38c-129">响应</span><span class="sxs-lookup"><span data-stu-id="6c38c-129">Response</span></span>

<span data-ttu-id="6c38c-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPC](../resources/cloudpc.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6c38c-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c38c-131">示例</span><span class="sxs-lookup"><span data-stu-id="6c38c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c38c-132">请求</span><span class="sxs-lookup"><span data-stu-id="6c38c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c38c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c38c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```
# <a name="c"></a>[<span data-ttu-id="6c38c-134">C#</span><span class="sxs-lookup"><span data-stu-id="6c38c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c38c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c38c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c38c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c38c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c38c-137">Java</span><span class="sxs-lookup"><span data-stu-id="6c38c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c38c-138">响应</span><span class="sxs-lookup"><span data-stu-id="6c38c-138">Response</span></span>

<span data-ttu-id="6c38c-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6c38c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "provisioningPolicyName": "Provisioning Policy Name value",
      "onPremisesConnectionName": "On-premises connection Name value",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "User Principal Name value",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null,
      "gracePeriodEndDateTime": "Grace Period End Date Time value "
    }
  ]
}
```
