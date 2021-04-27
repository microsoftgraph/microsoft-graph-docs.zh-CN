---
title: 获取 printSettings
description: 检索通用打印服务的租户范围设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6cbe8c25276f05ce432b13dbeb33e6f570e99da1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037597"
---
# <a name="get-printsettings"></a><span data-ttu-id="e0d5c-103">获取 printSettings</span><span class="sxs-lookup"><span data-stu-id="e0d5c-103">Get printSettings</span></span>

<span data-ttu-id="e0d5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0d5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0d5c-105">检索通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0d5c-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0d5c-106">Permissions</span></span>
<span data-ttu-id="e0d5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e0d5c-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e0d5c-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e0d5c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0d5c-111">Permission type</span></span> | <span data-ttu-id="e0d5c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0d5c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e0d5c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0d5c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e0d5c-114">PrintSettings.Read.All、PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0d5c-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="e0d5c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0d5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0d5c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-116">Not Supported.</span></span>|
|<span data-ttu-id="e0d5c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0d5c-117">Application</span></span>|<span data-ttu-id="e0d5c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0d5c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0d5c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0d5c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0d5c-120">Optional query parameters</span></span>
<span data-ttu-id="e0d5c-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e0d5c-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0d5c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0d5c-123">Request headers</span></span>
| <span data-ttu-id="e0d5c-124">名称</span><span class="sxs-lookup"><span data-stu-id="e0d5c-124">Name</span></span>      |<span data-ttu-id="e0d5c-125">说明</span><span class="sxs-lookup"><span data-stu-id="e0d5c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0d5c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0d5c-126">Authorization</span></span> | <span data-ttu-id="e0d5c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0d5c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0d5c-129">Request body</span></span>
<span data-ttu-id="e0d5c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e0d5c-131">响应</span><span class="sxs-lookup"><span data-stu-id="e0d5c-131">Response</span></span>
<span data-ttu-id="e0d5c-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printSettings](../resources/printsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0d5c-133">示例</span><span class="sxs-lookup"><span data-stu-id="e0d5c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0d5c-134">请求</span><span class="sxs-lookup"><span data-stu-id="e0d5c-134">Request</span></span>
<span data-ttu-id="e0d5c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0d5c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0d5c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/settings
```
# <a name="c"></a>[<span data-ttu-id="e0d5c-137">C#</span><span class="sxs-lookup"><span data-stu-id="e0d5c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0d5c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0d5c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0d5c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0d5c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0d5c-140">Java</span><span class="sxs-lookup"><span data-stu-id="e0d5c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0d5c-141">响应</span><span class="sxs-lookup"><span data-stu-id="e0d5c-141">Response</span></span>
<span data-ttu-id="e0d5c-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-142">The following is an example of the response.</span></span>
><span data-ttu-id="e0d5c-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0d5c-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
