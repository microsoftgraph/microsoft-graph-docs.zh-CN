---
title: 获取 privilegedRoleSummary
description: 检索 privilegedRoleSummary 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 9065cb240b9807822d703c8f5fdf0f7e18dea71f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331982"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="ae95c-103">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="ae95c-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae95c-104">检索[privilegedRoleSummary](../resources/privilegedrolesummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae95c-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae95c-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae95c-105">Permissions</span></span>
<span data-ttu-id="ae95c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae95c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae95c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae95c-108">Permission type</span></span>      | <span data-ttu-id="ae95c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae95c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae95c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae95c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae95c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae95c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae95c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae95c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae95c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae95c-113">Not supported.</span></span>    |
|<span data-ttu-id="ae95c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae95c-114">Application</span></span> | <span data-ttu-id="ae95c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae95c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae95c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae95c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae95c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae95c-117">Optional query parameters</span></span>
<span data-ttu-id="ae95c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae95c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae95c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae95c-119">Request headers</span></span>
| <span data-ttu-id="ae95c-120">名称</span><span class="sxs-lookup"><span data-stu-id="ae95c-120">Name</span></span>      |<span data-ttu-id="ae95c-121">说明</span><span class="sxs-lookup"><span data-stu-id="ae95c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae95c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae95c-122">Authorization</span></span>  | <span data-ttu-id="ae95c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae95c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae95c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae95c-125">Request body</span></span>
<span data-ttu-id="ae95c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae95c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae95c-127">响应</span><span class="sxs-lookup"><span data-stu-id="ae95c-127">Response</span></span>

<span data-ttu-id="ae95c-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleSummary](../resources/privilegedrolesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ae95c-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="ae95c-129">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="ae95c-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ae95c-130">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="ae95c-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ae95c-131">示例</span><span class="sxs-lookup"><span data-stu-id="ae95c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae95c-132">请求</span><span class="sxs-lookup"><span data-stu-id="ae95c-132">Request</span></span>
<span data-ttu-id="ae95c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae95c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="ae95c-134">响应</span><span class="sxs-lookup"><span data-stu-id="ae95c-134">Response</span></span>
<span data-ttu-id="ae95c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae95c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
