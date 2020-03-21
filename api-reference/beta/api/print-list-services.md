---
title: 获取服务
description: 检索 printService 对象的列表，这些对象代表可供租户使用的服务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cbe0735e884e1314dcb4ac62c0cb719ab9592e52
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895953"
---
# <a name="list-services"></a><span data-ttu-id="cffb3-103">列出服务</span><span class="sxs-lookup"><span data-stu-id="cffb3-103">List services</span></span>

<span data-ttu-id="cffb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cffb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cffb3-105">检索[printService](../resources/printservice.md)对象的列表，这些对象代表可供租户使用的**服务**。</span><span class="sxs-lookup"><span data-stu-id="cffb3-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="cffb3-106">权限</span><span class="sxs-lookup"><span data-stu-id="cffb3-106">Permissions</span></span>
<span data-ttu-id="cffb3-107">不需要任何权限即可调用此 API，但用户的租户必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="cffb3-107">No permissions are needed to call this API, but the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="cffb3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cffb3-108">Permission type</span></span> | <span data-ttu-id="cffb3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cffb3-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cffb3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cffb3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="cffb3-111">无。</span><span class="sxs-lookup"><span data-stu-id="cffb3-111">None.</span></span>|
|<span data-ttu-id="cffb3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cffb3-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cffb3-113">无。</span><span class="sxs-lookup"><span data-stu-id="cffb3-113">None.</span></span>|
|<span data-ttu-id="cffb3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cffb3-114">Application</span></span>|<span data-ttu-id="cffb3-115">无。</span><span class="sxs-lookup"><span data-stu-id="cffb3-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cffb3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cffb3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cffb3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cffb3-117">Optional query parameters</span></span>
<span data-ttu-id="cffb3-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cffb3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cffb3-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cffb3-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cffb3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cffb3-120">Request headers</span></span>
| <span data-ttu-id="cffb3-121">名称</span><span class="sxs-lookup"><span data-stu-id="cffb3-121">Name</span></span>      |<span data-ttu-id="cffb3-122">说明</span><span class="sxs-lookup"><span data-stu-id="cffb3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cffb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cffb3-123">Authorization</span></span> | <span data-ttu-id="cffb3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cffb3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cffb3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cffb3-126">Request body</span></span>
<span data-ttu-id="cffb3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cffb3-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cffb3-128">响应</span><span class="sxs-lookup"><span data-stu-id="cffb3-128">Response</span></span>
<span data-ttu-id="cffb3-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printService](../resources/printservice.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cffb3-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cffb3-130">示例</span><span class="sxs-lookup"><span data-stu-id="cffb3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cffb3-131">请求</span><span class="sxs-lookup"><span data-stu-id="cffb3-131">Request</span></span>
<span data-ttu-id="cffb3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cffb3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/print/services
```
##### <a name="response"></a><span data-ttu-id="cffb3-133">响应</span><span class="sxs-lookup"><span data-stu-id="cffb3-133">Response</span></span>
<span data-ttu-id="cffb3-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cffb3-134">The following is an example of the response.</span></span>
><span data-ttu-id="cffb3-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cffb3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->