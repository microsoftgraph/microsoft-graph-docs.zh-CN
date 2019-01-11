---
title: 获取 privilegedRoleSummary
description: 检索的属性和 privilegedRoleSummary 对象的关系。
localization_priority: Normal
ms.openlocfilehash: ebe3a0774869c09ba26cd01726590a6b7cddb58f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816077"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="895ad-103">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="895ad-103">Get privilegedRoleSummary</span></span>

> <span data-ttu-id="895ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="895ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="895ad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="895ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="895ad-106">检索的属性和[privilegedRoleSummary](../resources/privilegedrolesummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="895ad-106">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="895ad-107">权限</span><span class="sxs-lookup"><span data-stu-id="895ad-107">Permissions</span></span>
<span data-ttu-id="895ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="895ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="895ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="895ad-110">Permission type</span></span>      | <span data-ttu-id="895ad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="895ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="895ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="895ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="895ad-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="895ad-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="895ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="895ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="895ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="895ad-115">Not supported.</span></span>    |
|<span data-ttu-id="895ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="895ad-116">Application</span></span> | <span data-ttu-id="895ad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="895ad-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="895ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="895ad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="895ad-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="895ad-119">Optional query parameters</span></span>
<span data-ttu-id="895ad-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="895ad-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="895ad-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="895ad-121">Request headers</span></span>
| <span data-ttu-id="895ad-122">名称</span><span class="sxs-lookup"><span data-stu-id="895ad-122">Name</span></span>      |<span data-ttu-id="895ad-123">说明</span><span class="sxs-lookup"><span data-stu-id="895ad-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="895ad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="895ad-124">Authorization</span></span>  | <span data-ttu-id="895ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="895ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="895ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="895ad-127">Request body</span></span>
<span data-ttu-id="895ad-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="895ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="895ad-129">响应</span><span class="sxs-lookup"><span data-stu-id="895ad-129">Response</span></span>

<span data-ttu-id="895ad-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleSummary](../resources/privilegedrolesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="895ad-130">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="895ad-131">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="895ad-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="895ad-132">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="895ad-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="895ad-133">示例</span><span class="sxs-lookup"><span data-stu-id="895ad-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="895ad-134">请求</span><span class="sxs-lookup"><span data-stu-id="895ad-134">Request</span></span>
<span data-ttu-id="895ad-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="895ad-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="895ad-136">响应</span><span class="sxs-lookup"><span data-stu-id="895ad-136">Response</span></span>
<span data-ttu-id="895ad-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="895ad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
