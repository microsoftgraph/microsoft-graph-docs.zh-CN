---
title: 列出 privilegedApproval
description: 检索 privilegedapproval 对象的列表。
localization_priority: Normal
ms.openlocfilehash: 2e3adb6a85906c234ff64cf18b193a1156e35d14
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596427"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="80c40-103">列出 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="80c40-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80c40-104">检索 privilegedapproval 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="80c40-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="80c40-105">若要筛选查询中的结果，请在 URL 中使用标准 OData ``$filter`` 表达式。</span><span class="sxs-lookup"><span data-stu-id="80c40-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="80c40-106">权限</span><span class="sxs-lookup"><span data-stu-id="80c40-106">Permissions</span></span>
<span data-ttu-id="80c40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80c40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="80c40-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80c40-109">Permission type</span></span>      | <span data-ttu-id="80c40-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80c40-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80c40-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80c40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80c40-112">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="80c40-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80c40-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80c40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80c40-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80c40-114">Not supported.</span></span>    |
|<span data-ttu-id="80c40-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80c40-115">Application</span></span> | <span data-ttu-id="80c40-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80c40-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80c40-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80c40-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80c40-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80c40-118">Optional query parameters</span></span>
<span data-ttu-id="80c40-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80c40-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80c40-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80c40-120">Request headers</span></span>
| <span data-ttu-id="80c40-121">名称</span><span class="sxs-lookup"><span data-stu-id="80c40-121">Name</span></span>      |<span data-ttu-id="80c40-122">说明</span><span class="sxs-lookup"><span data-stu-id="80c40-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80c40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80c40-123">Authorization</span></span>  | <span data-ttu-id="80c40-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80c40-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80c40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="80c40-126">Request body</span></span>
<span data-ttu-id="80c40-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80c40-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80c40-128">响应</span><span class="sxs-lookup"><span data-stu-id="80c40-128">Response</span></span>

<span data-ttu-id="80c40-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="80c40-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="80c40-130">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="80c40-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="80c40-131">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="80c40-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="80c40-132">示例</span><span class="sxs-lookup"><span data-stu-id="80c40-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80c40-133">请求</span><span class="sxs-lookup"><span data-stu-id="80c40-133">Request</span></span>
<span data-ttu-id="80c40-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80c40-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="80c40-135">响应</span><span class="sxs-lookup"><span data-stu-id="80c40-135">Response</span></span>
<span data-ttu-id="80c40-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80c40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="80c40-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="80c40-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="80c40-140">语言</span><span class="sxs-lookup"><span data-stu-id="80c40-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80c40-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="80c40-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
