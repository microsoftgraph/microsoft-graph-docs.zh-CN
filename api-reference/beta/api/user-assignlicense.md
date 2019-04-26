---
title: assignLicense
description: 添加或删除用户的许可证, 以启用或禁用其对 Microsoft 云产品的使用。 例如, 组织可以拥有具有100许可证的 Office 365 企业版 E3 订阅, 此请求将其中一个许可证分配给特定用户。 还可以启用和禁用与订阅相关的特定计划。 若要了解有关订阅和许可证的详细信息, 请参阅此 Technet 文章。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9946a7ac53a0e0e8b90a31fd4767bcc0549468
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547989"
---
# <a name="assignlicense"></a><span data-ttu-id="2ef6c-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="2ef6c-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef6c-107">添加或删除用户的许可证, 以启用或禁用其对 Microsoft 云产品的使用。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="2ef6c-108">例如, 组织可以拥有具有100许可证的 Office 365 企业版 E3 订阅, 此请求将其中一个许可证分配给特定用户。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="2ef6c-109">还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="2ef6c-110">若要了解有关订阅和许可证的详细信息, 请参阅此[Technet 文章](https://technet.microsoft.com/en-us/library/mt765146.aspx)。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="2ef6c-111">若要获取目录中可用的订阅, 请执行[get subscribedsku 请求](subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2ef6c-112">权限</span><span class="sxs-lookup"><span data-stu-id="2ef6c-112">Permissions</span></span>
<span data-ttu-id="2ef6c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef6c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ef6c-115">Permission type</span></span>      | <span data-ttu-id="2ef6c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ef6c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef6c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ef6c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef6c-118">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef6c-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ef6c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ef6c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef6c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-120">Not supported.</span></span>    |
|<span data-ttu-id="2ef6c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ef6c-121">Application</span></span> | <span data-ttu-id="2ef6c-122">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef6c-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef6c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ef6c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="2ef6c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ef6c-124">Request headers</span></span>
| <span data-ttu-id="2ef6c-125">标头</span><span class="sxs-lookup"><span data-stu-id="2ef6c-125">Header</span></span>       | <span data-ttu-id="2ef6c-126">值</span><span class="sxs-lookup"><span data-stu-id="2ef6c-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ef6c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ef6c-127">Authorization</span></span>  | <span data-ttu-id="2ef6c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2ef6c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ef6c-130">Content-Type</span></span>  | <span data-ttu-id="2ef6c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef6c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ef6c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ef6c-132">Request body</span></span>
<span data-ttu-id="2ef6c-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ef6c-134">参数</span><span class="sxs-lookup"><span data-stu-id="2ef6c-134">Parameter</span></span>    | <span data-ttu-id="2ef6c-135">类型</span><span class="sxs-lookup"><span data-stu-id="2ef6c-135">Type</span></span>   |<span data-ttu-id="2ef6c-136">说明</span><span class="sxs-lookup"><span data-stu-id="2ef6c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ef6c-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="2ef6c-137">addLicenses</span></span>|<span data-ttu-id="2ef6c-138">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="2ef6c-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="2ef6c-139">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="2ef6c-140">您可以通过在[assignedLicense](../resources/assignedlicense.md)对象上设置**disabledPlans**属性来禁用与许可证关联的 servicePlans。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="2ef6c-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="2ef6c-141">removeLicenses</span></span>|<span data-ttu-id="2ef6c-142">Guid</span><span class="sxs-lookup"><span data-stu-id="2ef6c-142">Guid</span></span>|<span data-ttu-id="2ef6c-143">标识要删除的许可证的 skuIds 的集合。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="2ef6c-144">响应</span><span class="sxs-lookup"><span data-stu-id="2ef6c-144">Response</span></span>

<span data-ttu-id="2ef6c-145">如果成功, 此方法在`200 OK`响应正文中返回响应代码和更新的[user](../resources/user.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef6c-146">示例</span><span class="sxs-lookup"><span data-stu-id="2ef6c-146">Example</span></span>
<span data-ttu-id="2ef6c-147">向用户添加许可证。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="2ef6c-148">请求</span><span class="sxs-lookup"><span data-stu-id="2ef6c-148">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="2ef6c-149">示例</span><span class="sxs-lookup"><span data-stu-id="2ef6c-149">Example</span></span>
<span data-ttu-id="2ef6c-150">删除用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-150">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="2ef6c-151">请求</span><span class="sxs-lookup"><span data-stu-id="2ef6c-151">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="2ef6c-152">响应</span><span class="sxs-lookup"><span data-stu-id="2ef6c-152">Response</span></span>
<span data-ttu-id="2ef6c-153">在这两个示例中, 响应是更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-153">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="2ef6c-154">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2ef6c-155">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ef6c-155">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
