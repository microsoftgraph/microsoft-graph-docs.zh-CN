---
title: 更新设备
description: 更新设备的属性。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3c895aa8d6122691520d17886ebcdb6f51a2a8c6
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786017"
---
# <a name="update-device"></a><span data-ttu-id="aa53a-103">更新设备</span><span class="sxs-lookup"><span data-stu-id="aa53a-103">Update device</span></span>

<span data-ttu-id="aa53a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa53a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa53a-105">更新设备的属性。</span><span class="sxs-lookup"><span data-stu-id="aa53a-105">Update the properties of a device.</span></span>

<span data-ttu-id="aa53a-106">设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。</span><span class="sxs-lookup"><span data-stu-id="aa53a-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa53a-107">权限</span><span class="sxs-lookup"><span data-stu-id="aa53a-107">Permissions</span></span>
<span data-ttu-id="aa53a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa53a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa53a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa53a-110">Permission type</span></span>      | <span data-ttu-id="aa53a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa53a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa53a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa53a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa53a-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa53a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="aa53a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa53a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa53a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa53a-115">Not supported.</span></span> |
|<span data-ttu-id="aa53a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa53a-116">Application</span></span> | <span data-ttu-id="aa53a-117">不支持</span><span class="sxs-lookup"><span data-stu-id="aa53a-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa53a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa53a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="aa53a-119">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="aa53a-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa53a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa53a-120">Request headers</span></span>
| <span data-ttu-id="aa53a-121">名称</span><span class="sxs-lookup"><span data-stu-id="aa53a-121">Name</span></span>       | <span data-ttu-id="aa53a-122">类型</span><span class="sxs-lookup"><span data-stu-id="aa53a-122">Type</span></span> | <span data-ttu-id="aa53a-123">说明</span><span class="sxs-lookup"><span data-stu-id="aa53a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa53a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa53a-124">Authorization</span></span>  | <span data-ttu-id="aa53a-125">string</span><span class="sxs-lookup"><span data-stu-id="aa53a-125">string</span></span>  | <span data-ttu-id="aa53a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa53a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa53a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa53a-128">Request body</span></span>

<span data-ttu-id="aa53a-129">在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。</span><span class="sxs-lookup"><span data-stu-id="aa53a-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="aa53a-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="aa53a-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="aa53a-131">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="aa53a-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aa53a-132">属性</span><span class="sxs-lookup"><span data-stu-id="aa53a-132">Property</span></span>     | <span data-ttu-id="aa53a-133">类型</span><span class="sxs-lookup"><span data-stu-id="aa53a-133">Type</span></span>   |<span data-ttu-id="aa53a-134">说明</span><span class="sxs-lookup"><span data-stu-id="aa53a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa53a-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="aa53a-135">accountEnabled</span></span>|<span data-ttu-id="aa53a-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa53a-136">Boolean</span></span>| <span data-ttu-id="aa53a-137">启用帐户时为 **true**，否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="aa53a-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="aa53a-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="aa53a-138">operatingSystem</span></span>|<span data-ttu-id="aa53a-139">String</span><span class="sxs-lookup"><span data-stu-id="aa53a-139">String</span></span>|<span data-ttu-id="aa53a-140">设备上的操作系统类型。</span><span class="sxs-lookup"><span data-stu-id="aa53a-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="aa53a-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="aa53a-141">operatingSystemVersion</span></span>|<span data-ttu-id="aa53a-142">String</span><span class="sxs-lookup"><span data-stu-id="aa53a-142">String</span></span>|<span data-ttu-id="aa53a-143">设备上的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="aa53a-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="aa53a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="aa53a-144">displayName</span></span>|<span data-ttu-id="aa53a-145">String</span><span class="sxs-lookup"><span data-stu-id="aa53a-145">String</span></span>|<span data-ttu-id="aa53a-146">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="aa53a-146">The display name for the device.</span></span>|
|<span data-ttu-id="aa53a-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="aa53a-147">isCompliant</span></span>|<span data-ttu-id="aa53a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa53a-148">Boolean</span></span>|<span data-ttu-id="aa53a-149">如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。</span><span class="sxs-lookup"><span data-stu-id="aa53a-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="aa53a-150">这仅可通过 Intune 针对任何设备操作系统类型进行更新，或由适用于任何操作系统设备的已批准[MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) Windows更新。</span><span class="sxs-lookup"><span data-stu-id="aa53a-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="aa53a-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="aa53a-151">isManaged</span></span>|<span data-ttu-id="aa53a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa53a-152">Boolean</span></span>|<span data-ttu-id="aa53a-153">如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="aa53a-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="aa53a-154">这仅可通过 Intune 针对任何设备操作系统类型进行更新，或由适用于任何操作系统设备的已批准[MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) Windows更新。</span><span class="sxs-lookup"><span data-stu-id="aa53a-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="aa53a-155">由于 **设备** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作添加、更新或删除现有设备实例中扩展的自定义属性中你自己的特定于 `PATCH` 应用的数据。</span><span class="sxs-lookup"><span data-stu-id="aa53a-155">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="aa53a-156">响应</span><span class="sxs-lookup"><span data-stu-id="aa53a-156">Response</span></span>

<span data-ttu-id="aa53a-157">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aa53a-157">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa53a-158">示例</span><span class="sxs-lookup"><span data-stu-id="aa53a-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aa53a-159">请求</span><span class="sxs-lookup"><span data-stu-id="aa53a-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aa53a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa53a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="aa53a-161">C#</span><span class="sxs-lookup"><span data-stu-id="aa53a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa53a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa53a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa53a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa53a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa53a-164">Java</span><span class="sxs-lookup"><span data-stu-id="aa53a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aa53a-165">响应</span><span class="sxs-lookup"><span data-stu-id="aa53a-165">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="aa53a-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aa53a-166">See also</span></span>

- [<span data-ttu-id="aa53a-167">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="aa53a-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="aa53a-168">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="aa53a-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="aa53a-169">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="aa53a-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
