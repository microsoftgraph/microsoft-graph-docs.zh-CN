---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebb1d6ce33c2f10da19162d40f097c1043af62e8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935278"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="0dc44-103">列出 accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="0dc44-103">List accessPackageResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dc44-104">检索[accessPackageCatalog](../resources/accesspackagecatalog.md)中的[accessPackageResource](../resources/accesspackageresource.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0dc44-104">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0dc44-105">权限</span><span class="sxs-lookup"><span data-stu-id="0dc44-105">Permissions</span></span>

<span data-ttu-id="0dc44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0dc44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0dc44-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dc44-108">Permission type</span></span>                        | <span data-ttu-id="0dc44-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0dc44-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0dc44-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dc44-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="0dc44-111">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="0dc44-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0dc44-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dc44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dc44-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dc44-113">Not supported.</span></span> |
| <span data-ttu-id="0dc44-114">Application</span><span class="sxs-lookup"><span data-stu-id="0dc44-114">Application</span></span>                            | <span data-ttu-id="0dc44-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dc44-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dc44-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dc44-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0dc44-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0dc44-117">Optional query parameters</span></span>

<span data-ttu-id="0dc44-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0dc44-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0dc44-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0dc44-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dc44-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dc44-120">Request headers</span></span>

| <span data-ttu-id="0dc44-121">名称</span><span class="sxs-lookup"><span data-stu-id="0dc44-121">Name</span></span>      |<span data-ttu-id="0dc44-122">说明</span><span class="sxs-lookup"><span data-stu-id="0dc44-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0dc44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dc44-123">Authorization</span></span> | <span data-ttu-id="0dc44-124">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="0dc44-124">Bearer \{token\}.</span></span> <span data-ttu-id="0dc44-125">必填。</span><span class="sxs-lookup"><span data-stu-id="0dc44-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dc44-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dc44-126">Request body</span></span>

<span data-ttu-id="0dc44-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0dc44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dc44-128">响应</span><span class="sxs-lookup"><span data-stu-id="0dc44-128">Response</span></span>

<span data-ttu-id="0dc44-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageResource](../resources/accesspackageresource.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0dc44-129">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0dc44-130">示例</span><span class="sxs-lookup"><span data-stu-id="0dc44-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0dc44-131">请求</span><span class="sxs-lookup"><span data-stu-id="0dc44-131">Request</span></span>

<span data-ttu-id="0dc44-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0dc44-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

### <a name="response"></a><span data-ttu-id="0dc44-133">响应</span><span class="sxs-lookup"><span data-stu-id="0dc44-133">Response</span></span>

<span data-ttu-id="0dc44-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0dc44-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0dc44-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0dc44-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
