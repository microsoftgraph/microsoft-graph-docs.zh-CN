---
title: 列表 privilegedApproval
description: 检索 privilegedapproval 对象的列表。
ms.openlocfilehash: 35b3e2cf6b4034731c8ddf9d1af41e129acbfe3f
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748169"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="fa93d-103">列表 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="fa93d-103">List privilegedApproval</span></span>

> <span data-ttu-id="fa93d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa93d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa93d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa93d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa93d-106">检索 privilegedapproval 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="fa93d-106">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="fa93d-107">若要筛选查询的结果，请使用标准 OData ``$filter`` Uri 中的表达式。</span><span class="sxs-lookup"><span data-stu-id="fa93d-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa93d-108">权限</span><span class="sxs-lookup"><span data-stu-id="fa93d-108">Permissions</span></span>
<span data-ttu-id="fa93d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa93d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa93d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa93d-111">Permission type</span></span>      | <span data-ttu-id="fa93d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa93d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa93d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa93d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa93d-114">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa93d-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa93d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa93d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa93d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa93d-116">Not supported.</span></span>    |
|<span data-ttu-id="fa93d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa93d-117">Application</span></span> | <span data-ttu-id="fa93d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa93d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa93d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa93d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa93d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fa93d-120">Optional query parameters</span></span>
<span data-ttu-id="fa93d-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fa93d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa93d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa93d-122">Request headers</span></span>
| <span data-ttu-id="fa93d-123">名称</span><span class="sxs-lookup"><span data-stu-id="fa93d-123">Name</span></span>      |<span data-ttu-id="fa93d-124">说明</span><span class="sxs-lookup"><span data-stu-id="fa93d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa93d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa93d-125">Authorization</span></span>  | <span data-ttu-id="fa93d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa93d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa93d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa93d-128">Request body</span></span>
<span data-ttu-id="fa93d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa93d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa93d-130">响应</span><span class="sxs-lookup"><span data-stu-id="fa93d-130">Response</span></span>

<span data-ttu-id="fa93d-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedApproval](../resources/privilegedapproval.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="fa93d-131">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="fa93d-132">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="fa93d-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="fa93d-133">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="fa93d-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="fa93d-134">示例</span><span class="sxs-lookup"><span data-stu-id="fa93d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa93d-135">请求</span><span class="sxs-lookup"><span data-stu-id="fa93d-135">Request</span></span>
<span data-ttu-id="fa93d-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa93d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="fa93d-137">响应</span><span class="sxs-lookup"><span data-stu-id="fa93d-137">Response</span></span>
<span data-ttu-id="fa93d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa93d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
