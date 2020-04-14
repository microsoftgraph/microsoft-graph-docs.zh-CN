---
title: 更新组织
description: 更新 organization 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99bafa9aa4098700376a6281af359dfb02c77de1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463143"
---
# <a name="update-organization"></a><span data-ttu-id="2adaf-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="2adaf-103">Update organization</span></span>

<span data-ttu-id="2adaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2adaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2adaf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2adaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2adaf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2adaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2adaf-107">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2adaf-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2adaf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2adaf-108">Prerequisites</span></span>
<span data-ttu-id="2adaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2adaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2adaf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2adaf-111">Permission type</span></span>|<span data-ttu-id="2adaf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2adaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2adaf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2adaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2adaf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2adaf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2adaf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2adaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2adaf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2adaf-116">Not supported.</span></span>|
|<span data-ttu-id="2adaf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2adaf-117">Application</span></span>|<span data-ttu-id="2adaf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2adaf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2adaf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2adaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="2adaf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2adaf-120">Request headers</span></span>
|<span data-ttu-id="2adaf-121">标头</span><span class="sxs-lookup"><span data-stu-id="2adaf-121">Header</span></span>|<span data-ttu-id="2adaf-122">值</span><span class="sxs-lookup"><span data-stu-id="2adaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2adaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2adaf-123">Authorization</span></span>|<span data-ttu-id="2adaf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2adaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2adaf-125">接受</span><span class="sxs-lookup"><span data-stu-id="2adaf-125">Accept</span></span>|<span data-ttu-id="2adaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2adaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2adaf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2adaf-127">Request body</span></span>
<span data-ttu-id="2adaf-128">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2adaf-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="2adaf-129">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2adaf-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="2adaf-130">属性</span><span class="sxs-lookup"><span data-stu-id="2adaf-130">Property</span></span>|<span data-ttu-id="2adaf-131">类型</span><span class="sxs-lookup"><span data-stu-id="2adaf-131">Type</span></span>|<span data-ttu-id="2adaf-132">说明</span><span class="sxs-lookup"><span data-stu-id="2adaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2adaf-133">id</span><span class="sxs-lookup"><span data-stu-id="2adaf-133">id</span></span>|<span data-ttu-id="2adaf-134">String</span><span class="sxs-lookup"><span data-stu-id="2adaf-134">String</span></span>|<span data-ttu-id="2adaf-135">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="2adaf-135">The GUID for the object.</span></span>|
|<span data-ttu-id="2adaf-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="2adaf-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="2adaf-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="2adaf-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="2adaf-138">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="2adaf-138">Mobile device management authority.</span></span> <span data-ttu-id="2adaf-139">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="2adaf-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="2adaf-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="2adaf-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="2adaf-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="2adaf-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="2adaf-142">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="2adaf-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="2adaf-143">响应</span><span class="sxs-lookup"><span data-stu-id="2adaf-143">Response</span></span>
<span data-ttu-id="2adaf-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2adaf-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2adaf-145">示例</span><span class="sxs-lookup"><span data-stu-id="2adaf-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="2adaf-146">请求</span><span class="sxs-lookup"><span data-stu-id="2adaf-146">Request</span></span>
<span data-ttu-id="2adaf-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2adaf-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```

### <a name="response"></a><span data-ttu-id="2adaf-148">响应</span><span class="sxs-lookup"><span data-stu-id="2adaf-148">Response</span></span>
<span data-ttu-id="2adaf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2adaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```



