---
title: 列表 oauth2PermissionGrants
description: 检索 oauth2PermissionGrant 对象的列表。
localization_priority: Normal
ms.openlocfilehash: f75ae0922b8c02ab3b290b471db2e649a000fbcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813781"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="c07ee-103">列表 oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="c07ee-103">List oauth2PermissionGrants</span></span>

> <span data-ttu-id="c07ee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c07ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c07ee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c07ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c07ee-106">检索 oauth2PermissionGrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c07ee-106">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c07ee-107">权限</span><span class="sxs-lookup"><span data-stu-id="c07ee-107">Permissions</span></span>

<span data-ttu-id="c07ee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c07ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c07ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c07ee-110">Permission type</span></span>      | <span data-ttu-id="c07ee-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c07ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c07ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c07ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c07ee-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c07ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c07ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c07ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c07ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c07ee-115">Not supported.</span></span>    |
|<span data-ttu-id="c07ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c07ee-116">Application</span></span> | <span data-ttu-id="c07ee-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07ee-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c07ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c07ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c07ee-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c07ee-119">Optional query parameters</span></span>
<span data-ttu-id="c07ee-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c07ee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c07ee-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c07ee-121">Request headers</span></span>
| <span data-ttu-id="c07ee-122">名称</span><span class="sxs-lookup"><span data-stu-id="c07ee-122">Name</span></span> | <span data-ttu-id="c07ee-123">说明</span><span class="sxs-lookup"><span data-stu-id="c07ee-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="c07ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c07ee-124">Authorization</span></span>  | <span data-ttu-id="c07ee-125">string</span><span class="sxs-lookup"><span data-stu-id="c07ee-125">string</span></span>  | <span data-ttu-id="c07ee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c07ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c07ee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c07ee-128">Request body</span></span>
<span data-ttu-id="c07ee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c07ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c07ee-130">响应</span><span class="sxs-lookup"><span data-stu-id="c07ee-130">Response</span></span>

<span data-ttu-id="c07ee-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c07ee-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c07ee-132">示例</span><span class="sxs-lookup"><span data-stu-id="c07ee-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c07ee-133">请求</span><span class="sxs-lookup"><span data-stu-id="c07ee-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="c07ee-134">响应</span><span class="sxs-lookup"><span data-stu-id="c07ee-134">Response</span></span>

<span data-ttu-id="c07ee-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c07ee-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
