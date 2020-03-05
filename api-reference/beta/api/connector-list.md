---
title: 列出连接器
description: 检索连接器对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 75efa2301a4bb6e51bc50ec2cac768ef2ab0f76a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437614"
---
# <a name="list-connectors"></a><span data-ttu-id="f05aa-103">列出连接器</span><span class="sxs-lookup"><span data-stu-id="f05aa-103">List connectors</span></span>

<span data-ttu-id="f05aa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f05aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f05aa-105">检索连接器对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f05aa-105">Retrieve a list of connector objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f05aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="f05aa-106">Permissions</span></span>
<span data-ttu-id="f05aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f05aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f05aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f05aa-109">Permission type</span></span>      | <span data-ttu-id="f05aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f05aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f05aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f05aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f05aa-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f05aa-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f05aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f05aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f05aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f05aa-114">Not supported.</span></span>    |
|<span data-ttu-id="f05aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f05aa-115">Application</span></span> | <span data-ttu-id="f05aa-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f05aa-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f05aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f05aa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f05aa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f05aa-118">Optional query parameters</span></span>
<span data-ttu-id="f05aa-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f05aa-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f05aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f05aa-120">Request headers</span></span>
| <span data-ttu-id="f05aa-121">名称</span><span class="sxs-lookup"><span data-stu-id="f05aa-121">Name</span></span>      |<span data-ttu-id="f05aa-122">说明</span><span class="sxs-lookup"><span data-stu-id="f05aa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f05aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f05aa-123">Authorization</span></span>  | <span data-ttu-id="f05aa-124">负载.</span><span class="sxs-lookup"><span data-stu-id="f05aa-124">Bearer.</span></span> <span data-ttu-id="f05aa-125">必需</span><span class="sxs-lookup"><span data-stu-id="f05aa-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f05aa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f05aa-126">Request body</span></span>
<span data-ttu-id="f05aa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f05aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f05aa-128">响应</span><span class="sxs-lookup"><span data-stu-id="f05aa-128">Response</span></span>

<span data-ttu-id="f05aa-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[连接器](../resources/connector.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f05aa-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f05aa-130">示例</span><span class="sxs-lookup"><span data-stu-id="f05aa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f05aa-131">请求</span><span class="sxs-lookup"><span data-stu-id="f05aa-131">Request</span></span>
<span data-ttu-id="f05aa-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f05aa-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors
```
##### <a name="response"></a><span data-ttu-id="f05aa-133">响应</span><span class="sxs-lookup"><span data-stu-id="f05aa-133">Response</span></span>
<span data-ttu-id="f05aa-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f05aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
