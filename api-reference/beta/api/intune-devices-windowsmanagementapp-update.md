---
title: 更新 windowsManagementApp
description: 更新 windowsManagementApp 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27ba9154598480972e1d7f2c9a8b5d28bb3ec4b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412406"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="b42d8-103">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="b42d8-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="b42d8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b42d8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b42d8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b42d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b42d8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b42d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b42d8-107">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b42d8-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b42d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b42d8-108">Prerequisites</span></span>
<span data-ttu-id="b42d8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b42d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b42d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b42d8-111">Permission type</span></span>|<span data-ttu-id="b42d8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b42d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b42d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b42d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b42d8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b42d8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b42d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b42d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b42d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b42d8-116">Not supported.</span></span>|
|<span data-ttu-id="b42d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b42d8-117">Application</span></span>|<span data-ttu-id="b42d8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b42d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b42d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b42d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="b42d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b42d8-120">Request headers</span></span>
|<span data-ttu-id="b42d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="b42d8-121">Header</span></span>|<span data-ttu-id="b42d8-122">值</span><span class="sxs-lookup"><span data-stu-id="b42d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b42d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b42d8-123">Authorization</span></span>|<span data-ttu-id="b42d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b42d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b42d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b42d8-125">Accept</span></span>|<span data-ttu-id="b42d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b42d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b42d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b42d8-127">Request body</span></span>
<span data-ttu-id="b42d8-128">在请求正文中，提供[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b42d8-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="b42d8-129">下表显示时创建[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b42d8-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="b42d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="b42d8-130">Property</span></span>|<span data-ttu-id="b42d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="b42d8-131">Type</span></span>|<span data-ttu-id="b42d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="b42d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b42d8-133">id</span><span class="sxs-lookup"><span data-stu-id="b42d8-133">id</span></span>|<span data-ttu-id="b42d8-134">String</span><span class="sxs-lookup"><span data-stu-id="b42d8-134">String</span></span>|<span data-ttu-id="b42d8-135">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b42d8-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="b42d8-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="b42d8-136">availableVersion</span></span>|<span data-ttu-id="b42d8-137">String</span><span class="sxs-lookup"><span data-stu-id="b42d8-137">String</span></span>|<span data-ttu-id="b42d8-138">Windows 管理应用程序可用版本。</span><span class="sxs-lookup"><span data-stu-id="b42d8-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="b42d8-139">响应</span><span class="sxs-lookup"><span data-stu-id="b42d8-139">Response</span></span>
<span data-ttu-id="b42d8-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b42d8-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b42d8-141">示例</span><span class="sxs-lookup"><span data-stu-id="b42d8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b42d8-142">请求</span><span class="sxs-lookup"><span data-stu-id="b42d8-142">Request</span></span>
<span data-ttu-id="b42d8-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b42d8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="b42d8-144">响应</span><span class="sxs-lookup"><span data-stu-id="b42d8-144">Response</span></span>
<span data-ttu-id="b42d8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b42d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




