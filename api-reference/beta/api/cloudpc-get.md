---
title: 获取 cloudPC
description: 查看 cloudPC 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ad63ff3f4d152005624872f94482b44cb862ef9f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082214"
---
# <a name="get-cloudpc"></a><span data-ttu-id="30a5a-103">获取 cloudPC</span><span class="sxs-lookup"><span data-stu-id="30a5a-103">Get cloudPC</span></span>

<span data-ttu-id="30a5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a5a-105">读取特定 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30a5a-105">Read the properties and relationships of a specific [cloudPC](../resources/cloudpc.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="30a5a-106">权限</span><span class="sxs-lookup"><span data-stu-id="30a5a-106">Permissions</span></span>

<span data-ttu-id="30a5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a5a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="30a5a-109">Permission type</span></span>|<span data-ttu-id="30a5a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30a5a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30a5a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30a5a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30a5a-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a5a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="30a5a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30a5a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30a5a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="30a5a-114">Not supported.</span></span>|
|<span data-ttu-id="30a5a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="30a5a-115">Application</span></span>|<span data-ttu-id="30a5a-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a5a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30a5a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30a5a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30a5a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="30a5a-118">Optional query parameters</span></span>

<span data-ttu-id="30a5a-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="30a5a-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="30a5a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="30a5a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="30a5a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="30a5a-121">Request headers</span></span>

| <span data-ttu-id="30a5a-122">名称</span><span class="sxs-lookup"><span data-stu-id="30a5a-122">Name</span></span>          | <span data-ttu-id="30a5a-123">说明</span><span class="sxs-lookup"><span data-stu-id="30a5a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="30a5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="30a5a-124">Authorization</span></span> | <span data-ttu-id="30a5a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30a5a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30a5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="30a5a-127">Request body</span></span>

<span data-ttu-id="30a5a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30a5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30a5a-129">响应</span><span class="sxs-lookup"><span data-stu-id="30a5a-129">Response</span></span>

<span data-ttu-id="30a5a-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [cloudPC](../resources/cloudpc.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30a5a-130">If successful, this method returns a `200 OK` response code and a [cloudPC](../resources/cloudpc.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30a5a-131">示例</span><span class="sxs-lookup"><span data-stu-id="30a5a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30a5a-132">请求</span><span class="sxs-lookup"><span data-stu-id="30a5a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="30a5a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="30a5a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpc"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}
```
# <a name="c"></a>[<span data-ttu-id="30a5a-134">C#</span><span class="sxs-lookup"><span data-stu-id="30a5a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30a5a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a5a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30a5a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30a5a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30a5a-137">Java</span><span class="sxs-lookup"><span data-stu-id="30a5a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30a5a-138">响应</span><span class="sxs-lookup"><span data-stu-id="30a5a-138">Response</span></span>

<span data-ttu-id="30a5a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="30a5a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_cloudpc",
  "@odata.type": "microsoft.graph.cloudPC"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPC",
    "id": "ac74ae8b-85f7-4272-88cc-54192674ffff",
    "displayName": "Demo-0",
    "imageDisplayName": "Windows-10 19h1-evd",
    "managedDeviceId": "e87f50c7-fa7f-4687-aade-dd45f3d6ffff",  
    "managedDeviceName": "A00002GI001",
    "provisioningPolicyId": "13fa0778-ba00-438a-96d3-488c8602ffff",
    "provisioningPolicyName": "Marketing provisioning policy",
    "onPremisesConnectionName": "on-Premises connection for Marketing",
    "servicePlanId": "da5615b4-a484-4742-a019-2d52c91cffff",
    "servicePlanName": "standard",
    "status": "failed",
    "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails",
    "code": "internalServerError",
    "message": "There was an internal server error. Please contact support xxx.",
    "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "correlationId",
          "value": "52367774-cfb7-4e9c-ab51-1b864c31f2d1"
        }
      ]
    },
    "userPrincipalName": "pmitchell@cpccustomer001.onmicrosoft.com",
    "lastModifiedDateTime": "2020-11-03T18:14:34Z",
    "gracePeriodEndDateTime": "2020-11-010T20:00:34Z"
  }
}
```
