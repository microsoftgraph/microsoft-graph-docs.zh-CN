---
title: 列表 administrativeUnits
description: 检索 administrativeUnit 对象的列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cb2369d4badff139cfdb209174294911b5fd385
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936849"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="01095-103">列表 administrativeUnits</span><span class="sxs-lookup"><span data-stu-id="01095-103">List administrativeUnits</span></span>

> <span data-ttu-id="01095-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01095-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01095-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01095-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01095-106">检索[administrativeUnit](../resources/administrativeunit.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="01095-106">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="01095-107">权限</span><span class="sxs-lookup"><span data-stu-id="01095-107">Permissions</span></span>
<span data-ttu-id="01095-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01095-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01095-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01095-110">Permission type</span></span>      | <span data-ttu-id="01095-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01095-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01095-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01095-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01095-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01095-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01095-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01095-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01095-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01095-115">Not supported.</span></span>    |
|<span data-ttu-id="01095-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01095-116">Application</span></span> | <span data-ttu-id="01095-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01095-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01095-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01095-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01095-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01095-119">Optional query parameters</span></span>
<span data-ttu-id="01095-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01095-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01095-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="01095-121">Request headers</span></span>
| <span data-ttu-id="01095-122">名称</span><span class="sxs-lookup"><span data-stu-id="01095-122">Name</span></span>      |<span data-ttu-id="01095-123">说明</span><span class="sxs-lookup"><span data-stu-id="01095-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01095-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="01095-124">Authorization</span></span>  | <span data-ttu-id="01095-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01095-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01095-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="01095-127">Request body</span></span>
<span data-ttu-id="01095-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01095-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01095-129">响应</span><span class="sxs-lookup"><span data-stu-id="01095-129">Response</span></span>

<span data-ttu-id="01095-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[administrativeUnit](../resources/administrativeunit.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="01095-130">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01095-131">示例</span><span class="sxs-lookup"><span data-stu-id="01095-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01095-132">请求</span><span class="sxs-lookup"><span data-stu-id="01095-132">Request</span></span>
<span data-ttu-id="01095-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01095-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits
```
##### <a name="response"></a><span data-ttu-id="01095-134">响应</span><span class="sxs-lookup"><span data-stu-id="01095-134">Response</span></span>
<span data-ttu-id="01095-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01095-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "value": [
    {
      "displayName": "displayName-value",
      "description": "description-value",
      "visibility": "visibility-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List administrativeUnits",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
