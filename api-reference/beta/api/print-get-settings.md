---
title: 获取设置
description: 检索通用打印服务的租户范围设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 675e0c41e0aa9605b0a6088e13be78e9d52d57be
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895965"
---
# <a name="get-settings"></a><span data-ttu-id="a468f-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="a468f-103">Get settings</span></span>

<span data-ttu-id="a468f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a468f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a468f-105">检索通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="a468f-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="a468f-106">权限</span><span class="sxs-lookup"><span data-stu-id="a468f-106">Permissions</span></span>
<span data-ttu-id="a468f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a468f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a468f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a468f-109">Permission type</span></span> | <span data-ttu-id="a468f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a468f-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a468f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a468f-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a468f-112">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="a468f-112">Users.Read.All</span></span> |
|<span data-ttu-id="a468f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a468f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a468f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a468f-114">Not Supported.</span></span>|
|<span data-ttu-id="a468f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a468f-115">Application</span></span>|<span data-ttu-id="a468f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a468f-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a468f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a468f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a468f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a468f-118">Optional query parameters</span></span>
<span data-ttu-id="a468f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a468f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a468f-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a468f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a468f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a468f-121">Request headers</span></span>
| <span data-ttu-id="a468f-122">名称</span><span class="sxs-lookup"><span data-stu-id="a468f-122">Name</span></span>      |<span data-ttu-id="a468f-123">说明</span><span class="sxs-lookup"><span data-stu-id="a468f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a468f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a468f-124">Authorization</span></span> | <span data-ttu-id="a468f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a468f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a468f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a468f-127">Request body</span></span>
<span data-ttu-id="a468f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a468f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a468f-129">响应</span><span class="sxs-lookup"><span data-stu-id="a468f-129">Response</span></span>
<span data-ttu-id="a468f-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[printSettings](../resources/printsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a468f-130">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a468f-131">示例</span><span class="sxs-lookup"><span data-stu-id="a468f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a468f-132">请求</span><span class="sxs-lookup"><span data-stu-id="a468f-132">Request</span></span>
<span data-ttu-id="a468f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a468f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```http
GET https://graph.microsoft.com/beta/print/settings
```
##### <a name="response"></a><span data-ttu-id="a468f-134">响应</span><span class="sxs-lookup"><span data-stu-id="a468f-134">Response</span></span>
<span data-ttu-id="a468f-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a468f-135">The following is an example of the response.</span></span>
><span data-ttu-id="a468f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a468f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->