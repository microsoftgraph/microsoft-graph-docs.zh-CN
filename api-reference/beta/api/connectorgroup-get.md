---
title: 获取 connectorGroup
description: 检索 connectorGroup 对象的属性。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d487874241d6a557cd9548a7501f0a27b9b11f9
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556056"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="16930-103">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="16930-103">Get connectorGroup</span></span>

<span data-ttu-id="16930-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16930-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16930-105">检索[connectorGroup](../resources/connectorgroup.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="16930-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16930-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="16930-106">Permissions</span></span>
<span data-ttu-id="16930-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16930-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16930-109">Permission type</span></span>      | <span data-ttu-id="16930-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16930-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16930-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16930-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16930-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16930-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16930-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16930-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16930-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16930-114">Not supported.</span></span>    |
|<span data-ttu-id="16930-115">Application</span><span class="sxs-lookup"><span data-stu-id="16930-115">Application</span></span> | <span data-ttu-id="16930-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16930-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16930-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16930-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16930-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16930-118">Optional query parameters</span></span>
<span data-ttu-id="16930-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16930-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16930-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="16930-120">Request headers</span></span>
| <span data-ttu-id="16930-121">名称</span><span class="sxs-lookup"><span data-stu-id="16930-121">Name</span></span>      |<span data-ttu-id="16930-122">说明</span><span class="sxs-lookup"><span data-stu-id="16930-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16930-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16930-123">Authorization</span></span>  | <span data-ttu-id="16930-124">负载.</span><span class="sxs-lookup"><span data-stu-id="16930-124">Bearer.</span></span> <span data-ttu-id="16930-125">必需</span><span class="sxs-lookup"><span data-stu-id="16930-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="16930-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16930-126">Request body</span></span>
<span data-ttu-id="16930-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16930-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16930-128">响应</span><span class="sxs-lookup"><span data-stu-id="16930-128">Response</span></span>

<span data-ttu-id="16930-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16930-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16930-130">示例</span><span class="sxs-lookup"><span data-stu-id="16930-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16930-131">请求</span><span class="sxs-lookup"><span data-stu-id="16930-131">Request</span></span>
<span data-ttu-id="16930-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16930-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="16930-133">响应</span><span class="sxs-lookup"><span data-stu-id="16930-133">Response</span></span>
<span data-ttu-id="16930-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16930-134">The following is an example of the response.</span></span> <span data-ttu-id="16930-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16930-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16930-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16930-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
