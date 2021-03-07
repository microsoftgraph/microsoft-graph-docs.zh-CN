---
title: 列出 printServices
description: 检索 printService 对象列表，这些对象代表可供租户使用的服务。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c5226eadd4edfd3e8d2d15534eed3fcb5ffc9619
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517008"
---
# <a name="list-printservices"></a><span data-ttu-id="6e64b-103">列出 printServices</span><span class="sxs-lookup"><span data-stu-id="6e64b-103">List printServices</span></span>
<span data-ttu-id="6e64b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e64b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6e64b-105">检索 **printService** 对象列表，这些对象代表可供租户使用的服务。</span><span class="sxs-lookup"><span data-stu-id="6e64b-105">Retrieve a list of **printService** objects that represent the services available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e64b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e64b-106">Permissions</span></span>
<span data-ttu-id="6e64b-107">调用 **此** API 需要其中 [](/graph/permissions-reference#universal-print-permissions)一个委派的通用打印权限。</span><span class="sxs-lookup"><span data-stu-id="6e64b-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="6e64b-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e64b-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e64b-109">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e64b-109">Optional query parameters</span></span>
<span data-ttu-id="6e64b-110">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e64b-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6e64b-111">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6e64b-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e64b-112">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e64b-112">Request headers</span></span>
|<span data-ttu-id="6e64b-113">名称</span><span class="sxs-lookup"><span data-stu-id="6e64b-113">Name</span></span>|<span data-ttu-id="6e64b-114">说明</span><span class="sxs-lookup"><span data-stu-id="6e64b-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e64b-115">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e64b-115">Authorization</span></span>|<span data-ttu-id="6e64b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e64b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e64b-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e64b-118">Request body</span></span>
<span data-ttu-id="6e64b-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e64b-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e64b-120">响应</span><span class="sxs-lookup"><span data-stu-id="6e64b-120">Response</span></span>

<span data-ttu-id="6e64b-121">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printService](../resources/printservice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e64b-121">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e64b-122">示例</span><span class="sxs-lookup"><span data-stu-id="6e64b-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e64b-123">请求</span><span class="sxs-lookup"><span data-stu-id="6e64b-123">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```


### <a name="response"></a><span data-ttu-id="6e64b-124">响应</span><span class="sxs-lookup"><span data-stu-id="6e64b-124">Response</span></span>
<span data-ttu-id="6e64b-125">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6e64b-125">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printService)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

