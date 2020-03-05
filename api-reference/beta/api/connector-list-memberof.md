---
title: 列出 memberOf
description: 检索连接器所属的 connectorgroup。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b7e64ae1ba20377e64e09857c4e207204cc0beb6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437698"
---
# <a name="list-memberof"></a><span data-ttu-id="7bef5-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="7bef5-103">List memberOf</span></span>

<span data-ttu-id="7bef5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7bef5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bef5-105">检索连接器所属的 connectorgroup。</span><span class="sxs-lookup"><span data-stu-id="7bef5-105">Retrieve the connectorgroup the connector is a member of.</span></span>
## <a name="permissions"></a><span data-ttu-id="7bef5-106">权限</span><span class="sxs-lookup"><span data-stu-id="7bef5-106">Permissions</span></span>
<span data-ttu-id="7bef5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bef5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bef5-109">Permission type</span></span>      | <span data-ttu-id="7bef5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7bef5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bef5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bef5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7bef5-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7bef5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7bef5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bef5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bef5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bef5-114">Not supported.</span></span>    |
|<span data-ttu-id="7bef5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bef5-115">Application</span></span> | <span data-ttu-id="7bef5-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bef5-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bef5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bef5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7bef5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7bef5-118">Optional query parameters</span></span>
<span data-ttu-id="7bef5-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7bef5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bef5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bef5-120">Request headers</span></span>
| <span data-ttu-id="7bef5-121">名称</span><span class="sxs-lookup"><span data-stu-id="7bef5-121">Name</span></span>      |<span data-ttu-id="7bef5-122">说明</span><span class="sxs-lookup"><span data-stu-id="7bef5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bef5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bef5-123">Authorization</span></span>  | <span data-ttu-id="7bef5-124">负载.</span><span class="sxs-lookup"><span data-stu-id="7bef5-124">Bearer.</span></span> <span data-ttu-id="7bef5-125">必需</span><span class="sxs-lookup"><span data-stu-id="7bef5-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bef5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bef5-126">Request body</span></span>
<span data-ttu-id="7bef5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7bef5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bef5-128">响应</span><span class="sxs-lookup"><span data-stu-id="7bef5-128">Response</span></span>

<span data-ttu-id="7bef5-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7bef5-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bef5-130">示例</span><span class="sxs-lookup"><span data-stu-id="7bef5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bef5-131">请求</span><span class="sxs-lookup"><span data-stu-id="7bef5-131">Request</span></span>
<span data-ttu-id="7bef5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bef5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="7bef5-133">响应</span><span class="sxs-lookup"><span data-stu-id="7bef5-133">Response</span></span>
<span data-ttu-id="7bef5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bef5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
