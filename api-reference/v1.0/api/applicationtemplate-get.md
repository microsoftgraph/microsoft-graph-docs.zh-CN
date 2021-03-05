---
title: 获取 applicationTemplate
description: 检索 applicationtemplate 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: fa9276b3dffd6ecca8df004e469c0dcd562011d9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476419"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="ed08a-103">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="ed08a-103">Get applicationTemplate</span></span>

<span data-ttu-id="ed08a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed08a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed08a-105">检索 [applicationTemplate 对象](../resources/applicationtemplate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ed08a-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed08a-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed08a-106">Permissions</span></span>

<span data-ttu-id="ed08a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed08a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed08a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed08a-109">Permission type</span></span>                        | <span data-ttu-id="ed08a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed08a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ed08a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed08a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed08a-112">无。</span><span class="sxs-lookup"><span data-stu-id="ed08a-112">None.</span></span>                                       |
| <span data-ttu-id="ed08a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed08a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed08a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed08a-114">Not supported.</span></span>                              |
| <span data-ttu-id="ed08a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed08a-115">Application</span></span>                            | <span data-ttu-id="ed08a-116">无。</span><span class="sxs-lookup"><span data-stu-id="ed08a-116">None.</span></span>                                       |

<span data-ttu-id="ed08a-117">调用此 API 不需要其他权限，只要您的应用程序具有调用 Microsoft Graph 的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="ed08a-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="ed08a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed08a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed08a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed08a-119">Optional query parameters</span></span>

<span data-ttu-id="ed08a-120">查询参数 `$select` 可用于仅指定获得最佳性能所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ed08a-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="ed08a-121">始终返回 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="ed08a-121">The **id** property is always returned.</span></span>

<span data-ttu-id="ed08a-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ed08a-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed08a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed08a-123">Request headers</span></span>

| <span data-ttu-id="ed08a-124">名称</span><span class="sxs-lookup"><span data-stu-id="ed08a-124">Name</span></span>          | <span data-ttu-id="ed08a-125">说明</span><span class="sxs-lookup"><span data-stu-id="ed08a-125">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="ed08a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed08a-126">Authorization</span></span> | <span data-ttu-id="ed08a-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ed08a-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed08a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed08a-128">Request body</span></span>

<span data-ttu-id="ed08a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed08a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed08a-130">响应</span><span class="sxs-lookup"><span data-stu-id="ed08a-130">Response</span></span>

<span data-ttu-id="ed08a-131">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [applicationTemplate](../resources/applicationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed08a-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed08a-132">示例</span><span class="sxs-lookup"><span data-stu-id="ed08a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed08a-133">请求</span><span class="sxs-lookup"><span data-stu-id="ed08a-133">Request</span></span>

<span data-ttu-id="ed08a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed08a-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates/{id}
```

### <a name="response"></a><span data-ttu-id="ed08a-135">响应</span><span class="sxs-lookup"><span data-stu-id="ed08a-135">Response</span></span>

<span data-ttu-id="ed08a-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed08a-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ed08a-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed08a-137">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
