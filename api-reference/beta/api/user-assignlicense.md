---
title: assignLicense
description: 添加或删除的用户启用或禁用 Microsoft 云服务及其使用的许可证。 例如，组织可以有 100 许可证，与 Office 365 企业版 E3 订阅，此请求将一个这些许可证分配给特定用户。 您还可以启用和禁用与订阅关联的特定计划。 若要了解有关订阅和许可证的详细信息，请参阅以下 Technet 文章。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82347f46855baa91b5a42452cdbacc914bc89cdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933790"
---
# <a name="assignlicense"></a><span data-ttu-id="805a1-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="805a1-106">assignLicense</span></span>

> <span data-ttu-id="805a1-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="805a1-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="805a1-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="805a1-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="805a1-109">添加或删除的用户启用或禁用 Microsoft 云服务及其使用的许可证。</span><span class="sxs-lookup"><span data-stu-id="805a1-109">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="805a1-110">例如，组织可以有 100 许可证，与 Office 365 企业版 E3 订阅，此请求将一个这些许可证分配给特定用户。</span><span class="sxs-lookup"><span data-stu-id="805a1-110">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="805a1-111">您还可以启用和禁用与订阅关联的特定计划。</span><span class="sxs-lookup"><span data-stu-id="805a1-111">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="805a1-112">若要了解有关订阅和许可证的详细信息，请参阅以下[Technet 文章](https://technet.microsoft.com/en-us/library/mt765146.aspx)。</span><span class="sxs-lookup"><span data-stu-id="805a1-112">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="805a1-113">若要获取的目录中可用的订阅，请执行[获取 subscribedSkus 请求](subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="805a1-113">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="805a1-114">权限</span><span class="sxs-lookup"><span data-stu-id="805a1-114">Permissions</span></span>
<span data-ttu-id="805a1-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="805a1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="805a1-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="805a1-117">Permission type</span></span>      | <span data-ttu-id="805a1-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="805a1-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="805a1-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="805a1-119">Delegated (work or school account)</span></span> | <span data-ttu-id="805a1-120">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="805a1-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="805a1-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="805a1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="805a1-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="805a1-122">Not supported.</span></span>    |
|<span data-ttu-id="805a1-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="805a1-123">Application</span></span> | <span data-ttu-id="805a1-124">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="805a1-124">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="805a1-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="805a1-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="805a1-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="805a1-126">Request headers</span></span>
| <span data-ttu-id="805a1-127">标头</span><span class="sxs-lookup"><span data-stu-id="805a1-127">Header</span></span>       | <span data-ttu-id="805a1-128">值</span><span class="sxs-lookup"><span data-stu-id="805a1-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="805a1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="805a1-129">Authorization</span></span>  | <span data-ttu-id="805a1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="805a1-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="805a1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="805a1-132">Content-Type</span></span>  | <span data-ttu-id="805a1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="805a1-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="805a1-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="805a1-134">Request body</span></span>
<span data-ttu-id="805a1-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="805a1-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="805a1-136">参数</span><span class="sxs-lookup"><span data-stu-id="805a1-136">Parameter</span></span>    | <span data-ttu-id="805a1-137">类型</span><span class="sxs-lookup"><span data-stu-id="805a1-137">Type</span></span>   |<span data-ttu-id="805a1-138">说明</span><span class="sxs-lookup"><span data-stu-id="805a1-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="805a1-139">addLicenses</span><span class="sxs-lookup"><span data-stu-id="805a1-139">addLicenses</span></span>|<span data-ttu-id="805a1-140">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="805a1-140">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="805a1-141">指定要添加的许可证的[assignedLicense](../resources/assignedlicense.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="805a1-141">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="805a1-142">您可以禁用 servicePlans 通过[assignedLicense](../resources/assignedlicense.md)对象上设置**disabledPlans**属性与许可相关联。</span><span class="sxs-lookup"><span data-stu-id="805a1-142">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="805a1-143">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="805a1-143">removeLicenses</span></span>|<span data-ttu-id="805a1-144">Guid</span><span class="sxs-lookup"><span data-stu-id="805a1-144">Guid</span></span>|<span data-ttu-id="805a1-145">标识要删除的许可证的 skuIds 的集合。</span><span class="sxs-lookup"><span data-stu-id="805a1-145">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="805a1-146">响应</span><span class="sxs-lookup"><span data-stu-id="805a1-146">Response</span></span>

<span data-ttu-id="805a1-147">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[用户](../resources/user.md)对象。</span><span class="sxs-lookup"><span data-stu-id="805a1-147">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="805a1-148">示例</span><span class="sxs-lookup"><span data-stu-id="805a1-148">Example</span></span>
<span data-ttu-id="805a1-149">添加到用户许可证。</span><span class="sxs-lookup"><span data-stu-id="805a1-149">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="805a1-150">请求</span><span class="sxs-lookup"><span data-stu-id="805a1-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a><span data-ttu-id="805a1-151">示例</span><span class="sxs-lookup"><span data-stu-id="805a1-151">Example</span></span>
<span data-ttu-id="805a1-152">从用户删除许可证。</span><span class="sxs-lookup"><span data-stu-id="805a1-152">Remove licenses from the user.</span></span>

#####<a name="request"></a><span data-ttu-id="805a1-153">请求</span><span class="sxs-lookup"><span data-stu-id="805a1-153">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="805a1-154">响应</span><span class="sxs-lookup"><span data-stu-id="805a1-154">Response</span></span>
<span data-ttu-id="805a1-155">在这两个示例中，响应是更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="805a1-155">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="805a1-156">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="805a1-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="805a1-157">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="805a1-157">All of the properties will be returned from an actual call.</span></span>
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
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
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
