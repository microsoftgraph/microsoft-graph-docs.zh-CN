---
title: 更新 windowsManagementApp
description: 更新 windowsManagementApp 对象的属性。
author: tfitzmac
ms.openlocfilehash: 4e14dc250167fed09969cea82b8291ce4bd9bf97
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337518"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="cb6dc-103">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="cb6dc-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="cb6dc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb6dc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb6dc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb6dc-107">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb6dc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb6dc-108">Prerequisites</span></span>
<span data-ttu-id="cb6dc-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cb6dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb6dc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb6dc-111">Permission type</span></span>|<span data-ttu-id="cb6dc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb6dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb6dc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb6dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb6dc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6dc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb6dc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb6dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb6dc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-116">Not supported.</span></span>|
|<span data-ttu-id="cb6dc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb6dc-117">Application</span></span>|<span data-ttu-id="cb6dc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb6dc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb6dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="cb6dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb6dc-120">Request headers</span></span>
|<span data-ttu-id="cb6dc-121">标头</span><span class="sxs-lookup"><span data-stu-id="cb6dc-121">Header</span></span>|<span data-ttu-id="cb6dc-122">值</span><span class="sxs-lookup"><span data-stu-id="cb6dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb6dc-123">授权</span><span class="sxs-lookup"><span data-stu-id="cb6dc-123">Authorization</span></span>|<span data-ttu-id="cb6dc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb6dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb6dc-125">Accept</span></span>|<span data-ttu-id="cb6dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb6dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb6dc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb6dc-127">Request body</span></span>
<span data-ttu-id="cb6dc-128">在请求正文中，提供[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="cb6dc-129">下表显示时创建[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="cb6dc-130">属性</span><span class="sxs-lookup"><span data-stu-id="cb6dc-130">Property</span></span>|<span data-ttu-id="cb6dc-131">类型</span><span class="sxs-lookup"><span data-stu-id="cb6dc-131">Type</span></span>|<span data-ttu-id="cb6dc-132">说明</span><span class="sxs-lookup"><span data-stu-id="cb6dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6dc-133">id</span><span class="sxs-lookup"><span data-stu-id="cb6dc-133">id</span></span>|<span data-ttu-id="cb6dc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cb6dc-134">String</span></span>|<span data-ttu-id="cb6dc-135">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cb6dc-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="cb6dc-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="cb6dc-136">availableVersion</span></span>|<span data-ttu-id="cb6dc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="cb6dc-137">String</span></span>|<span data-ttu-id="cb6dc-138">Windows 管理应用程序可用版本。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="cb6dc-139">响应</span><span class="sxs-lookup"><span data-stu-id="cb6dc-139">Response</span></span>
<span data-ttu-id="cb6dc-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb6dc-141">示例</span><span class="sxs-lookup"><span data-stu-id="cb6dc-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb6dc-142">请求</span><span class="sxs-lookup"><span data-stu-id="cb6dc-142">Request</span></span>
<span data-ttu-id="cb6dc-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 53

{
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="cb6dc-144">响应</span><span class="sxs-lookup"><span data-stu-id="cb6dc-144">Response</span></span>
<span data-ttu-id="cb6dc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb6dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





