---
title: 列表 servicePrincipals
description: 检索 servicePrincipal 对象的列表。
localization_priority: Normal
ms.openlocfilehash: cd61b69e330ac376d15bfaf99c1147b8f9402d7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526086"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="b3f83-103">列表 servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="b3f83-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3f83-104">检索 servicePrincipal 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b3f83-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3f83-105">权限</span><span class="sxs-lookup"><span data-stu-id="b3f83-105">Permissions</span></span>

<span data-ttu-id="b3f83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b3f83-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3f83-108">Permission type</span></span>      | <span data-ttu-id="b3f83-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3f83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3f83-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3f83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3f83-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3f83-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3f83-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3f83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3f83-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3f83-113">Not supported.</span></span>    |
|<span data-ttu-id="b3f83-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3f83-114">Application</span></span> | <span data-ttu-id="b3f83-115">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3f83-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3f83-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3f83-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3f83-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3f83-117">Optional query parameters</span></span>

<span data-ttu-id="b3f83-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b3f83-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3f83-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3f83-119">Request headers</span></span>
| <span data-ttu-id="b3f83-120">名称</span><span class="sxs-lookup"><span data-stu-id="b3f83-120">Name</span></span> | <span data-ttu-id="b3f83-121">说明</span><span class="sxs-lookup"><span data-stu-id="b3f83-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b3f83-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3f83-122">Authorization</span></span>  | <span data-ttu-id="b3f83-123">string</span><span class="sxs-lookup"><span data-stu-id="b3f83-123">string</span></span>  | <span data-ttu-id="b3f83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3f83-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3f83-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3f83-126">Request body</span></span>

<span data-ttu-id="b3f83-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3f83-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3f83-128">响应</span><span class="sxs-lookup"><span data-stu-id="b3f83-128">Response</span></span>

<span data-ttu-id="b3f83-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[servicePrincipal](../resources/serviceprincipal.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b3f83-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3f83-130">示例</span><span class="sxs-lookup"><span data-stu-id="b3f83-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3f83-131">请求</span><span class="sxs-lookup"><span data-stu-id="b3f83-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="b3f83-132">响应</span><span class="sxs-lookup"><span data-stu-id="b3f83-132">Response</span></span>

<span data-ttu-id="b3f83-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3f83-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
