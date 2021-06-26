---
title: 通过 Windows Update for Business 部署服务注册更新管理
description: 当设备通过 Windows Update for Business 部署服务注册更新管理时，可以使用部署服务管理从 Windows Update 传递到该设备的内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 86a10a5b8b6878faad92e48132ab9283039ee3e6
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151424"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="de27b-103">通过 Windows Update for Business 部署服务注册更新管理</span><span class="sxs-lookup"><span data-stu-id="de27b-103">Enroll in update management by the Windows Update for Business deployment service</span></span>

<span data-ttu-id="de27b-104">当你通过 Windows Update for Business 部署服务在更新管理中注册设备时，可以使用部署服务管理从 Windows Update 传递到该设备的内容。</span><span class="sxs-lookup"><span data-stu-id="de27b-104">When you enroll device in update management by the Windows Update for Business deployment service, you can use the deployment service to manage content delivered from Windows Update to that device.</span></span> <span data-ttu-id="de27b-105">你可以按更新类别在更新管理中注册设备。</span><span class="sxs-lookup"><span data-stu-id="de27b-105">You can enroll a device in update management by update category.</span></span>

<span data-ttu-id="de27b-106">现在，部署服务支持注册管理Windows 10更新。</span><span class="sxs-lookup"><span data-stu-id="de27b-106">Today, the deployment service supports enrollment in management of Windows 10 feature updates.</span></span> <span data-ttu-id="de27b-107">目前，部署服务不需要注册管理质量Windows 10以部署快速的质量更新。</span><span class="sxs-lookup"><span data-stu-id="de27b-107">At this time, the deployment service does not require enrollment in management of Windows 10 quality updates in order to deploy expedited quality updates.</span></span>

## <a name="enroll-the-device-in-update-management"></a><span data-ttu-id="de27b-108">在更新管理中注册设备</span><span class="sxs-lookup"><span data-stu-id="de27b-108">Enroll the device in update management</span></span>

<span data-ttu-id="de27b-109">当你为某个更新类别注册管理中的设备时，部署服务将成为该类别的更新（来自 Windows 更新）的颁发机构。</span><span class="sxs-lookup"><span data-stu-id="de27b-109">When you enroll a device in management for a certain update category, the deployment service becomes the authority for updates of that category coming from Windows Update.</span></span> <span data-ttu-id="de27b-110">因此，设备不会从 Windows Update 接收该类别的更新，直到你通过使用部署服务将其分配给部署 来部署[更新](windowsupdates-deployments.md)。</span><span class="sxs-lookup"><span data-stu-id="de27b-110">As a result, devices do not receive updates of that category from Windows Update until you deploy an update using the deployment service by assigning it to a [deployment](windowsupdates-deployments.md).</span></span> <span data-ttu-id="de27b-111">设备在服务注册管理时会自动注册到服务 (即 [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) 对象在设备上不存在时) 。</span><span class="sxs-lookup"><span data-stu-id="de27b-111">Devices are automatically registered with the service when enrolled in management by the service (i.e. an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) object is automatically created if it does not already exist).</span></span>

### <a name="request"></a><span data-ttu-id="de27b-112">请求</span><span class="sxs-lookup"><span data-stu-id="de27b-112">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="de27b-113">响应</span><span class="sxs-lookup"><span data-stu-id="de27b-113">Response</span></span>

``` http
HTTP/1.1 202 Accepted
```

## <a name="check-the-enrollment-state-of-a-device"></a><span data-ttu-id="de27b-114">检查设备的注册状态</span><span class="sxs-lookup"><span data-stu-id="de27b-114">Check the enrollment state of a device</span></span>

