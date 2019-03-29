---
title: 更新 windowsManagementApp
description: 更新 windowsManagementApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b68af1276d24845e3bb90b5e7a6db38a09806aa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962839"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="69f16-103">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="69f16-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="69f16-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69f16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f16-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69f16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f16-106">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69f16-106">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f16-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69f16-107">Prerequisites</span></span>
<span data-ttu-id="69f16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69f16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69f16-110">Permission type</span></span>|<span data-ttu-id="69f16-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69f16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69f16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69f16-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f16-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69f16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69f16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f16-115">Not supported.</span></span>|
|<span data-ttu-id="69f16-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69f16-116">Application</span></span>|<span data-ttu-id="69f16-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f16-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69f16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="69f16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="69f16-119">Request headers</span></span>
|<span data-ttu-id="69f16-120">标头</span><span class="sxs-lookup"><span data-stu-id="69f16-120">Header</span></span>|<span data-ttu-id="69f16-121">值</span><span class="sxs-lookup"><span data-stu-id="69f16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f16-122">Authorization</span></span>|<span data-ttu-id="69f16-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69f16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f16-124">接受</span><span class="sxs-lookup"><span data-stu-id="69f16-124">Accept</span></span>|<span data-ttu-id="69f16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69f16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f16-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69f16-126">Request body</span></span>
<span data-ttu-id="69f16-127">在请求正文中, 提供[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69f16-127">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="69f16-128">下表显示创建[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69f16-128">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="69f16-129">属性</span><span class="sxs-lookup"><span data-stu-id="69f16-129">Property</span></span>|<span data-ttu-id="69f16-130">类型</span><span class="sxs-lookup"><span data-stu-id="69f16-130">Type</span></span>|<span data-ttu-id="69f16-131">说明</span><span class="sxs-lookup"><span data-stu-id="69f16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f16-132">id</span><span class="sxs-lookup"><span data-stu-id="69f16-132">id</span></span>|<span data-ttu-id="69f16-133">String</span><span class="sxs-lookup"><span data-stu-id="69f16-133">String</span></span>|<span data-ttu-id="69f16-134">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="69f16-134">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="69f16-135">availableVersion</span><span class="sxs-lookup"><span data-stu-id="69f16-135">availableVersion</span></span>|<span data-ttu-id="69f16-136">String</span><span class="sxs-lookup"><span data-stu-id="69f16-136">String</span></span>|<span data-ttu-id="69f16-137">Windows 管理应用程序的可用版本。</span><span class="sxs-lookup"><span data-stu-id="69f16-137">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="69f16-138">响应</span><span class="sxs-lookup"><span data-stu-id="69f16-138">Response</span></span>
<span data-ttu-id="69f16-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69f16-139">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f16-140">示例</span><span class="sxs-lookup"><span data-stu-id="69f16-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f16-141">请求</span><span class="sxs-lookup"><span data-stu-id="69f16-141">Request</span></span>
<span data-ttu-id="69f16-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69f16-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="69f16-143">响应</span><span class="sxs-lookup"><span data-stu-id="69f16-143">Response</span></span>
<span data-ttu-id="69f16-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69f16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```




