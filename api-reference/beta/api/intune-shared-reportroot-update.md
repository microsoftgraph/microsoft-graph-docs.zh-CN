---
title: 更新 reportRoot
description: 更新 reportRoot 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1b58de10b42c1343fda22bf48e3fe02e3be4452
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458145"
---
# <a name="update-reportroot"></a><span data-ttu-id="8e5fc-103">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="8e5fc-103">Update reportRoot</span></span>

<span data-ttu-id="8e5fc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8e5fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e5fc-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8e5fc-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e5fc-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e5fc-108">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-108">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e5fc-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e5fc-109">Prerequisites</span></span>
<span data-ttu-id="8e5fc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e5fc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e5fc-112">Permission type</span></span>|<span data-ttu-id="8e5fc-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8e5fc-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e5fc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e5fc-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8e5fc-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8e5fc-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8e5fc-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5fc-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8e5fc-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="8e5fc-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8e5fc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5fc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e5fc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e5fc-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e5fc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-120">Not supported.</span></span>|
|<span data-ttu-id="8e5fc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e5fc-121">Application</span></span>||
| <span data-ttu-id="8e5fc-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8e5fc-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8e5fc-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5fc-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8e5fc-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="8e5fc-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8e5fc-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5fc-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e5fc-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e5fc-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="8e5fc-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e5fc-127">Request headers</span></span>
|<span data-ttu-id="8e5fc-128">标头</span><span class="sxs-lookup"><span data-stu-id="8e5fc-128">Header</span></span>|<span data-ttu-id="8e5fc-129">值</span><span class="sxs-lookup"><span data-stu-id="8e5fc-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e5fc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e5fc-130">Authorization</span></span>|<span data-ttu-id="8e5fc-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e5fc-132">接受</span><span class="sxs-lookup"><span data-stu-id="8e5fc-132">Accept</span></span>|<span data-ttu-id="8e5fc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="8e5fc-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e5fc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e5fc-134">Request body</span></span>
<span data-ttu-id="8e5fc-135">在请求正文中，提供 [reportRoot](../resources/intune-shared-reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-135">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="8e5fc-136">下表显示了创建 [reportRoot](../resources/intune-shared-reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-136">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="8e5fc-137">属性</span><span class="sxs-lookup"><span data-stu-id="8e5fc-137">Property</span></span>|<span data-ttu-id="8e5fc-138">类型</span><span class="sxs-lookup"><span data-stu-id="8e5fc-138">Type</span></span>|<span data-ttu-id="8e5fc-139">说明</span><span class="sxs-lookup"><span data-stu-id="8e5fc-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e5fc-140">id</span><span class="sxs-lookup"><span data-stu-id="8e5fc-140">id</span></span>|<span data-ttu-id="8e5fc-141">String</span><span class="sxs-lookup"><span data-stu-id="8e5fc-141">String</span></span>|<span data-ttu-id="8e5fc-142">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-142">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8e5fc-143">响应</span><span class="sxs-lookup"><span data-stu-id="8e5fc-143">Response</span></span>
<span data-ttu-id="8e5fc-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-144">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e5fc-145">示例</span><span class="sxs-lookup"><span data-stu-id="8e5fc-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e5fc-146">请求</span><span class="sxs-lookup"><span data-stu-id="8e5fc-146">Request</span></span>
<span data-ttu-id="8e5fc-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="8e5fc-148">响应</span><span class="sxs-lookup"><span data-stu-id="8e5fc-148">Response</span></span>
<span data-ttu-id="8e5fc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e5fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```











