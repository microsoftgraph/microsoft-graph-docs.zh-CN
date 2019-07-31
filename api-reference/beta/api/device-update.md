---
title: 更新设备
description: 更新设备的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3c83896caf151d069c29603995316e9f56c3147d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951314"
---
# <a name="update-device"></a><span data-ttu-id="41c59-103">更新设备</span><span class="sxs-lookup"><span data-stu-id="41c59-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41c59-104">更新设备的属性。</span><span class="sxs-lookup"><span data-stu-id="41c59-104">Update the properties of a device.</span></span>

<span data-ttu-id="41c59-105">设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。</span><span class="sxs-lookup"><span data-stu-id="41c59-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="41c59-106">权限</span><span class="sxs-lookup"><span data-stu-id="41c59-106">Permissions</span></span>
<span data-ttu-id="41c59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41c59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c59-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="41c59-109">Permission type</span></span>      | <span data-ttu-id="41c59-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41c59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41c59-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41c59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="41c59-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41c59-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="41c59-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41c59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41c59-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="41c59-114">Not supported.</span></span> |
|<span data-ttu-id="41c59-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="41c59-115">Application</span></span> | <span data-ttu-id="41c59-116">不支持</span><span class="sxs-lookup"><span data-stu-id="41c59-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="41c59-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41c59-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="41c59-118">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="41c59-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41c59-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41c59-119">Request headers</span></span>
| <span data-ttu-id="41c59-120">名称</span><span class="sxs-lookup"><span data-stu-id="41c59-120">Name</span></span>       | <span data-ttu-id="41c59-121">类型</span><span class="sxs-lookup"><span data-stu-id="41c59-121">Type</span></span> | <span data-ttu-id="41c59-122">说明</span><span class="sxs-lookup"><span data-stu-id="41c59-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41c59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41c59-123">Authorization</span></span>  | <span data-ttu-id="41c59-124">string</span><span class="sxs-lookup"><span data-stu-id="41c59-124">string</span></span>  | <span data-ttu-id="41c59-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41c59-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41c59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41c59-127">Request body</span></span>

<span data-ttu-id="41c59-128">在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。</span><span class="sxs-lookup"><span data-stu-id="41c59-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="41c59-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="41c59-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="41c59-130">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="41c59-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="41c59-131">属性</span><span class="sxs-lookup"><span data-stu-id="41c59-131">Property</span></span>     | <span data-ttu-id="41c59-132">类型</span><span class="sxs-lookup"><span data-stu-id="41c59-132">Type</span></span>   |<span data-ttu-id="41c59-133">说明</span><span class="sxs-lookup"><span data-stu-id="41c59-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41c59-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="41c59-134">accountEnabled</span></span>|<span data-ttu-id="41c59-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="41c59-135">Boolean</span></span>| <span data-ttu-id="41c59-136">如果帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="41c59-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="41c59-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="41c59-137">operatingSystem</span></span>|<span data-ttu-id="41c59-138">String</span><span class="sxs-lookup"><span data-stu-id="41c59-138">String</span></span>|<span data-ttu-id="41c59-139">设备上的操作系统类型。</span><span class="sxs-lookup"><span data-stu-id="41c59-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="41c59-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="41c59-140">operatingSystemVersion</span></span>|<span data-ttu-id="41c59-141">String</span><span class="sxs-lookup"><span data-stu-id="41c59-141">String</span></span>|<span data-ttu-id="41c59-142">设备上的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="41c59-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="41c59-143">displayName</span><span class="sxs-lookup"><span data-stu-id="41c59-143">displayName</span></span>|<span data-ttu-id="41c59-144">String</span><span class="sxs-lookup"><span data-stu-id="41c59-144">String</span></span>|<span data-ttu-id="41c59-145">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="41c59-145">The display name for the device.</span></span>|
|<span data-ttu-id="41c59-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="41c59-146">isCompliant</span></span>|<span data-ttu-id="41c59-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="41c59-147">Boolean</span></span>|<span data-ttu-id="41c59-148">如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。</span><span class="sxs-lookup"><span data-stu-id="41c59-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="41c59-149">这只能由 Intune 针对任何设备 OS 类型或经批准的适用于 Windows OS 设备的[MDM 应用](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。</span><span class="sxs-lookup"><span data-stu-id="41c59-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="41c59-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="41c59-150">isManaged</span></span>|<span data-ttu-id="41c59-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="41c59-151">Boolean</span></span>|<span data-ttu-id="41c59-152">如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="41c59-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="41c59-153">这只能由 Intune 针对任何设备 OS 类型或经批准的适用于 Windows OS 设备的[MDM 应用](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)进行更新。</span><span class="sxs-lookup"><span data-stu-id="41c59-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="41c59-154">由于**设备**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**设备**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="41c59-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="41c59-155">响应</span><span class="sxs-lookup"><span data-stu-id="41c59-155">Response</span></span>

<span data-ttu-id="41c59-156">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="41c59-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41c59-157">示例</span><span class="sxs-lookup"><span data-stu-id="41c59-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="41c59-158">请求</span><span class="sxs-lookup"><span data-stu-id="41c59-158">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41c59-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="41c59-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="41c59-160">C#</span><span class="sxs-lookup"><span data-stu-id="41c59-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41c59-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="41c59-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41c59-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="41c59-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41c59-163">Java</span><span class="sxs-lookup"><span data-stu-id="41c59-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41c59-164">响应</span><span class="sxs-lookup"><span data-stu-id="41c59-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="41c59-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="41c59-165">See also</span></span>

- [<span data-ttu-id="41c59-166">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="41c59-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="41c59-167">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="41c59-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="41c59-168">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="41c59-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
