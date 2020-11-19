---
title: 更新组织
description: 更新 organization 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f677c8b235edc74996601d95c0e841b10bee9d82
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49305468"
---
# <a name="update-organization"></a><span data-ttu-id="d6d30-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="d6d30-103">Update organization</span></span>

<span data-ttu-id="d6d30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6d30-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6d30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d30-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6d30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d30-107">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6d30-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d30-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6d30-108">Prerequisites</span></span>
<span data-ttu-id="d6d30-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6d30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d30-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6d30-111">Permission type</span></span>|<span data-ttu-id="d6d30-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6d30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d30-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6d30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d30-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d30-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6d30-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6d30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6d30-116">Not supported.</span></span>|
|<span data-ttu-id="d6d30-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6d30-117">Application</span></span>|<span data-ttu-id="d6d30-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d30-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d30-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6d30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="d6d30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6d30-120">Request headers</span></span>
|<span data-ttu-id="d6d30-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6d30-121">Header</span></span>|<span data-ttu-id="d6d30-122">值</span><span class="sxs-lookup"><span data-stu-id="d6d30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6d30-123">Authorization</span></span>|<span data-ttu-id="d6d30-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6d30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d30-125">接受</span><span class="sxs-lookup"><span data-stu-id="d6d30-125">Accept</span></span>|<span data-ttu-id="d6d30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6d30-127">Request body</span></span>
<span data-ttu-id="d6d30-128">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6d30-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="d6d30-129">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6d30-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="d6d30-130">属性</span><span class="sxs-lookup"><span data-stu-id="d6d30-130">Property</span></span>|<span data-ttu-id="d6d30-131">类型</span><span class="sxs-lookup"><span data-stu-id="d6d30-131">Type</span></span>|<span data-ttu-id="d6d30-132">说明</span><span class="sxs-lookup"><span data-stu-id="d6d30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d30-133">id</span><span class="sxs-lookup"><span data-stu-id="d6d30-133">id</span></span>|<span data-ttu-id="d6d30-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d6d30-134">String</span></span>|<span data-ttu-id="d6d30-135">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="d6d30-135">The GUID for the object.</span></span>|
|<span data-ttu-id="d6d30-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="d6d30-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="d6d30-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="d6d30-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="d6d30-138">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="d6d30-138">Mobile device management authority.</span></span> <span data-ttu-id="d6d30-139">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="d6d30-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="d6d30-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="d6d30-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="d6d30-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="d6d30-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="d6d30-142">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="d6d30-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="d6d30-143">响应</span><span class="sxs-lookup"><span data-stu-id="d6d30-143">Response</span></span>
<span data-ttu-id="d6d30-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6d30-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d30-145">示例</span><span class="sxs-lookup"><span data-stu-id="d6d30-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d30-146">请求</span><span class="sxs-lookup"><span data-stu-id="d6d30-146">Request</span></span>
<span data-ttu-id="d6d30-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6d30-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6d30-148">响应</span><span class="sxs-lookup"><span data-stu-id="d6d30-148">Response</span></span>
<span data-ttu-id="d6d30-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6d30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




