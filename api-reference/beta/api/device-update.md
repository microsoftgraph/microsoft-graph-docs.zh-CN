---
title: 更新设备
description: 更新设备的属性。
author: tfitzmac
ms.openlocfilehash: df86581c1edb531e822204698486358fac29f106
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356558"
---
# <a name="update-device"></a><span data-ttu-id="880e9-103">更新设备</span><span class="sxs-lookup"><span data-stu-id="880e9-103">Update device</span></span>

> <span data-ttu-id="880e9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="880e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="880e9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="880e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="880e9-106">更新设备的属性。</span><span class="sxs-lookup"><span data-stu-id="880e9-106">Update the properties of a device.</span></span>

<span data-ttu-id="880e9-107">设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。</span><span class="sxs-lookup"><span data-stu-id="880e9-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="880e9-108">权限</span><span class="sxs-lookup"><span data-stu-id="880e9-108">Permissions</span></span>
<span data-ttu-id="880e9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="880e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="880e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="880e9-111">Permission type</span></span>      | <span data-ttu-id="880e9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="880e9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="880e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="880e9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="880e9-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="880e9-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="880e9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="880e9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="880e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="880e9-116">Not supported.</span></span> |
|<span data-ttu-id="880e9-117">应用</span><span class="sxs-lookup"><span data-stu-id="880e9-117">Application</span></span> | <span data-ttu-id="880e9-118">不支持</span><span class="sxs-lookup"><span data-stu-id="880e9-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="880e9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="880e9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="880e9-120">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="880e9-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="880e9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="880e9-121">Request headers</span></span>
| <span data-ttu-id="880e9-122">Name</span><span class="sxs-lookup"><span data-stu-id="880e9-122">Name</span></span>       | <span data-ttu-id="880e9-123">类型</span><span class="sxs-lookup"><span data-stu-id="880e9-123">Type</span></span> | <span data-ttu-id="880e9-124">说明</span><span class="sxs-lookup"><span data-stu-id="880e9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="880e9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="880e9-125">Authorization</span></span>  | <span data-ttu-id="880e9-126">string</span><span class="sxs-lookup"><span data-stu-id="880e9-126">string</span></span>  | <span data-ttu-id="880e9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="880e9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="880e9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="880e9-129">Request body</span></span>

<span data-ttu-id="880e9-130">在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。</span><span class="sxs-lookup"><span data-stu-id="880e9-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="880e9-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="880e9-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="880e9-132">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="880e9-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="880e9-133">属性</span><span class="sxs-lookup"><span data-stu-id="880e9-133">Property</span></span>     | <span data-ttu-id="880e9-134">类型</span><span class="sxs-lookup"><span data-stu-id="880e9-134">Type</span></span>   |<span data-ttu-id="880e9-135">说明</span><span class="sxs-lookup"><span data-stu-id="880e9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="880e9-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="880e9-136">accountEnabled</span></span>|<span data-ttu-id="880e9-137">布尔</span><span class="sxs-lookup"><span data-stu-id="880e9-137">Boolean</span></span>| <span data-ttu-id="880e9-138">如果帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="880e9-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="880e9-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="880e9-139">operatingSystem</span></span>|<span data-ttu-id="880e9-140">String</span><span class="sxs-lookup"><span data-stu-id="880e9-140">String</span></span>|<span data-ttu-id="880e9-141">设备上的操作系统类型。</span><span class="sxs-lookup"><span data-stu-id="880e9-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="880e9-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="880e9-142">operatingSystemVersion</span></span>|<span data-ttu-id="880e9-143">String</span><span class="sxs-lookup"><span data-stu-id="880e9-143">String</span></span>|<span data-ttu-id="880e9-144">设备上的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="880e9-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="880e9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="880e9-145">displayName</span></span>|<span data-ttu-id="880e9-146">String</span><span class="sxs-lookup"><span data-stu-id="880e9-146">String</span></span>|<span data-ttu-id="880e9-147">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="880e9-147">The display name for the device.</span></span>|
|<span data-ttu-id="880e9-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="880e9-148">isCompliant</span></span>|<span data-ttu-id="880e9-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="880e9-149">Boolean</span></span>|<span data-ttu-id="880e9-150">如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。</span><span class="sxs-lookup"><span data-stu-id="880e9-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="880e9-151">此值只可以由 Intune 的任何设备操作系统类型或[批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)的 Windows 操作系统设备更新。</span><span class="sxs-lookup"><span data-stu-id="880e9-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="880e9-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="880e9-152">isManaged</span></span>|<span data-ttu-id="880e9-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="880e9-153">Boolean</span></span>|<span data-ttu-id="880e9-154">如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="880e9-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="880e9-155">此值只可以由 Intune 的任何设备操作系统类型或[批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)的 Windows 操作系统设备更新。</span><span class="sxs-lookup"><span data-stu-id="880e9-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="880e9-156">由于**设备**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**设备**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="880e9-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="880e9-157">响应</span><span class="sxs-lookup"><span data-stu-id="880e9-157">Response</span></span>

<span data-ttu-id="880e9-158">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="880e9-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="880e9-159">示例</span><span class="sxs-lookup"><span data-stu-id="880e9-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="880e9-160">请求</span><span class="sxs-lookup"><span data-stu-id="880e9-160">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="880e9-161">响应</span><span class="sxs-lookup"><span data-stu-id="880e9-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="880e9-162">另请参阅</span><span class="sxs-lookup"><span data-stu-id="880e9-162">See also</span></span>

- [<span data-ttu-id="880e9-163">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="880e9-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="880e9-164">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="880e9-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="880e9-165">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="880e9-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
