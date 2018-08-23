# <a name="update-device"></a><span data-ttu-id="bafbf-101">更新设备</span><span class="sxs-lookup"><span data-stu-id="bafbf-101">Update device</span></span>

<span data-ttu-id="bafbf-102">更新已注册设备的属性。</span><span class="sxs-lookup"><span data-stu-id="bafbf-102">Update the properties of a registered device.</span></span>

<span data-ttu-id="bafbf-103">设备的特定属性只能通过获准的移动设备管理 (MDM) 应用进行更新。</span><span class="sxs-lookup"><span data-stu-id="bafbf-103">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="bafbf-104">权限</span><span class="sxs-lookup"><span data-stu-id="bafbf-104">Permissions</span></span>
<span data-ttu-id="bafbf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bafbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bafbf-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="bafbf-107">Permission type</span></span>      | <span data-ttu-id="bafbf-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bafbf-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bafbf-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bafbf-109">Delegated (work or school account)</span></span> | <span data-ttu-id="bafbf-110">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bafbf-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bafbf-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bafbf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bafbf-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="bafbf-112">Not supported.</span></span> |
|<span data-ttu-id="bafbf-113">应用</span><span class="sxs-lookup"><span data-stu-id="bafbf-113">Application</span></span> | <span data-ttu-id="bafbf-114">不支持</span><span class="sxs-lookup"><span data-stu-id="bafbf-114">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="bafbf-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="bafbf-116">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="bafbf-116">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bafbf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bafbf-117">Request headers</span></span>
| <span data-ttu-id="bafbf-118">名称</span><span class="sxs-lookup"><span data-stu-id="bafbf-118">Name</span></span>       | <span data-ttu-id="bafbf-119">类型</span><span class="sxs-lookup"><span data-stu-id="bafbf-119">Type</span></span> | <span data-ttu-id="bafbf-120">说明</span><span class="sxs-lookup"><span data-stu-id="bafbf-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bafbf-121">授权</span><span class="sxs-lookup"><span data-stu-id="bafbf-121">Authorization</span></span>  | <span data-ttu-id="bafbf-122">字符串</span><span class="sxs-lookup"><span data-stu-id="bafbf-122">string</span></span>  | <span data-ttu-id="bafbf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bafbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bafbf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bafbf-125">Request body</span></span>

<span data-ttu-id="bafbf-126">在请求正文中，提供应更新的 [device](../resources/device.md) 属性值。</span><span class="sxs-lookup"><span data-stu-id="bafbf-126">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="bafbf-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bafbf-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bafbf-128">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bafbf-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bafbf-129">属性</span><span class="sxs-lookup"><span data-stu-id="bafbf-129">Property</span></span>     | <span data-ttu-id="bafbf-130">类型</span><span class="sxs-lookup"><span data-stu-id="bafbf-130">Type</span></span>   |<span data-ttu-id="bafbf-131">说明</span><span class="sxs-lookup"><span data-stu-id="bafbf-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bafbf-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="bafbf-132">accountEnabled</span></span>|<span data-ttu-id="bafbf-133">布尔</span><span class="sxs-lookup"><span data-stu-id="bafbf-133">Boolean</span></span>| <span data-ttu-id="bafbf-134">如果帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="bafbf-134">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="bafbf-135">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bafbf-135">operatingSystem</span></span>|<span data-ttu-id="bafbf-136">字符串</span><span class="sxs-lookup"><span data-stu-id="bafbf-136">String</span></span>|<span data-ttu-id="bafbf-137">设备上的操作系统类型。</span><span class="sxs-lookup"><span data-stu-id="bafbf-137">The type of operating system on the device.</span></span>|
|<span data-ttu-id="bafbf-138">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="bafbf-138">operatingSystemVersion</span></span>|<span data-ttu-id="bafbf-139">字符串</span><span class="sxs-lookup"><span data-stu-id="bafbf-139">String</span></span>|<span data-ttu-id="bafbf-140">设备上的操作系统版本</span><span class="sxs-lookup"><span data-stu-id="bafbf-140">The version of the operating system on the device</span></span>|
|<span data-ttu-id="bafbf-141">displayName</span><span class="sxs-lookup"><span data-stu-id="bafbf-141">displayName</span></span>|<span data-ttu-id="bafbf-142">字符串</span><span class="sxs-lookup"><span data-stu-id="bafbf-142">String</span></span>|<span data-ttu-id="bafbf-143">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="bafbf-143">The display name for the device.</span></span>|
|<span data-ttu-id="bafbf-144">isCompliant</span><span class="sxs-lookup"><span data-stu-id="bafbf-144">isCompliant</span></span>|<span data-ttu-id="bafbf-145">布尔</span><span class="sxs-lookup"><span data-stu-id="bafbf-145">Boolean</span></span>|<span data-ttu-id="bafbf-146">如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。</span><span class="sxs-lookup"><span data-stu-id="bafbf-146">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="bafbf-147">此值只可以由 Intune 针对任何设备操作系统类型或[经批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)针对 Windows 操作系统设备更新。</span><span class="sxs-lookup"><span data-stu-id="bafbf-147">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="bafbf-148">isManaged</span><span class="sxs-lookup"><span data-stu-id="bafbf-148">isManaged</span></span>|<span data-ttu-id="bafbf-149">布尔</span><span class="sxs-lookup"><span data-stu-id="bafbf-149">Boolean</span></span>|<span data-ttu-id="bafbf-150">如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="bafbf-150">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="bafbf-151">此值只可以由 Intune 针对任何设备操作系统类型或[经批准 MDM 应用程序](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)针对 Windows 操作系统设备更新。</span><span class="sxs-lookup"><span data-stu-id="bafbf-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="bafbf-152">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-152">Response</span></span>

<span data-ttu-id="bafbf-153">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bafbf-153">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bafbf-154">示例</span><span class="sxs-lookup"><span data-stu-id="bafbf-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bafbf-155">请求</span><span class="sxs-lookup"><span data-stu-id="bafbf-155">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="bafbf-156">响应</span><span class="sxs-lookup"><span data-stu-id="bafbf-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
