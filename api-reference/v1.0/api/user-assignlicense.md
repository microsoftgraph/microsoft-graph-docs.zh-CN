---
title: assignLicense
description: 为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1110d7d68dcc700c57a993b7c09defc0ec7f709
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865814"
---
# <a name="user-assignlicense"></a><span data-ttu-id="4df11-104">用户：assignLicense</span><span class="sxs-lookup"><span data-stu-id="4df11-104">user: assignLicense</span></span>
<span data-ttu-id="4df11-p102">为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="4df11-p102">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4df11-107">权限</span><span class="sxs-lookup"><span data-stu-id="4df11-107">Permissions</span></span>
<span data-ttu-id="4df11-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4df11-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4df11-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4df11-110">Permission type</span></span>      | <span data-ttu-id="4df11-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4df11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4df11-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4df11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4df11-113">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4df11-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4df11-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4df11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4df11-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4df11-115">Not supported.</span></span>    |
|<span data-ttu-id="4df11-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4df11-116">Application</span></span> | <span data-ttu-id="4df11-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4df11-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4df11-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4df11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="4df11-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4df11-119">Request headers</span></span>
| <span data-ttu-id="4df11-120">标头</span><span class="sxs-lookup"><span data-stu-id="4df11-120">Header</span></span>       | <span data-ttu-id="4df11-121">值</span><span class="sxs-lookup"><span data-stu-id="4df11-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4df11-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4df11-122">Authorization</span></span>  | <span data-ttu-id="4df11-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4df11-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4df11-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4df11-125">Content-Type</span></span>  | <span data-ttu-id="4df11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4df11-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4df11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4df11-127">Request body</span></span>
<span data-ttu-id="4df11-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4df11-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4df11-129">参数</span><span class="sxs-lookup"><span data-stu-id="4df11-129">Parameter</span></span>    | <span data-ttu-id="4df11-130">类型</span><span class="sxs-lookup"><span data-stu-id="4df11-130">Type</span></span>   |<span data-ttu-id="4df11-131">说明</span><span class="sxs-lookup"><span data-stu-id="4df11-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4df11-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="4df11-132">addLicenses</span></span>|<span data-ttu-id="4df11-133">AssignedLicense 集合</span><span class="sxs-lookup"><span data-stu-id="4df11-133">AssignedLicense collection</span></span>|<span data-ttu-id="4df11-p105">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。可以通过设置 [assignedLicense](../resources/assignedlicense.md) 对象中的 **disabledPlans** 属性禁用与许可证相关的计划。</span><span class="sxs-lookup"><span data-stu-id="4df11-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="4df11-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="4df11-136">removeLicenses</span></span>|<span data-ttu-id="4df11-137">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="4df11-137">Guid collection</span></span>|<span data-ttu-id="4df11-138">标识要删除的许可证的 GUID 的集合。</span><span class="sxs-lookup"><span data-stu-id="4df11-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="4df11-139">响应</span><span class="sxs-lookup"><span data-stu-id="4df11-139">Response</span></span>

<span data-ttu-id="4df11-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4df11-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4df11-141">示例</span><span class="sxs-lookup"><span data-stu-id="4df11-141">Example</span></span>
<span data-ttu-id="4df11-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4df11-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4df11-143">请求</span><span class="sxs-lookup"><span data-stu-id="4df11-143">Request</span></span>
<span data-ttu-id="4df11-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4df11-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4df11-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4df11-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4df11-146">C#</span><span class="sxs-lookup"><span data-stu-id="4df11-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4df11-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4df11-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4df11-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4df11-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4df11-149">Java</span><span class="sxs-lookup"><span data-stu-id="4df11-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4df11-150">响应</span><span class="sxs-lookup"><span data-stu-id="4df11-150">Response</span></span>
<span data-ttu-id="4df11-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4df11-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
