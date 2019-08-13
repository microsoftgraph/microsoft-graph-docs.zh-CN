---
title: List licenseDetails
description: 检索 licenseDetails 对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 947fb36ef77f2212491fcceb312960bfbc14306e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326077"
---
# <a name="list-licensedetails"></a><span data-ttu-id="3f584-103">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="3f584-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f584-104">检索 licenseDetails 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3f584-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f584-105">权限</span><span class="sxs-lookup"><span data-stu-id="3f584-105">Permissions</span></span>
<span data-ttu-id="3f584-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f584-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f584-108">Permission type</span></span>      | <span data-ttu-id="3f584-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f584-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f584-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f584-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f584-111">User. read, User. all, All, all, Directory.accessasuser.all, all, all, all, all。 All</span><span class="sxs-lookup"><span data-stu-id="3f584-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f584-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f584-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f584-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="3f584-113">User.Read</span></span>    |
|<span data-ttu-id="3f584-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f584-114">Application</span></span> | <span data-ttu-id="3f584-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f584-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f584-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f584-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f584-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3f584-117">Optional query parameters</span></span>
<span data-ttu-id="3f584-118">此方法**不**支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="3f584-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f584-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f584-119">Request headers</span></span>
| <span data-ttu-id="3f584-120">名称</span><span class="sxs-lookup"><span data-stu-id="3f584-120">Name</span></span>      |<span data-ttu-id="3f584-121">说明</span><span class="sxs-lookup"><span data-stu-id="3f584-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f584-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f584-122">Authorization</span></span>  | <span data-ttu-id="3f584-123">持有&lt;者代码&gt;</span><span class="sxs-lookup"><span data-stu-id="3f584-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f584-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f584-124">Request body</span></span>
<span data-ttu-id="3f584-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f584-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f584-126">响应</span><span class="sxs-lookup"><span data-stu-id="3f584-126">Response</span></span>

<span data-ttu-id="3f584-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[licenseDetails](../resources/licensedetails.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3f584-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f584-128">示例</span><span class="sxs-lookup"><span data-stu-id="3f584-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f584-129">请求</span><span class="sxs-lookup"><span data-stu-id="3f584-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3f584-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3f584-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f584-131">C#</span><span class="sxs-lookup"><span data-stu-id="3f584-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f584-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f584-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f584-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="3f584-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3f584-134">Java</span><span class="sxs-lookup"><span data-stu-id="3f584-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3f584-135">响应</span><span class="sxs-lookup"><span data-stu-id="3f584-135">Response</span></span>
<span data-ttu-id="3f584-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f584-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
