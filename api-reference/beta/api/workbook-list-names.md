---
title: 列出名称
description: 检索 nameditem 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: da13ae0734c5508c1eb2db2bb5874a52957c27db
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536451"
---
# <a name="list-names"></a><span data-ttu-id="ae433-103">列出名称</span><span class="sxs-lookup"><span data-stu-id="ae433-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae433-104">检索 nameditem 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ae433-104">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae433-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae433-105">Permissions</span></span>
<span data-ttu-id="ae433-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae433-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae433-108">Permission type</span></span>      | <span data-ttu-id="ae433-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae433-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae433-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae433-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae433-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae433-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae433-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae433-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae433-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae433-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae433-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae433-114">Application</span></span> | <span data-ttu-id="ae433-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae433-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae433-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae433-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae433-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae433-117">Optional query parameters</span></span>
<span data-ttu-id="ae433-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae433-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae433-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae433-119">Request headers</span></span>
| <span data-ttu-id="ae433-120">名称</span><span class="sxs-lookup"><span data-stu-id="ae433-120">Name</span></span>      |<span data-ttu-id="ae433-121">说明</span><span class="sxs-lookup"><span data-stu-id="ae433-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae433-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae433-122">Authorization</span></span>  | <span data-ttu-id="ae433-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae433-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae433-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae433-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae433-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ae433-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae433-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae433-128">Request body</span></span>
<span data-ttu-id="ae433-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae433-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae433-130">响应</span><span class="sxs-lookup"><span data-stu-id="ae433-130">Response</span></span>

<span data-ttu-id="ae433-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [NamedItem](../resources/nameditem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ae433-131">If successful, this method returns a `200 OK` response code and collection of [NamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae433-132">示例</span><span class="sxs-lookup"><span data-stu-id="ae433-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae433-133">请求</span><span class="sxs-lookup"><span data-stu-id="ae433-133">Request</span></span>
<span data-ttu-id="ae433-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae433-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names
```
##### <a name="response"></a><span data-ttu-id="ae433-135">响应</span><span class="sxs-lookup"><span data-stu-id="ae433-135">Response</span></span>
<span data-ttu-id="ae433-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae433-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "value": [
    {
      "name": "name-value",
      "type": "type-value",
      "value": {
      },
      "visible": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-list-names.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
