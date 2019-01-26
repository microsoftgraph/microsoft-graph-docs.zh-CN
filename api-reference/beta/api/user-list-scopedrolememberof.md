---
title: 列出 scopedAdministratorOf
description: 检索用户的 scopedRoleMembership 的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: af5d74161aff083e6d1bc70ad8efa7866d4cc02c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577331"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="54868-103">列出 scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="54868-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54868-104">检索[scopedRoleMembership](../resources/scopedrolemembership.md)用户的列表。</span><span class="sxs-lookup"><span data-stu-id="54868-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="54868-105">权限</span><span class="sxs-lookup"><span data-stu-id="54868-105">Permissions</span></span>
<span data-ttu-id="54868-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54868-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="54868-108">Permission type</span></span>      | <span data-ttu-id="54868-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54868-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54868-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54868-110">Delegated (work or school account)</span></span> | <span data-ttu-id="54868-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54868-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54868-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54868-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54868-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="54868-113">Not supported.</span></span>    |
|<span data-ttu-id="54868-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="54868-114">Application</span></span> | <span data-ttu-id="54868-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54868-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54868-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54868-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="54868-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54868-117">Optional query parameters</span></span>
<span data-ttu-id="54868-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54868-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54868-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54868-119">Request headers</span></span>
| <span data-ttu-id="54868-120">标头</span><span class="sxs-lookup"><span data-stu-id="54868-120">Header</span></span>       | <span data-ttu-id="54868-121">值</span><span class="sxs-lookup"><span data-stu-id="54868-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54868-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54868-122">Authorization</span></span>  | <span data-ttu-id="54868-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54868-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54868-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="54868-125">Request body</span></span>
<span data-ttu-id="54868-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54868-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54868-127">响应</span><span class="sxs-lookup"><span data-stu-id="54868-127">Response</span></span>

<span data-ttu-id="54868-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[scopedRoleMembership](../resources/scopedrolemembership.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="54868-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54868-129">示例</span><span class="sxs-lookup"><span data-stu-id="54868-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54868-130">请求</span><span class="sxs-lookup"><span data-stu-id="54868-130">Request</span></span>
<span data-ttu-id="54868-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54868-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
##### <a name="response"></a><span data-ttu-id="54868-132">响应</span><span class="sxs-lookup"><span data-stu-id="54868-132">Response</span></span>
<span data-ttu-id="54868-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54868-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
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
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-scopedrolememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
