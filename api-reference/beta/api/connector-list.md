---
title: 列表连接器
description: 检索连接器对象的列表。
ms.openlocfilehash: 663105bc3f2ac7ae8826a22dc6c849d1095551d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041645"
---
# <a name="list-connectors"></a><span data-ttu-id="ef131-103">列表连接器</span><span class="sxs-lookup"><span data-stu-id="ef131-103">List connectors</span></span>

> <span data-ttu-id="ef131-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ef131-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef131-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ef131-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef131-106">检索连接器对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ef131-106">Retrieve a list of connector objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef131-107">权限</span><span class="sxs-lookup"><span data-stu-id="ef131-107">Permissions</span></span>
<span data-ttu-id="ef131-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef131-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef131-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef131-110">Permission type</span></span>      | <span data-ttu-id="ef131-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef131-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef131-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef131-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef131-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef131-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef131-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef131-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef131-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef131-115">Not supported.</span></span>    |
|<span data-ttu-id="ef131-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef131-116">Application</span></span> | <span data-ttu-id="ef131-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef131-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef131-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef131-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef131-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ef131-119">Optional query parameters</span></span>
<span data-ttu-id="ef131-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ef131-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef131-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef131-121">Request headers</span></span>
| <span data-ttu-id="ef131-122">名称</span><span class="sxs-lookup"><span data-stu-id="ef131-122">Name</span></span>      |<span data-ttu-id="ef131-123">说明</span><span class="sxs-lookup"><span data-stu-id="ef131-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef131-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef131-124">Authorization</span></span>  | <span data-ttu-id="ef131-125">持有者。</span><span class="sxs-lookup"><span data-stu-id="ef131-125">Bearer.</span></span> <span data-ttu-id="ef131-126">必需</span><span class="sxs-lookup"><span data-stu-id="ef131-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef131-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef131-127">Request body</span></span>
<span data-ttu-id="ef131-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef131-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef131-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef131-129">Response</span></span>

<span data-ttu-id="ef131-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[连接器](../resources/connector.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="ef131-130">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef131-131">示例</span><span class="sxs-lookup"><span data-stu-id="ef131-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef131-132">请求</span><span class="sxs-lookup"><span data-stu-id="ef131-132">Request</span></span>
<span data-ttu-id="ef131-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef131-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors
```
##### <a name="response"></a><span data-ttu-id="ef131-134">响应</span><span class="sxs-lookup"><span data-stu-id="ef131-134">Response</span></span>
<span data-ttu-id="ef131-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef131-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
