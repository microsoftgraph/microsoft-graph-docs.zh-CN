---
title: 更新设备
description: 更新已注册设备的属性。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5f756633f7e6052c4eb954f953299603507b50ee
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442087"
---
# <a name="update-device"></a><span data-ttu-id="6cafd-103">更新设备</span><span class="sxs-lookup"><span data-stu-id="6cafd-103">Update device</span></span>

<span data-ttu-id="6cafd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cafd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cafd-105">更新已注册设备的属性。</span><span class="sxs-lookup"><span data-stu-id="6cafd-105">Update the properties of a registered device.</span></span>

<span data-ttu-id="6cafd-106">设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。</span><span class="sxs-lookup"><span data-stu-id="6cafd-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cafd-107">权限</span><span class="sxs-lookup"><span data-stu-id="6cafd-107">Permissions</span></span>
<span data-ttu-id="6cafd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cafd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cafd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cafd-110">Permission type</span></span>      | <span data-ttu-id="6cafd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cafd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cafd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cafd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6cafd-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cafd-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6cafd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cafd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cafd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cafd-115">Not supported.</span></span> |
|<span data-ttu-id="6cafd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cafd-116">Application</span></span> | <span data-ttu-id="6cafd-117">不支持</span><span class="sxs-lookup"><span data-stu-id="6cafd-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cafd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cafd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="6cafd-119">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="6cafd-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cafd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cafd-120">Request headers</span></span>
| <span data-ttu-id="6cafd-121">名称</span><span class="sxs-lookup"><span data-stu-id="6cafd-121">Name</span></span>       | <span data-ttu-id="6cafd-122">类型</span><span class="sxs-lookup"><span data-stu-id="6cafd-122">Type</span></span> | <span data-ttu-id="6cafd-123">说明</span><span class="sxs-lookup"><span data-stu-id="6cafd-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6cafd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cafd-124">Authorization</span></span>  | <span data-ttu-id="6cafd-125">string</span><span class="sxs-lookup"><span data-stu-id="6cafd-125">string</span></span>  | <span data-ttu-id="6cafd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cafd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cafd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cafd-128">Request body</span></span>

<span data-ttu-id="6cafd-129">在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。</span><span class="sxs-lookup"><span data-stu-id="6cafd-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="6cafd-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="6cafd-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6cafd-131">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="6cafd-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6cafd-132">属性</span><span class="sxs-lookup"><span data-stu-id="6cafd-132">Property</span></span>     | <span data-ttu-id="6cafd-133">类型</span><span class="sxs-lookup"><span data-stu-id="6cafd-133">Type</span></span>   |<span data-ttu-id="6cafd-134">说明</span><span class="sxs-lookup"><span data-stu-id="6cafd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cafd-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="6cafd-135">accountEnabled</span></span>|<span data-ttu-id="6cafd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cafd-136">Boolean</span></span>| <span data-ttu-id="6cafd-137">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="6cafd-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="6cafd-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="6cafd-138">operatingSystem</span></span>|<span data-ttu-id="6cafd-139">String</span><span class="sxs-lookup"><span data-stu-id="6cafd-139">String</span></span>|<span data-ttu-id="6cafd-140">设备上的操作系统类型。</span><span class="sxs-lookup"><span data-stu-id="6cafd-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="6cafd-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6cafd-141">operatingSystemVersion</span></span>|<span data-ttu-id="6cafd-142">String</span><span class="sxs-lookup"><span data-stu-id="6cafd-142">String</span></span>|<span data-ttu-id="6cafd-143">设备上的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="6cafd-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="6cafd-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6cafd-144">displayName</span></span>|<span data-ttu-id="6cafd-145">String</span><span class="sxs-lookup"><span data-stu-id="6cafd-145">String</span></span>|<span data-ttu-id="6cafd-146">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="6cafd-146">The display name for the device.</span></span>|
|<span data-ttu-id="6cafd-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="6cafd-147">isCompliant</span></span>|<span data-ttu-id="6cafd-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cafd-148">Boolean</span></span>|<span data-ttu-id="6cafd-149">如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。</span><span class="sxs-lookup"><span data-stu-id="6cafd-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="6cafd-150">这只能由 Intune 针对任何设备操作系统类型进行更新，或由适用于 Windows OS 设备的已批准 [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) 应用更新。</span><span class="sxs-lookup"><span data-stu-id="6cafd-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="6cafd-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="6cafd-151">isManaged</span></span>|<span data-ttu-id="6cafd-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cafd-152">Boolean</span></span>|<span data-ttu-id="6cafd-153">如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="6cafd-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="6cafd-154">这只能由 Intune 针对任何设备操作系统类型进行更新，或由适用于 Windows OS 设备的已批准 [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) 应用更新。</span><span class="sxs-lookup"><span data-stu-id="6cafd-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="6cafd-155">响应</span><span class="sxs-lookup"><span data-stu-id="6cafd-155">Response</span></span>

<span data-ttu-id="6cafd-156">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6cafd-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6cafd-157">示例</span><span class="sxs-lookup"><span data-stu-id="6cafd-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cafd-158">请求</span><span class="sxs-lookup"><span data-stu-id="6cafd-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6cafd-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cafd-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="6cafd-160">C#</span><span class="sxs-lookup"><span data-stu-id="6cafd-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cafd-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cafd-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cafd-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cafd-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cafd-163">Java</span><span class="sxs-lookup"><span data-stu-id="6cafd-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6cafd-164">响应</span><span class="sxs-lookup"><span data-stu-id="6cafd-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
