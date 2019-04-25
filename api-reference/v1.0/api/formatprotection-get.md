---
title: 获取 FormatProtection
description: 检索 formatprotection 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: dd6d4ef53555d2c6eb8c9232d7a08ea7579e20e3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524139"
---
# <a name="get-formatprotection"></a><span data-ttu-id="bc1e5-103">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="bc1e5-103">Get FormatProtection</span></span>

<span data-ttu-id="bc1e5-104">检索 formatprotection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-104">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc1e5-105">权限</span><span class="sxs-lookup"><span data-stu-id="bc1e5-105">Permissions</span></span>
<span data-ttu-id="bc1e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc1e5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc1e5-108">Permission type</span></span>      | <span data-ttu-id="bc1e5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc1e5-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bc1e5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc1e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc1e5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc1e5-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="bc1e5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc1e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc1e5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-113">Not supported.</span></span>    | 
|<span data-ttu-id="bc1e5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc1e5-114">Application</span></span> | <span data-ttu-id="bc1e5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bc1e5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc1e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc1e5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc1e5-117">Optional query parameters</span></span>
<span data-ttu-id="bc1e5-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc1e5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc1e5-119">Request headers</span></span>
| <span data-ttu-id="bc1e5-120">名称</span><span class="sxs-lookup"><span data-stu-id="bc1e5-120">Name</span></span>      |<span data-ttu-id="bc1e5-121">说明</span><span class="sxs-lookup"><span data-stu-id="bc1e5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc1e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc1e5-122">Authorization</span></span>  | <span data-ttu-id="bc1e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bc1e5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc1e5-125">Request body</span></span>
<span data-ttu-id="bc1e5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc1e5-127">响应</span><span class="sxs-lookup"><span data-stu-id="bc1e5-127">Response</span></span>

<span data-ttu-id="bc1e5-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-128">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc1e5-129">示例</span><span class="sxs-lookup"><span data-stu-id="bc1e5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc1e5-130">请求</span><span class="sxs-lookup"><span data-stu-id="bc1e5-130">Request</span></span>
<span data-ttu-id="bc1e5-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="bc1e5-132">响应</span><span class="sxs-lookup"><span data-stu-id="bc1e5-132">Response</span></span>
<span data-ttu-id="bc1e5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc1e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
