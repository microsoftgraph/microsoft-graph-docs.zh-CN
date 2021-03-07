---
title: 获取 printService
description: 检索打印服务的属性和关系。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 19ddebf1697e75822d08bc92825b17e5b4b540c0
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517160"
---
# <a name="get-printservice"></a><span data-ttu-id="20b9a-103">获取 printService</span><span class="sxs-lookup"><span data-stu-id="20b9a-103">Get printService</span></span>
<span data-ttu-id="20b9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20b9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="20b9a-105">检索打印服务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="20b9a-105">Retrieve the properties and relationships of a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="20b9a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="20b9a-106">Permissions</span></span>
<span data-ttu-id="20b9a-107">调用 **此** API 需要其中 [](/graph/permissions-reference#universal-print-permissions)一个委派的通用打印权限。</span><span class="sxs-lookup"><span data-stu-id="20b9a-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="20b9a-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20b9a-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services/{printServiceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20b9a-109">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20b9a-109">Optional query parameters</span></span>
<span data-ttu-id="20b9a-110">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="20b9a-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="20b9a-111">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="20b9a-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20b9a-112">请求标头</span><span class="sxs-lookup"><span data-stu-id="20b9a-112">Request headers</span></span>
|<span data-ttu-id="20b9a-113">名称</span><span class="sxs-lookup"><span data-stu-id="20b9a-113">Name</span></span>|<span data-ttu-id="20b9a-114">说明</span><span class="sxs-lookup"><span data-stu-id="20b9a-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20b9a-115">Authorization</span><span class="sxs-lookup"><span data-stu-id="20b9a-115">Authorization</span></span>|<span data-ttu-id="20b9a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20b9a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b9a-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="20b9a-118">Request body</span></span>
<span data-ttu-id="20b9a-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20b9a-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20b9a-120">响应</span><span class="sxs-lookup"><span data-stu-id="20b9a-120">Response</span></span>

<span data-ttu-id="20b9a-121">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [printService](../resources/printservice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20b9a-121">If successful, this method returns a `200 OK` response code and a [printService](../resources/printservice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20b9a-122">示例</span><span class="sxs-lookup"><span data-stu-id="20b9a-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20b9a-123">请求</span><span class="sxs-lookup"><span data-stu-id="20b9a-123">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services/{printServiceId}
```


### <a name="response"></a><span data-ttu-id="20b9a-124">响应</span><span class="sxs-lookup"><span data-stu-id="20b9a-124">Response</span></span>
<span data-ttu-id="20b9a-125">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="20b9a-125">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services/$entity",
  "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
  "endpoints": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

