---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。 已注册的所有者是云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。
ms.openlocfilehash: 9b2acee14598c631c7f782391cb22a7917685e02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046126"
---
# <a name="list-registeredowners"></a><span data-ttu-id="5eecf-106">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="5eecf-106">List registeredOwners</span></span>

> <span data-ttu-id="5eecf-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5eecf-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eecf-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5eecf-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5eecf-109">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="5eecf-109">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="5eecf-110">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="5eecf-110">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="5eecf-111">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="5eecf-111">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="5eecf-112">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="5eecf-112">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eecf-113">权限</span><span class="sxs-lookup"><span data-stu-id="5eecf-113">Permissions</span></span>

<span data-ttu-id="5eecf-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5eecf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eecf-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="5eecf-116">Permission type</span></span>      | <span data-ttu-id="5eecf-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5eecf-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eecf-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5eecf-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5eecf-119">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5eecf-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5eecf-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5eecf-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eecf-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5eecf-121">Not supported.</span></span>    |
|<span data-ttu-id="5eecf-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="5eecf-122">Application</span></span> | <span data-ttu-id="5eecf-123">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eecf-123">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eecf-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5eecf-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="5eecf-125">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="5eecf-125">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5eecf-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5eecf-126">Optional query parameters</span></span>
<span data-ttu-id="5eecf-127">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5eecf-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5eecf-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="5eecf-128">Request headers</span></span>
| <span data-ttu-id="5eecf-129">名称</span><span class="sxs-lookup"><span data-stu-id="5eecf-129">Name</span></span>       | <span data-ttu-id="5eecf-130">类型</span><span class="sxs-lookup"><span data-stu-id="5eecf-130">Type</span></span> | <span data-ttu-id="5eecf-131">说明</span><span class="sxs-lookup"><span data-stu-id="5eecf-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5eecf-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eecf-132">Authorization</span></span>  | <span data-ttu-id="5eecf-133">string</span><span class="sxs-lookup"><span data-stu-id="5eecf-133">string</span></span>  | <span data-ttu-id="5eecf-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5eecf-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eecf-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5eecf-136">Request body</span></span>
<span data-ttu-id="5eecf-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5eecf-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eecf-138">响应</span><span class="sxs-lookup"><span data-stu-id="5eecf-138">Response</span></span>

<span data-ttu-id="5eecf-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5eecf-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5eecf-140">示例</span><span class="sxs-lookup"><span data-stu-id="5eecf-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5eecf-141">请求</span><span class="sxs-lookup"><span data-stu-id="5eecf-141">Request</span></span>
<span data-ttu-id="5eecf-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5eecf-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="5eecf-143">响应</span><span class="sxs-lookup"><span data-stu-id="5eecf-143">Response</span></span>
<span data-ttu-id="5eecf-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5eecf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->