---
title: 获取 connectorGroup
description: 检索 connectorGroup 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 57759efae263639da38ba74b6e3123c30a7e8878
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437474"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="e309d-103">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e309d-103">Get connectorGroup</span></span>

<span data-ttu-id="e309d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e309d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e309d-105">检索 connectorGroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e309d-105">Retrieve the properties of a connectorGroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e309d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e309d-106">Permissions</span></span>
<span data-ttu-id="e309d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e309d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e309d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e309d-109">Permission type</span></span>      | <span data-ttu-id="e309d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e309d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e309d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e309d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e309d-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e309d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e309d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e309d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e309d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e309d-114">Not supported.</span></span>    |
|<span data-ttu-id="e309d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e309d-115">Application</span></span> | <span data-ttu-id="e309d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e309d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e309d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e309d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e309d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e309d-118">Optional query parameters</span></span>
<span data-ttu-id="e309d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e309d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e309d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e309d-120">Request headers</span></span>
| <span data-ttu-id="e309d-121">名称</span><span class="sxs-lookup"><span data-stu-id="e309d-121">Name</span></span>      |<span data-ttu-id="e309d-122">说明</span><span class="sxs-lookup"><span data-stu-id="e309d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e309d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e309d-123">Authorization</span></span>  | <span data-ttu-id="e309d-124">负载.</span><span class="sxs-lookup"><span data-stu-id="e309d-124">Bearer.</span></span> <span data-ttu-id="e309d-125">必需</span><span class="sxs-lookup"><span data-stu-id="e309d-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e309d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e309d-126">Request body</span></span>
<span data-ttu-id="e309d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e309d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e309d-128">响应</span><span class="sxs-lookup"><span data-stu-id="e309d-128">Response</span></span>

<span data-ttu-id="e309d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e309d-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e309d-130">示例</span><span class="sxs-lookup"><span data-stu-id="e309d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e309d-131">请求</span><span class="sxs-lookup"><span data-stu-id="e309d-131">Request</span></span>
<span data-ttu-id="e309d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e309d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="e309d-133">响应</span><span class="sxs-lookup"><span data-stu-id="e309d-133">Response</span></span>
<span data-ttu-id="e309d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e309d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isDefault": true
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
