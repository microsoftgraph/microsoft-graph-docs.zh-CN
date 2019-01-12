---
title: assignLicense
description: 为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96ececfce4800560b1f2ae625d12e67d10f3f325
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965773"
---
# <a name="assignlicense"></a><span data-ttu-id="14d74-104">assignLicense</span><span class="sxs-lookup"><span data-stu-id="14d74-104">assignLicense</span></span>
<span data-ttu-id="14d74-p102">为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="14d74-p102">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="14d74-107">权限</span><span class="sxs-lookup"><span data-stu-id="14d74-107">Permissions</span></span>
<span data-ttu-id="14d74-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14d74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14d74-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14d74-110">Permission type</span></span>      | <span data-ttu-id="14d74-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14d74-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14d74-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14d74-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14d74-113">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d74-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="14d74-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14d74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14d74-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14d74-115">Not supported.</span></span>    |
|<span data-ttu-id="14d74-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14d74-116">Application</span></span> | <span data-ttu-id="14d74-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d74-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14d74-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14d74-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="14d74-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14d74-119">Request headers</span></span>
| <span data-ttu-id="14d74-120">标头</span><span class="sxs-lookup"><span data-stu-id="14d74-120">Header</span></span>       | <span data-ttu-id="14d74-121">值</span><span class="sxs-lookup"><span data-stu-id="14d74-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14d74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14d74-122">Authorization</span></span>  | <span data-ttu-id="14d74-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14d74-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14d74-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14d74-125">Content-Type</span></span>  | <span data-ttu-id="14d74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14d74-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14d74-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14d74-127">Request body</span></span>
<span data-ttu-id="14d74-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="14d74-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14d74-129">参数</span><span class="sxs-lookup"><span data-stu-id="14d74-129">Parameter</span></span>    | <span data-ttu-id="14d74-130">类型</span><span class="sxs-lookup"><span data-stu-id="14d74-130">Type</span></span>   |<span data-ttu-id="14d74-131">说明</span><span class="sxs-lookup"><span data-stu-id="14d74-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14d74-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="14d74-132">addLicenses</span></span>|<span data-ttu-id="14d74-133">AssignedLicense 集合</span><span class="sxs-lookup"><span data-stu-id="14d74-133">AssignedLicense collection</span></span>|<span data-ttu-id="14d74-p105">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。可以通过设置 [assignedLicense](../resources/assignedlicense.md) 对象中的 **disabledPlans** 属性禁用与许可证相关的计划。</span><span class="sxs-lookup"><span data-stu-id="14d74-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="14d74-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="14d74-136">removeLicenses</span></span>|<span data-ttu-id="14d74-137">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="14d74-137">Guid collection</span></span>|<span data-ttu-id="14d74-138">标识要删除的许可证的 GUID 的集合。</span><span class="sxs-lookup"><span data-stu-id="14d74-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="14d74-139">响应</span><span class="sxs-lookup"><span data-stu-id="14d74-139">Response</span></span>

<span data-ttu-id="14d74-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14d74-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d74-141">示例</span><span class="sxs-lookup"><span data-stu-id="14d74-141">Example</span></span>
<span data-ttu-id="14d74-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="14d74-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="14d74-143">请求</span><span class="sxs-lookup"><span data-stu-id="14d74-143">Request</span></span>
<span data-ttu-id="14d74-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14d74-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "guid"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="14d74-145">响应</span><span class="sxs-lookup"><span data-stu-id="14d74-145">Response</span></span>
<span data-ttu-id="14d74-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14d74-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "0118A350-71FC-4EC3-8F0C-6A1CB8867561"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-02T12:13:14Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
