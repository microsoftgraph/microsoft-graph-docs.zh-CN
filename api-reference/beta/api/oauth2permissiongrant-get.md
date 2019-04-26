---
title: 获取 oAuth2Permissiongrant
description: 检索 oAuth2Permissiongrant 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 482d1f310b6eadcfe7df9e961af4ee4c229e9c12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338214"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="4c656-103">获取 oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="4c656-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c656-104">检索 oAuth2Permissiongrant 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c656-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c656-105">权限</span><span class="sxs-lookup"><span data-stu-id="4c656-105">Permissions</span></span>
<span data-ttu-id="4c656-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4c656-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c656-108">Permission type</span></span>      | <span data-ttu-id="4c656-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c656-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c656-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c656-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c656-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c656-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c656-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c656-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c656-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c656-113">Not supported.</span></span>    |
|<span data-ttu-id="4c656-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c656-114">Application</span></span> | <span data-ttu-id="4c656-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c656-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c656-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c656-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c656-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4c656-117">Optional query parameters</span></span>
<span data-ttu-id="4c656-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4c656-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c656-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c656-119">Request headers</span></span>
| <span data-ttu-id="4c656-120">名称</span><span class="sxs-lookup"><span data-stu-id="4c656-120">Name</span></span>       | <span data-ttu-id="4c656-121">类型</span><span class="sxs-lookup"><span data-stu-id="4c656-121">Type</span></span> | <span data-ttu-id="4c656-122">说明</span><span class="sxs-lookup"><span data-stu-id="4c656-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c656-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c656-123">Authorization</span></span>  | <span data-ttu-id="4c656-124">string</span><span class="sxs-lookup"><span data-stu-id="4c656-124">string</span></span>  | <span data-ttu-id="4c656-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c656-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c656-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c656-127">Request body</span></span>
<span data-ttu-id="4c656-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c656-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c656-129">响应</span><span class="sxs-lookup"><span data-stu-id="4c656-129">Response</span></span>

<span data-ttu-id="4c656-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4c656-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c656-131">示例</span><span class="sxs-lookup"><span data-stu-id="4c656-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c656-132">请求</span><span class="sxs-lookup"><span data-stu-id="4c656-132">Request</span></span>
<span data-ttu-id="4c656-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c656-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="4c656-134">响应</span><span class="sxs-lookup"><span data-stu-id="4c656-134">Response</span></span>
<span data-ttu-id="4c656-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c656-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
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
  "suppressions": []
}
-->
