---
title: 获取 privilegedApproval
description: 检索 privilegedapproval 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: d66424622f30ecd91788e9135585921a6af44330
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594941"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="dd611-103">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="dd611-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd611-104">检索 privilegedapproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd611-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd611-105">权限</span><span class="sxs-lookup"><span data-stu-id="dd611-105">Permissions</span></span>
<span data-ttu-id="dd611-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd611-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd611-108">Permission type</span></span>      | <span data-ttu-id="dd611-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd611-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd611-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd611-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd611-111">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="dd611-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="dd611-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd611-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd611-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd611-113">Not supported.</span></span>    |
|<span data-ttu-id="dd611-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd611-114">Application</span></span> | <span data-ttu-id="dd611-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd611-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd611-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd611-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd611-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dd611-117">Optional query parameters</span></span>
<span data-ttu-id="dd611-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd611-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd611-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd611-119">Request headers</span></span>
| <span data-ttu-id="dd611-120">名称</span><span class="sxs-lookup"><span data-stu-id="dd611-120">Name</span></span>      |<span data-ttu-id="dd611-121">说明</span><span class="sxs-lookup"><span data-stu-id="dd611-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd611-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd611-122">Authorization</span></span>  | <span data-ttu-id="dd611-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd611-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd611-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd611-125">Request body</span></span>
<span data-ttu-id="dd611-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd611-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd611-127">响应</span><span class="sxs-lookup"><span data-stu-id="dd611-127">Response</span></span>

<span data-ttu-id="dd611-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd611-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="dd611-129">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="dd611-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dd611-130">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="dd611-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="dd611-131">示例</span><span class="sxs-lookup"><span data-stu-id="dd611-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd611-132">请求</span><span class="sxs-lookup"><span data-stu-id="dd611-132">Request</span></span>
<span data-ttu-id="dd611-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd611-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="dd611-134">响应</span><span class="sxs-lookup"><span data-stu-id="dd611-134">Response</span></span>
<span data-ttu-id="dd611-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd611-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dd611-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dd611-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dd611-139">语言</span><span class="sxs-lookup"><span data-stu-id="dd611-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd611-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd611-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
