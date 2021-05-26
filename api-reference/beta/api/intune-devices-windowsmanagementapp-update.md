---
title: 更新 windowsManagementApp
description: 更新 windowsManagementApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15fea6f46279f96ce3d1f235b92475bdc67d0f16
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662940"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="fe748-103">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="fe748-103">Update windowsManagementApp</span></span>

<span data-ttu-id="fe748-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe748-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe748-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe748-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe748-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe748-107">更新 [windowsManagementApp 对象](../resources/intune-devices-windowsmanagementapp.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="fe748-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe748-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe748-108">Prerequisites</span></span>
<span data-ttu-id="fe748-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe748-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe748-111">Permission type</span></span>|<span data-ttu-id="fe748-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe748-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe748-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe748-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe748-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe748-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe748-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe748-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe748-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe748-116">Not supported.</span></span>|
|<span data-ttu-id="fe748-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe748-117">Application</span></span>|<span data-ttu-id="fe748-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe748-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe748-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe748-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="fe748-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe748-120">Request headers</span></span>
|<span data-ttu-id="fe748-121">标头</span><span class="sxs-lookup"><span data-stu-id="fe748-121">Header</span></span>|<span data-ttu-id="fe748-122">值</span><span class="sxs-lookup"><span data-stu-id="fe748-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe748-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe748-123">Authorization</span></span>|<span data-ttu-id="fe748-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe748-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe748-125">接受</span><span class="sxs-lookup"><span data-stu-id="fe748-125">Accept</span></span>|<span data-ttu-id="fe748-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe748-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe748-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe748-127">Request body</span></span>
<span data-ttu-id="fe748-128">在请求正文中，提供 [windowsManagementApp 对象的](../resources/intune-devices-windowsmanagementapp.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe748-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="fe748-129">下表显示创建 [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe748-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="fe748-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe748-130">Property</span></span>|<span data-ttu-id="fe748-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe748-131">Type</span></span>|<span data-ttu-id="fe748-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe748-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe748-133">id</span><span class="sxs-lookup"><span data-stu-id="fe748-133">id</span></span>|<span data-ttu-id="fe748-134">String</span><span class="sxs-lookup"><span data-stu-id="fe748-134">String</span></span>|<span data-ttu-id="fe748-135">管理应用程序的唯Windows标识符</span><span class="sxs-lookup"><span data-stu-id="fe748-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="fe748-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="fe748-136">availableVersion</span></span>|<span data-ttu-id="fe748-137">String</span><span class="sxs-lookup"><span data-stu-id="fe748-137">String</span></span>|<span data-ttu-id="fe748-138">Windows管理应用可用版本。</span><span class="sxs-lookup"><span data-stu-id="fe748-138">Windows management app available version.</span></span>|
|<span data-ttu-id="fe748-139">managedInstaller</span><span class="sxs-lookup"><span data-stu-id="fe748-139">managedInstaller</span></span>|[<span data-ttu-id="fe748-140">managedInstallerStatus</span><span class="sxs-lookup"><span data-stu-id="fe748-140">managedInstallerStatus</span></span>](../resources/intune-devices-managedinstallerstatus.md)|<span data-ttu-id="fe748-141">托管安装程序状态。</span><span class="sxs-lookup"><span data-stu-id="fe748-141">Managed Installer Status.</span></span> <span data-ttu-id="fe748-142">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="fe748-142">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="fe748-143">managedInstallerConfiguredDateTime</span><span class="sxs-lookup"><span data-stu-id="fe748-143">managedInstallerConfiguredDateTime</span></span>|<span data-ttu-id="fe748-144">String</span><span class="sxs-lookup"><span data-stu-id="fe748-144">String</span></span>|<span data-ttu-id="fe748-145">托管安装程序配置的日期时间</span><span class="sxs-lookup"><span data-stu-id="fe748-145">Managed Installer Configured Date Time</span></span>|



## <a name="response"></a><span data-ttu-id="fe748-146">响应</span><span class="sxs-lookup"><span data-stu-id="fe748-146">Response</span></span>
<span data-ttu-id="fe748-147">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe748-147">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe748-148">示例</span><span class="sxs-lookup"><span data-stu-id="fe748-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe748-149">请求</span><span class="sxs-lookup"><span data-stu-id="fe748-149">Request</span></span>
<span data-ttu-id="fe748-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe748-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="fe748-151">响应</span><span class="sxs-lookup"><span data-stu-id="fe748-151">Response</span></span>
<span data-ttu-id="fe748-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe748-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```




