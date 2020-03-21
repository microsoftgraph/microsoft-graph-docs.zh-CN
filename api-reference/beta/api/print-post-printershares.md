---
title: 创建 printerShare
description: 为指定的打印机创建新的打印机共享。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f4a1263f9deffe35eed89b7d7840038948ce409d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895714"
---
# <a name="create-printershare"></a><span data-ttu-id="858d9-103">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="858d9-103">Create printerShare</span></span>

<span data-ttu-id="858d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="858d9-105">为指定的[打印机](../resources/printer.md)创建新的**printerShare** 。</span><span class="sxs-lookup"><span data-stu-id="858d9-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="858d9-106">权限</span><span class="sxs-lookup"><span data-stu-id="858d9-106">Permissions</span></span>
<span data-ttu-id="858d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="858d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="858d9-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="858d9-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="858d9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="858d9-110">Permission type</span></span> | <span data-ttu-id="858d9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="858d9-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="858d9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="858d9-112">Delegated (work or school account)</span></span>| <span data-ttu-id="858d9-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="858d9-113">Users.Read.All</span></span> |
|<span data-ttu-id="858d9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="858d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="858d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="858d9-115">Not Supported.</span></span>|
|<span data-ttu-id="858d9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="858d9-116">Application</span></span>|<span data-ttu-id="858d9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="858d9-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="858d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="858d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares
```
## <a name="request-headers"></a><span data-ttu-id="858d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="858d9-119">Request headers</span></span>
| <span data-ttu-id="858d9-120">名称</span><span class="sxs-lookup"><span data-stu-id="858d9-120">Name</span></span>          | <span data-ttu-id="858d9-121">说明</span><span class="sxs-lookup"><span data-stu-id="858d9-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="858d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="858d9-122">Authorization</span></span> | <span data-ttu-id="858d9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="858d9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="858d9-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="858d9-125">Content-type</span></span>  | <span data-ttu-id="858d9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="858d9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="858d9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="858d9-128">Request body</span></span>
<span data-ttu-id="858d9-129">在请求正文中，提供[printerShare](../resources/printershare.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="858d9-129">In the request body, supply a JSON representation of [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="858d9-130">打印机共享的**id**和**createdDateTime**属性是在创建资源时自动设置的，但共享名称和关联的打印机必须包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="858d9-130">The printer share's **id** and **createdDateTime** properties are set automatically upon resource creation, but the share name and associated printer must be included in the request.</span></span>

<span data-ttu-id="858d9-131">打印机引用是使用`@odata.bind`语法设置的，如示例中所示。</span><span class="sxs-lookup"><span data-stu-id="858d9-131">The printer reference is set by using `@odata.bind` syntax, as shown in the example.</span></span>

## <a name="response"></a><span data-ttu-id="858d9-132">响应</span><span class="sxs-lookup"><span data-stu-id="858d9-132">Response</span></span>
<span data-ttu-id="858d9-133">如果成功，此方法在响应`201 Created`正文中返回响应代码和[printerShare](../resources/printershare.md)对象。</span><span class="sxs-lookup"><span data-stu-id="858d9-133">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="858d9-134">示例</span><span class="sxs-lookup"><span data-stu-id="858d9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="858d9-135">请求</span><span class="sxs-lookup"><span data-stu-id="858d9-135">Request</span></span>
<span data-ttu-id="858d9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="858d9-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
##### <a name="response"></a><span data-ttu-id="858d9-137">响应</span><span class="sxs-lookup"><span data-stu-id="858d9-137">Response</span></span>
<span data-ttu-id="858d9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="858d9-138">The following is an example of the response.</span></span>
><span data-ttu-id="858d9-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="858d9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "name": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->