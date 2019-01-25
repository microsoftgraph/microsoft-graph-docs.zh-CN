---
title: 列出 licenseDetails
description: 检索 licenseDetails 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7dae02120f17dfbd329758734ba5fb912adfe0e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515942"
---
# <a name="list-licensedetails"></a><span data-ttu-id="e12d6-103">列出 licenseDetails</span><span class="sxs-lookup"><span data-stu-id="e12d6-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e12d6-104">检索 licenseDetails 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e12d6-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e12d6-105">权限</span><span class="sxs-lookup"><span data-stu-id="e12d6-105">Permissions</span></span>
<span data-ttu-id="e12d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e12d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e12d6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e12d6-108">Permission type</span></span>      | <span data-ttu-id="e12d6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e12d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e12d6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e12d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e12d6-111">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e12d6-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e12d6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e12d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e12d6-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="e12d6-113">User.Read</span></span>    |
|<span data-ttu-id="e12d6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e12d6-114">Application</span></span> | <span data-ttu-id="e12d6-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e12d6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e12d6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e12d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e12d6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e12d6-117">Optional query parameters</span></span>
<span data-ttu-id="e12d6-118">该方法**不**支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="e12d6-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e12d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e12d6-119">Request headers</span></span>
| <span data-ttu-id="e12d6-120">名称</span><span class="sxs-lookup"><span data-stu-id="e12d6-120">Name</span></span>      |<span data-ttu-id="e12d6-121">说明</span><span class="sxs-lookup"><span data-stu-id="e12d6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e12d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e12d6-122">Authorization</span></span>  | <span data-ttu-id="e12d6-123">持有者&lt;代码&gt;</span><span class="sxs-lookup"><span data-stu-id="e12d6-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="e12d6-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e12d6-124">Request body</span></span>
<span data-ttu-id="e12d6-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e12d6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e12d6-126">响应</span><span class="sxs-lookup"><span data-stu-id="e12d6-126">Response</span></span>

<span data-ttu-id="e12d6-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [licenseDetails](../resources/licensedetails.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e12d6-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e12d6-128">示例</span><span class="sxs-lookup"><span data-stu-id="e12d6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e12d6-129">请求</span><span class="sxs-lookup"><span data-stu-id="e12d6-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="e12d6-130">响应</span><span class="sxs-lookup"><span data-stu-id="e12d6-130">Response</span></span>
<span data-ttu-id="e12d6-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e12d6-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
