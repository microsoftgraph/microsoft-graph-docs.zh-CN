---
title: 更新组织
description: 更新 organization 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d0aa91f64aca9bb82d44a22dce6b6e0b36d84199
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411272"
---
# <a name="update-organization"></a><span data-ttu-id="9d81e-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="9d81e-103">Update organization</span></span>

> <span data-ttu-id="9d81e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9d81e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9d81e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d81e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d81e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d81e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d81e-107">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d81e-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d81e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d81e-108">Prerequisites</span></span>
<span data-ttu-id="9d81e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9d81e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9d81e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d81e-111">Permission type</span></span>|<span data-ttu-id="9d81e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d81e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d81e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d81e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d81e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d81e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9d81e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d81e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d81e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d81e-116">Not supported.</span></span>|
|<span data-ttu-id="9d81e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d81e-117">Application</span></span>|<span data-ttu-id="9d81e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d81e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d81e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d81e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="9d81e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d81e-120">Request headers</span></span>
|<span data-ttu-id="9d81e-121">标头</span><span class="sxs-lookup"><span data-stu-id="9d81e-121">Header</span></span>|<span data-ttu-id="9d81e-122">值</span><span class="sxs-lookup"><span data-stu-id="9d81e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d81e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d81e-123">Authorization</span></span>|<span data-ttu-id="9d81e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d81e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d81e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d81e-125">Accept</span></span>|<span data-ttu-id="9d81e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d81e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d81e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d81e-127">Request body</span></span>
<span data-ttu-id="9d81e-128">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d81e-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="9d81e-129">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9d81e-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="9d81e-130">属性</span><span class="sxs-lookup"><span data-stu-id="9d81e-130">Property</span></span>|<span data-ttu-id="9d81e-131">类型</span><span class="sxs-lookup"><span data-stu-id="9d81e-131">Type</span></span>|<span data-ttu-id="9d81e-132">说明</span><span class="sxs-lookup"><span data-stu-id="9d81e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d81e-133">id</span><span class="sxs-lookup"><span data-stu-id="9d81e-133">id</span></span>|<span data-ttu-id="9d81e-134">String</span><span class="sxs-lookup"><span data-stu-id="9d81e-134">String</span></span>|<span data-ttu-id="9d81e-135">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="9d81e-135">The GUID for the object.</span></span>|
|<span data-ttu-id="9d81e-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="9d81e-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="9d81e-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="9d81e-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="9d81e-138">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="9d81e-138">Mobile device management authority.</span></span> <span data-ttu-id="9d81e-139">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="9d81e-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="9d81e-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="9d81e-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="9d81e-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="9d81e-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="9d81e-142">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="9d81e-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="9d81e-143">响应</span><span class="sxs-lookup"><span data-stu-id="9d81e-143">Response</span></span>
<span data-ttu-id="9d81e-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d81e-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d81e-145">示例</span><span class="sxs-lookup"><span data-stu-id="9d81e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d81e-146">请求</span><span class="sxs-lookup"><span data-stu-id="9d81e-146">Request</span></span>
<span data-ttu-id="9d81e-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d81e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d81e-148">响应</span><span class="sxs-lookup"><span data-stu-id="9d81e-148">Response</span></span>
<span data-ttu-id="9d81e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d81e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