<span data-ttu-id="de27b-115">可以通过获取设备并查看 **azureADDevice** 对象的 **注册和错误** 属性来检查设备的注册状态。 [](/graph/api/windowsupdates-azureaddevice-get)</span><span class="sxs-lookup"><span data-stu-id="de27b-115">You can check the enrollment state of a device by [getting the device](/graph/api/windowsupdates-azureaddevice-get) and looking at the **enrollments** and **errors** properties on the **azureADDevice** object.</span></span> <span data-ttu-id="de27b-116">在更新管理中成功注册的设备在注册集合中具有 [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) 对象，并且它在错误集合中没有任何 [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) 对象。</span><span class="sxs-lookup"><span data-stu-id="de27b-116">A device that is successfully enrolled in update management has an [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) object in the enrollments collection, and it does not have any [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) objects in the errors collection.</span></span> <span data-ttu-id="de27b-117">服务尝试注册但遇到错误的设备已填充注册和错误的集合。</span><span class="sxs-lookup"><span data-stu-id="de27b-117">A device that the service tried to enroll but encountered an error has populated collections for both enrollments and errors.</span></span> <span data-ttu-id="de27b-118">服务尚未收到任何注册请求的设备具有注册和错误的空集合。</span><span class="sxs-lookup"><span data-stu-id="de27b-118">A device for which the service has not received any enrollment requests has empty collections for both enrollments and errors.</span></span>

<span data-ttu-id="de27b-119">以下示例显示已成功注册服务功能更新管理的设备。</span><span class="sxs-lookup"><span data-stu-id="de27b-119">The following example shows a device that is successfully enrolled in management of feature updates by the service.</span></span>

### <a name="request"></a><span data-ttu-id="de27b-120">请求</span><span class="sxs-lookup"><span data-stu-id="de27b-120">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a><span data-ttu-id="de27b-121">响应</span><span class="sxs-lookup"><span data-stu-id="de27b-121">Response</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a><span data-ttu-id="de27b-122">注销服务管理或注销服务</span><span class="sxs-lookup"><span data-stu-id="de27b-122">Unenroll from management by the service or unregister from the service</span></span> 

<span data-ttu-id="de27b-123">当注销设备以从服务管理给定更新类别时，该设备将不再由部署服务管理，并且可能会开始根据 Windows Update 的策略配置接收其他更新。</span><span class="sxs-lookup"><span data-stu-id="de27b-123">When you unenroll a device from management by the service for a given update category, the device is no longer managed by the deployment service and may start receiving other updates from Windows Update based on its policy configuration.</span></span> <span data-ttu-id="de27b-124">如果将设备分配给给定更新类别的任何部署，则它不会接收该内容。</span><span class="sxs-lookup"><span data-stu-id="de27b-124">If the device is assigned to any deployments for the given update category, it does not receive that content.</span></span> <span data-ttu-id="de27b-125">设备仍注册到服务中，并且仍在注册并接收其他更新类别 (（如果适用) ）。</span><span class="sxs-lookup"><span data-stu-id="de27b-125">The device remains registered with the service and is still enrolled and receiving content for other update categories (if applicable).</span></span>

### <a name="request"></a><span data-ttu-id="de27b-126">请求</span><span class="sxs-lookup"><span data-stu-id="de27b-126">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="de27b-127">响应</span><span class="sxs-lookup"><span data-stu-id="de27b-127">Response</span></span>

``` http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="de27b-128">可以通过删除设备对象从服务中完全注销设备。</span><span class="sxs-lookup"><span data-stu-id="de27b-128">You can unregister a device from the service completely by deleting the device object.</span></span> <span data-ttu-id="de27b-129">当设备注销时，该服务会自动注销所有更新类别的管理，并且从每个 [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) 和 [updatableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup)中删除该设备。</span><span class="sxs-lookup"><span data-stu-id="de27b-129">When a device is unregistered, it is automatically unenrolled from management by the service for all update categories and removed from every [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) and [updatableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup).</span></span>

### <a name="request"></a><span data-ttu-id="de27b-130">请求</span><span class="sxs-lookup"><span data-stu-id="de27b-130">Request</span></span>

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a><span data-ttu-id="de27b-131">响应</span><span class="sxs-lookup"><span data-stu-id="de27b-131">Response</span></span>
``` http
HTTP/1.1 202 Accepted
```

