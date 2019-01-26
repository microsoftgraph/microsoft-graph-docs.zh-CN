---
title: 列表 scopedRoleMembers
description: 检索 scopedRoleMembership 资源的列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06ed1a4f06b3d348e81039b5701f5adff9e3b85b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576134"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="331f0-103">列表 scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="331f0-103">List scopedRoleMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="331f0-104">检索[scopedRoleMembership](../resources/scopedrolemembership.md)资源的列表。</span><span class="sxs-lookup"><span data-stu-id="331f0-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="331f0-105">权限</span><span class="sxs-lookup"><span data-stu-id="331f0-105">Permissions</span></span>
<span data-ttu-id="331f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="331f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="331f0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="331f0-108">Permission type</span></span>      | <span data-ttu-id="331f0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="331f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="331f0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="331f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="331f0-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="331f0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="331f0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="331f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="331f0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="331f0-113">Not supported.</span></span>    |
|<span data-ttu-id="331f0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="331f0-114">Application</span></span> | <span data-ttu-id="331f0-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="331f0-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="331f0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="331f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="331f0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="331f0-117">Optional query parameters</span></span>
<span data-ttu-id="331f0-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="331f0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="331f0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="331f0-119">Request headers</span></span>
| <span data-ttu-id="331f0-120">名称</span><span class="sxs-lookup"><span data-stu-id="331f0-120">Name</span></span>      |<span data-ttu-id="331f0-121">说明</span><span class="sxs-lookup"><span data-stu-id="331f0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="331f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="331f0-122">Authorization</span></span>  | <span data-ttu-id="331f0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="331f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="331f0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="331f0-125">Request body</span></span>
<span data-ttu-id="331f0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="331f0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="331f0-127">响应</span><span class="sxs-lookup"><span data-stu-id="331f0-127">Response</span></span>

<span data-ttu-id="331f0-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[scopedRoleMembership](../resources/scopedrolemembership.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="331f0-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="331f0-129">示例</span><span class="sxs-lookup"><span data-stu-id="331f0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="331f0-130">请求</span><span class="sxs-lookup"><span data-stu-id="331f0-130">Request</span></span>
<span data-ttu-id="331f0-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="331f0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
##### <a name="response"></a><span data-ttu-id="331f0-132">响应</span><span class="sxs-lookup"><span data-stu-id="331f0-132">Response</span></span>
<span data-ttu-id="331f0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="331f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-list-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
