---
title: 列出 licenseDetails
description: 检索 licenseDetails 对象列表。
ms.openlocfilehash: aefcc158721a83b53bdb4557c6dc7a1b47bc6bfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048029"
---
# <a name="list-licensedetails"></a><span data-ttu-id="d4f61-103">列出 licenseDetails</span><span class="sxs-lookup"><span data-stu-id="d4f61-103">List licenseDetails</span></span>

> <span data-ttu-id="d4f61-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4f61-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4f61-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4f61-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4f61-106">检索 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d4f61-106">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4f61-107">权限</span><span class="sxs-lookup"><span data-stu-id="d4f61-107">Permissions</span></span>
<span data-ttu-id="d4f61-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4f61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4f61-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4f61-110">Permission type</span></span>      | <span data-ttu-id="d4f61-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4f61-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4f61-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4f61-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d4f61-113">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4f61-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4f61-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4f61-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4f61-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="d4f61-115">User.Read</span></span>    |
|<span data-ttu-id="d4f61-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4f61-116">Application</span></span> | <span data-ttu-id="d4f61-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4f61-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4f61-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4f61-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4f61-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4f61-119">Optional query parameters</span></span>
<span data-ttu-id="d4f61-120">该方法**不**支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="d4f61-120">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4f61-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4f61-121">Request headers</span></span>
| <span data-ttu-id="d4f61-122">名称</span><span class="sxs-lookup"><span data-stu-id="d4f61-122">Name</span></span>      |<span data-ttu-id="d4f61-123">说明</span><span class="sxs-lookup"><span data-stu-id="d4f61-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4f61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4f61-124">Authorization</span></span>  | <span data-ttu-id="d4f61-125">持有者&lt;代码&gt;</span><span class="sxs-lookup"><span data-stu-id="d4f61-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4f61-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4f61-126">Request body</span></span>
<span data-ttu-id="d4f61-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4f61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4f61-128">响应</span><span class="sxs-lookup"><span data-stu-id="d4f61-128">Response</span></span>

<span data-ttu-id="d4f61-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [licenseDetails](../resources/licensedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d4f61-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4f61-130">示例</span><span class="sxs-lookup"><span data-stu-id="d4f61-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4f61-131">请求</span><span class="sxs-lookup"><span data-stu-id="d4f61-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="d4f61-132">响应</span><span class="sxs-lookup"><span data-stu-id="d4f61-132">Response</span></span>
<span data-ttu-id="d4f61-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4f61-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->