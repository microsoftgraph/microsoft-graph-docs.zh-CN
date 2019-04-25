---
title: 列出设备可传递组
description: 获取设备所属的组。 此 API 请求是可传递的, 并且还将返回设备是其嵌套成员的所有组。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: fbe7aee8066c56ad9f49dd2ad77fedfe0b75fbfc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583639"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="7807c-104">列出设备可传递组</span><span class="sxs-lookup"><span data-stu-id="7807c-104">List device transitive groups</span></span>

<span data-ttu-id="7807c-105">获取设备所属的组。</span><span class="sxs-lookup"><span data-stu-id="7807c-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="7807c-106">此 API 请求是可传递的, 并且还将返回设备是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="7807c-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="7807c-107">权限</span><span class="sxs-lookup"><span data-stu-id="7807c-107">Permissions</span></span>

<span data-ttu-id="7807c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7807c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7807c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7807c-110">Permission type</span></span>      | <span data-ttu-id="7807c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7807c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7807c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7807c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7807c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7807c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7807c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7807c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7807c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7807c-115">Not supported.</span></span>    |
|<span data-ttu-id="7807c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7807c-116">Application</span></span> | <span data-ttu-id="7807c-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7807c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7807c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7807c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7807c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7807c-119">Optional query parameters</span></span>

<span data-ttu-id="7807c-120">此方法支持 [OData 查询参数](/graph/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7807c-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7807c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7807c-121">Request headers</span></span>

| <span data-ttu-id="7807c-122">标头</span><span class="sxs-lookup"><span data-stu-id="7807c-122">Header</span></span>       | <span data-ttu-id="7807c-123">值</span><span class="sxs-lookup"><span data-stu-id="7807c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7807c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7807c-124">Authorization</span></span>  | <span data-ttu-id="7807c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7807c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7807c-127">接受</span><span class="sxs-lookup"><span data-stu-id="7807c-127">Accept</span></span>  | <span data-ttu-id="7807c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7807c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7807c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7807c-129">Request body</span></span>

<span data-ttu-id="7807c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7807c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7807c-131">响应</span><span class="sxs-lookup"><span data-stu-id="7807c-131">Response</span></span>

<span data-ttu-id="7807c-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7807c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7807c-133">示例</span><span class="sxs-lookup"><span data-stu-id="7807c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7807c-134">请求</span><span class="sxs-lookup"><span data-stu-id="7807c-134">Request</span></span>

<span data-ttu-id="7807c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7807c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="7807c-136">响应</span><span class="sxs-lookup"><span data-stu-id="7807c-136">Response</span></span>

<span data-ttu-id="7807c-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7807c-137">Here is an example of the response.</span></span> 

><span data-ttu-id="7807c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7807c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->