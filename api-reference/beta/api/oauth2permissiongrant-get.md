---
title: 获取 oAuth2Permissiongrant
description: 检索的属性和 oAuth2Permissiongrant 对象的关系。
localization_priority: Normal
ms.openlocfilehash: 2b389e7f811444b9dc9fb1d9c2f619006611e11e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640537"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="0f292-103">获取 oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="0f292-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f292-104">检索的属性和 oAuth2Permissiongrant 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0f292-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f292-105">权限</span><span class="sxs-lookup"><span data-stu-id="0f292-105">Permissions</span></span>
<span data-ttu-id="0f292-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0f292-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f292-108">Permission type</span></span>      | <span data-ttu-id="0f292-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f292-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f292-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f292-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f292-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0f292-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0f292-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f292-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f292-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f292-113">Not supported.</span></span>    |
|<span data-ttu-id="0f292-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f292-114">Application</span></span> | <span data-ttu-id="0f292-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f292-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f292-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f292-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0f292-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0f292-117">Optional query parameters</span></span>
<span data-ttu-id="0f292-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0f292-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f292-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f292-119">Request headers</span></span>
| <span data-ttu-id="0f292-120">名称</span><span class="sxs-lookup"><span data-stu-id="0f292-120">Name</span></span>       | <span data-ttu-id="0f292-121">类型</span><span class="sxs-lookup"><span data-stu-id="0f292-121">Type</span></span> | <span data-ttu-id="0f292-122">说明</span><span class="sxs-lookup"><span data-stu-id="0f292-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f292-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f292-123">Authorization</span></span>  | <span data-ttu-id="0f292-124">string</span><span class="sxs-lookup"><span data-stu-id="0f292-124">string</span></span>  | <span data-ttu-id="0f292-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f292-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f292-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f292-127">Request body</span></span>
<span data-ttu-id="0f292-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f292-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f292-129">响应</span><span class="sxs-lookup"><span data-stu-id="0f292-129">Response</span></span>

<span data-ttu-id="0f292-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f292-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f292-131">示例</span><span class="sxs-lookup"><span data-stu-id="0f292-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f292-132">请求</span><span class="sxs-lookup"><span data-stu-id="0f292-132">Request</span></span>
<span data-ttu-id="0f292-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f292-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="0f292-134">响应</span><span class="sxs-lookup"><span data-stu-id="0f292-134">Response</span></span>
<span data-ttu-id="0f292-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f292-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
