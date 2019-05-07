---
title: 'servicePrincipal: List oAuth2Permissiongrants'
description: 检索 oAuth2Permissiongrant 对象的列表。
localization_priority: Normal
ms.openlocfilehash: 104d197d843acfb1ac7c20330dd4c7e3af58ee60
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638786"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="c0d66-103">servicePrincipal: List oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="c0d66-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d66-104">检索 oAuth2Permissiongrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c0d66-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d66-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0d66-105">Permissions</span></span>
<span data-ttu-id="c0d66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0d66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d66-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0d66-108">Permission type</span></span>      | <span data-ttu-id="c0d66-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0d66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0d66-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0d66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0d66-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0d66-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0d66-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0d66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d66-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0d66-113">Not supported.</span></span>    |
|<span data-ttu-id="c0d66-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0d66-114">Application</span></span> | <span data-ttu-id="c0d66-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d66-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0d66-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0d66-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0d66-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0d66-117">Optional query parameters</span></span>
<span data-ttu-id="c0d66-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0d66-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0d66-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0d66-119">Request headers</span></span>
| <span data-ttu-id="c0d66-120">名称</span><span class="sxs-lookup"><span data-stu-id="c0d66-120">Name</span></span>       | <span data-ttu-id="c0d66-121">类型</span><span class="sxs-lookup"><span data-stu-id="c0d66-121">Type</span></span> | <span data-ttu-id="c0d66-122">说明</span><span class="sxs-lookup"><span data-stu-id="c0d66-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0d66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0d66-123">Authorization</span></span>  | <span data-ttu-id="c0d66-124">string</span><span class="sxs-lookup"><span data-stu-id="c0d66-124">string</span></span>  | <span data-ttu-id="c0d66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0d66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0d66-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0d66-127">Request body</span></span>
<span data-ttu-id="c0d66-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0d66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0d66-129">响应</span><span class="sxs-lookup"><span data-stu-id="c0d66-129">Response</span></span>

<span data-ttu-id="c0d66-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0d66-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0d66-131">示例</span><span class="sxs-lookup"><span data-stu-id="c0d66-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0d66-132">请求</span><span class="sxs-lookup"><span data-stu-id="c0d66-132">Request</span></span>
<span data-ttu-id="c0d66-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0d66-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
##### <a name="response"></a><span data-ttu-id="c0d66-134">响应</span><span class="sxs-lookup"><span data-stu-id="c0d66-134">Response</span></span>
<span data-ttu-id="c0d66-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0d66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c0d66-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c0d66-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c0d66-139">语言</span><span class="sxs-lookup"><span data-stu-id="c0d66-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d66-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d66-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
