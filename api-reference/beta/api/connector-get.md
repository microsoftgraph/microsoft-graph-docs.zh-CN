---
title: 获取连接器
description: 检索连接器对象的属性。
ms.openlocfilehash: f299648093350d4d91637268aa76908f69ca7a38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044596"
---
# <a name="get-connector"></a><span data-ttu-id="1a533-103">获取连接器</span><span class="sxs-lookup"><span data-stu-id="1a533-103">Get connector</span></span>

> <span data-ttu-id="1a533-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a533-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a533-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a533-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a533-106">检索连接器对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a533-106">Retrieve the properties of a connector object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a533-107">权限</span><span class="sxs-lookup"><span data-stu-id="1a533-107">Permissions</span></span>
<span data-ttu-id="1a533-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a533-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a533-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a533-110">Permission type</span></span>      | <span data-ttu-id="1a533-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a533-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a533-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a533-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a533-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a533-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a533-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a533-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a533-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a533-115">Not supported.</span></span>    |
|<span data-ttu-id="1a533-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a533-116">Application</span></span> | <span data-ttu-id="1a533-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a533-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a533-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a533-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a533-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a533-119">Optional query parameters</span></span>
<span data-ttu-id="1a533-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a533-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a533-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a533-121">Request headers</span></span>
| <span data-ttu-id="1a533-122">名称</span><span class="sxs-lookup"><span data-stu-id="1a533-122">Name</span></span>      |<span data-ttu-id="1a533-123">说明</span><span class="sxs-lookup"><span data-stu-id="1a533-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a533-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a533-124">Authorization</span></span>  | <span data-ttu-id="1a533-125">持有者。</span><span class="sxs-lookup"><span data-stu-id="1a533-125">Bearer.</span></span> <span data-ttu-id="1a533-126">必需</span><span class="sxs-lookup"><span data-stu-id="1a533-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a533-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a533-127">Request body</span></span>
<span data-ttu-id="1a533-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a533-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a533-129">响应</span><span class="sxs-lookup"><span data-stu-id="1a533-129">Response</span></span>

<span data-ttu-id="1a533-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[连接器](../resources/connector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a533-130">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a533-131">示例</span><span class="sxs-lookup"><span data-stu-id="1a533-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a533-132">请求</span><span class="sxs-lookup"><span data-stu-id="1a533-132">Request</span></span>
<span data-ttu-id="1a533-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a533-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="1a533-134">响应</span><span class="sxs-lookup"><span data-stu-id="1a533-134">Response</span></span>
<span data-ttu-id="1a533-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a533-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
