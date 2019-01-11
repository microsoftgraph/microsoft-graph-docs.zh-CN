---
title: 列表 privilegedRoleAssignments
description: 检索 privilegedRoleAssignment 对象，对应于组织的所有角色分配列表。
localization_priority: Normal
ms.openlocfilehash: ee6fac823e4d05eb13ada0a3ad1082ba1a78a7e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838659"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="16b9d-103">列表 privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="16b9d-103">List privilegedRoleAssignments</span></span>

> <span data-ttu-id="16b9d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="16b9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16b9d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16b9d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16b9d-106">检索[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象，对应于组织的所有角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="16b9d-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="16b9d-107">权限</span><span class="sxs-lookup"><span data-stu-id="16b9d-107">Permissions</span></span>
<span data-ttu-id="16b9d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16b9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="16b9d-110">请求者需要拥有以下角色之一：_具有权限的角色管理员_、_全局管理员_、_安全管理员_或_安全读取器_。</span><span class="sxs-lookup"><span data-stu-id="16b9d-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="16b9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16b9d-111">Permission type</span></span>      | <span data-ttu-id="16b9d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16b9d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16b9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16b9d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16b9d-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16b9d-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16b9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16b9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b9d-116">Not supported.</span></span>    |
|<span data-ttu-id="16b9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16b9d-117">Application</span></span> | <span data-ttu-id="16b9d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b9d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16b9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16b9d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16b9d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16b9d-120">Optional query parameters</span></span>
<span data-ttu-id="16b9d-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16b9d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16b9d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="16b9d-122">Request headers</span></span>
| <span data-ttu-id="16b9d-123">名称</span><span class="sxs-lookup"><span data-stu-id="16b9d-123">Name</span></span>      |<span data-ttu-id="16b9d-124">说明</span><span class="sxs-lookup"><span data-stu-id="16b9d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16b9d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b9d-125">Authorization</span></span>  | <span data-ttu-id="16b9d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16b9d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16b9d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="16b9d-128">Request body</span></span>
<span data-ttu-id="16b9d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16b9d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b9d-130">响应</span><span class="sxs-lookup"><span data-stu-id="16b9d-130">Response</span></span>

<span data-ttu-id="16b9d-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="16b9d-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="16b9d-132">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="16b9d-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="16b9d-133">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="16b9d-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="16b9d-134">示例</span><span class="sxs-lookup"><span data-stu-id="16b9d-134">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="16b9d-135">获取所有角色分配</span><span class="sxs-lookup"><span data-stu-id="16b9d-135">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="16b9d-136">请求</span><span class="sxs-lookup"><span data-stu-id="16b9d-136">Request</span></span>
<span data-ttu-id="16b9d-137">下面的示例演示请求以获取所有角色分配：</span><span class="sxs-lookup"><span data-stu-id="16b9d-137">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="16b9d-138">响应</span><span class="sxs-lookup"><span data-stu-id="16b9d-138">Response</span></span>
<span data-ttu-id="16b9d-139">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="16b9d-139">The following example shows the response.</span></span> <span data-ttu-id="16b9d-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16b9d-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16b9d-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16b9d-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```
### <a name="get-active-role-assignments"></a><span data-ttu-id="16b9d-142">获取活动角色分配</span><span class="sxs-lookup"><span data-stu-id="16b9d-142">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="16b9d-143">请求</span><span class="sxs-lookup"><span data-stu-id="16b9d-143">Request</span></span> 
<span data-ttu-id="16b9d-144">下面的示例演示对查询的主动角色分配的请求：</span><span class="sxs-lookup"><span data-stu-id="16b9d-144">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="16b9d-145">响应</span><span class="sxs-lookup"><span data-stu-id="16b9d-145">Response</span></span>
<span data-ttu-id="16b9d-146">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="16b9d-146">The following example shows the response.</span></span> <span data-ttu-id="16b9d-147">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16b9d-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16b9d-148">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16b9d-148">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="16b9d-149">获取永久角色分配</span><span class="sxs-lookup"><span data-stu-id="16b9d-149">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="16b9d-150">请求</span><span class="sxs-lookup"><span data-stu-id="16b9d-150">Request</span></span> 
<span data-ttu-id="16b9d-151">下面的示例演示请求查询永久角色分配，其中``expirationDateTime``值是``null``:</span><span class="sxs-lookup"><span data-stu-id="16b9d-151">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="16b9d-152">响应</span><span class="sxs-lookup"><span data-stu-id="16b9d-152">Response</span></span>
<span data-ttu-id="16b9d-153">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="16b9d-153">The following example shows the response.</span></span> <span data-ttu-id="16b9d-154">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16b9d-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16b9d-155">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16b9d-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="16b9d-156">获取合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="16b9d-156">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="16b9d-157">请求</span><span class="sxs-lookup"><span data-stu-id="16b9d-157">Request</span></span> 
<span data-ttu-id="16b9d-158">下面的示例演示向查询合格的角色分配，包括活动和非活动的请求：</span><span class="sxs-lookup"><span data-stu-id="16b9d-158">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="16b9d-159">响应</span><span class="sxs-lookup"><span data-stu-id="16b9d-159">Response</span></span> 
<span data-ttu-id="16b9d-160">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="16b9d-160">The following example shows the response.</span></span> <span data-ttu-id="16b9d-161">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16b9d-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16b9d-162">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16b9d-162">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
