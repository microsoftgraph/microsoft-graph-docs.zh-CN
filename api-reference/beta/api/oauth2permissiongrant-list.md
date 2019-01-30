---
title: List oauth2PermissionGrants
description: 检索 oauth2PermissionGrant 对象的列表。
localization_priority: Normal
ms.openlocfilehash: 9af84b4af64466658058259a665d426484511526
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643253"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="baea8-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="baea8-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baea8-104">检索 oauth2PermissionGrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="baea8-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="baea8-105">权限</span><span class="sxs-lookup"><span data-stu-id="baea8-105">Permissions</span></span>

<span data-ttu-id="baea8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="baea8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="baea8-108">Permission type</span></span>      | <span data-ttu-id="baea8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baea8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baea8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baea8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="baea8-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="baea8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="baea8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baea8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baea8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="baea8-113">Not supported.</span></span>    |
|<span data-ttu-id="baea8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="baea8-114">Application</span></span> | <span data-ttu-id="baea8-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baea8-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="baea8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baea8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="baea8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="baea8-117">Optional query parameters</span></span>
<span data-ttu-id="baea8-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="baea8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="baea8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="baea8-119">Request headers</span></span>
| <span data-ttu-id="baea8-120">名称</span><span class="sxs-lookup"><span data-stu-id="baea8-120">Name</span></span> | <span data-ttu-id="baea8-121">说明</span><span class="sxs-lookup"><span data-stu-id="baea8-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="baea8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="baea8-122">Authorization</span></span>  | <span data-ttu-id="baea8-123">string</span><span class="sxs-lookup"><span data-stu-id="baea8-123">string</span></span>  | <span data-ttu-id="baea8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="baea8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baea8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="baea8-126">Request body</span></span>
<span data-ttu-id="baea8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="baea8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baea8-128">响应</span><span class="sxs-lookup"><span data-stu-id="baea8-128">Response</span></span>

<span data-ttu-id="baea8-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="baea8-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="baea8-130">示例</span><span class="sxs-lookup"><span data-stu-id="baea8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="baea8-131">请求</span><span class="sxs-lookup"><span data-stu-id="baea8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="baea8-132">响应</span><span class="sxs-lookup"><span data-stu-id="baea8-132">Response</span></span>

<span data-ttu-id="baea8-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="baea8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
