---
title: 更新设备
description: 更新已注册设备的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aaa8343307707142ca969c4257cc051e36a8cd7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889535"
---
# <a name="update-device"></a><span data-ttu-id="104b9-103">更新设备</span><span class="sxs-lookup"><span data-stu-id="104b9-103">Update device</span></span>

<span data-ttu-id="104b9-104">更新已注册设备的属性。</span><span class="sxs-lookup"><span data-stu-id="104b9-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="104b9-105">设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。</span><span class="sxs-lookup"><span data-stu-id="104b9-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="104b9-106">权限</span><span class="sxs-lookup"><span data-stu-id="104b9-106">Permissions</span></span>
<span data-ttu-id="104b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="104b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="104b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="104b9-109">Permission type</span></span>      | <span data-ttu-id="104b9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="104b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="104b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="104b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="104b9-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="104b9-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="104b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="104b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="104b9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="104b9-114">Not supported.</span></span> |
|<span data-ttu-id="104b9-115">应用</span><span class="sxs-lookup"><span data-stu-id="104b9-115">Application</span></span> | <span data-ttu-id="104b9-116">不支持</span><span class="sxs-lookup"><span data-stu-id="104b9-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="104b9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="104b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="104b9-118">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="104b9-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="104b9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="104b9-119">Request headers</span></span>
| <span data-ttu-id="104b9-120">名称</span><span class="sxs-lookup"><span data-stu-id="104b9-120">Name</span></span>       | <span data-ttu-id="104b9-121">类型</span><span class="sxs-lookup"><span data-stu-id="104b9-121">Type</span></span> | <span data-ttu-id="104b9-122">说明</span><span class="sxs-lookup"><span data-stu-id="104b9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="104b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="104b9-123">Authorization</span></span>  | <span data-ttu-id="104b9-124">string</span><span class="sxs-lookup"><span data-stu-id="104b9-124">string</span></span>  | <span data-ttu-id="104b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="104b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="104b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="104b9-127">Request body</span></span>

<span data-ttu-id="104b9-128">在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。</span><span class="sxs-lookup"><span data-stu-id="104b9-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="104b9-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="104b9-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="104b9-130">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="104b9-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="104b9-131">属性</span><span class="sxs-lookup"><span data-stu-id="104b9-131">Property</span></span>     | <span data-ttu-id="104b9-132">类型</span><span class="sxs-lookup"><span data-stu-id="104b9-132">Type</span></span>   |<span data-ttu-id="104b9-133">说明</span><span class="sxs-lookup"><span data-stu-id="104b9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="104b9-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="104b9-134">accountEnabled</span></span>|<span data-ttu-id="104b9-135">布尔</span><span class="sxs-lookup"><span data-stu-id="104b9-135">Boolean</span></span>| <span data-ttu-id="104b9-136">如果帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="104b9-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="104b9-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="104b9-137">operatingSystem</span></span>|<span data-ttu-id="104b9-138">String</span><span class="sxs-lookup"><span data-stu-id="104b9-138">String</span></span>|<span data-ttu-id="104b9-139">设备上的操作系统类型。</span><span class="sxs-lookup"><span data-stu-id="104b9-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="104b9-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="104b9-140">operatingSystemVersion</span></span>|<span data-ttu-id="104b9-141">String</span><span class="sxs-lookup"><span data-stu-id="104b9-141">String</span></span>|<span data-ttu-id="104b9-142">设备上的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="104b9-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="104b9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="104b9-143">displayName</span></span>|<span data-ttu-id="104b9-144">String</span><span class="sxs-lookup"><span data-stu-id="104b9-144">String</span></span>|<span data-ttu-id="104b9-145">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="104b9-145">The display name for the device.</span></span>|
|<span data-ttu-id="104b9-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="104b9-146">isCompliant</span></span>|<span data-ttu-id="104b9-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="104b9-147">Boolean</span></span>|<span data-ttu-id="104b9-148">如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。</span><span class="sxs-lookup"><span data-stu-id="104b9-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="104b9-149">此值只可以由 Intune 的任何设备操作系统类型或[批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)的 Windows 操作系统设备更新。</span><span class="sxs-lookup"><span data-stu-id="104b9-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="104b9-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="104b9-150">isManaged</span></span>|<span data-ttu-id="104b9-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="104b9-151">Boolean</span></span>|<span data-ttu-id="104b9-152">如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="104b9-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="104b9-153">此值只可以由 Intune 的任何设备操作系统类型或[批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)的 Windows 操作系统设备更新。</span><span class="sxs-lookup"><span data-stu-id="104b9-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="104b9-154">响应</span><span class="sxs-lookup"><span data-stu-id="104b9-154">Response</span></span>

<span data-ttu-id="104b9-155">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="104b9-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="104b9-156">示例</span><span class="sxs-lookup"><span data-stu-id="104b9-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="104b9-157">请求</span><span class="sxs-lookup"><span data-stu-id="104b9-157">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="104b9-158">响应</span><span class="sxs-lookup"><span data-stu-id="104b9-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
