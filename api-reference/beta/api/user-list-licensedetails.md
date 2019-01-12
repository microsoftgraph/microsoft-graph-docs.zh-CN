---
title: 列出 licenseDetails
description: 检索 licenseDetails 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80b2e707ec6106def7d8539dcf5e8e9a20179503
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991893"
---
# <a name="list-licensedetails"></a><span data-ttu-id="ae58e-103">列出 licenseDetails</span><span class="sxs-lookup"><span data-stu-id="ae58e-103">List licenseDetails</span></span>

> <span data-ttu-id="ae58e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae58e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae58e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae58e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae58e-106">检索 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ae58e-106">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae58e-107">权限</span><span class="sxs-lookup"><span data-stu-id="ae58e-107">Permissions</span></span>
<span data-ttu-id="ae58e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae58e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae58e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae58e-110">Permission type</span></span>      | <span data-ttu-id="ae58e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae58e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae58e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae58e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae58e-113">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae58e-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae58e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae58e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae58e-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="ae58e-115">User.Read</span></span>    |
|<span data-ttu-id="ae58e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae58e-116">Application</span></span> | <span data-ttu-id="ae58e-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae58e-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae58e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae58e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae58e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae58e-119">Optional query parameters</span></span>
<span data-ttu-id="ae58e-120">该方法**不**支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="ae58e-120">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae58e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae58e-121">Request headers</span></span>
| <span data-ttu-id="ae58e-122">名称</span><span class="sxs-lookup"><span data-stu-id="ae58e-122">Name</span></span>      |<span data-ttu-id="ae58e-123">说明</span><span class="sxs-lookup"><span data-stu-id="ae58e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae58e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae58e-124">Authorization</span></span>  | <span data-ttu-id="ae58e-125">持有者&lt;代码&gt;</span><span class="sxs-lookup"><span data-stu-id="ae58e-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae58e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae58e-126">Request body</span></span>
<span data-ttu-id="ae58e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae58e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae58e-128">响应</span><span class="sxs-lookup"><span data-stu-id="ae58e-128">Response</span></span>

<span data-ttu-id="ae58e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [licenseDetails](../resources/licensedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ae58e-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae58e-130">示例</span><span class="sxs-lookup"><span data-stu-id="ae58e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae58e-131">请求</span><span class="sxs-lookup"><span data-stu-id="ae58e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="ae58e-132">响应</span><span class="sxs-lookup"><span data-stu-id="ae58e-132">Response</span></span>
<span data-ttu-id="ae58e-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae58e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
