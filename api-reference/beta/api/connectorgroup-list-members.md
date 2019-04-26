---
title: 列出成员
description: 检索与 connectorGroup 相关联的连接器对象的列表。
localization_priority: Normal
ms.openlocfilehash: 0ceb5c6e0af7d9b661cbd32c2a7412322be1cf91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327504"
---
# <a name="list-members"></a><span data-ttu-id="582d6-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="582d6-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="582d6-104">检索与 connectorGroup 相关联的连接器对象的列表。</span><span class="sxs-lookup"><span data-stu-id="582d6-104">Retrieve a list of connector objects associated with a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="582d6-105">权限</span><span class="sxs-lookup"><span data-stu-id="582d6-105">Permissions</span></span>
<span data-ttu-id="582d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="582d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="582d6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="582d6-108">Permission type</span></span>      | <span data-ttu-id="582d6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="582d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="582d6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="582d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="582d6-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="582d6-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="582d6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="582d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="582d6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="582d6-113">Not supported.</span></span>    |
|<span data-ttu-id="582d6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="582d6-114">Application</span></span> | <span data-ttu-id="582d6-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="582d6-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="582d6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="582d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="582d6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="582d6-117">Optional query parameters</span></span>
<span data-ttu-id="582d6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="582d6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="582d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="582d6-119">Request headers</span></span>
| <span data-ttu-id="582d6-120">名称</span><span class="sxs-lookup"><span data-stu-id="582d6-120">Name</span></span>      |<span data-ttu-id="582d6-121">说明</span><span class="sxs-lookup"><span data-stu-id="582d6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="582d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="582d6-122">Authorization</span></span>  | <span data-ttu-id="582d6-123">负载.</span><span class="sxs-lookup"><span data-stu-id="582d6-123">Bearer.</span></span> <span data-ttu-id="582d6-124">必需</span><span class="sxs-lookup"><span data-stu-id="582d6-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="582d6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="582d6-125">Request body</span></span>
<span data-ttu-id="582d6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="582d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="582d6-127">响应</span><span class="sxs-lookup"><span data-stu-id="582d6-127">Response</span></span>

<span data-ttu-id="582d6-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[连接器](../resources/connector.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="582d6-128">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="582d6-129">示例</span><span class="sxs-lookup"><span data-stu-id="582d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="582d6-130">请求</span><span class="sxs-lookup"><span data-stu-id="582d6-130">Request</span></span>
<span data-ttu-id="582d6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="582d6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="582d6-132">响应</span><span class="sxs-lookup"><span data-stu-id="582d6-132">Response</span></span>
<span data-ttu-id="582d6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="582d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
