---
title: 更新组织
description: 更新 organization 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b66eea4b04f21f85aa38b9777a17cb73e87fe6fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751459"
---
# <a name="update-organization"></a><span data-ttu-id="3b091-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="3b091-103">Update organization</span></span>

<span data-ttu-id="3b091-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b091-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b091-106">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b091-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b091-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b091-107">Prerequisites</span></span>
<span data-ttu-id="3b091-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b091-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b091-110">Permission type</span></span>|<span data-ttu-id="3b091-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b091-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b091-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b091-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b091-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b091-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b091-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b091-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b091-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b091-115">Not supported.</span></span>|
|<span data-ttu-id="3b091-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b091-116">Application</span></span>|<span data-ttu-id="3b091-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b091-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b091-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b091-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="3b091-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b091-119">Request headers</span></span>
|<span data-ttu-id="3b091-120">标头</span><span class="sxs-lookup"><span data-stu-id="3b091-120">Header</span></span>|<span data-ttu-id="3b091-121">值</span><span class="sxs-lookup"><span data-stu-id="3b091-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b091-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b091-122">Authorization</span></span>|<span data-ttu-id="3b091-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b091-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b091-124">接受</span><span class="sxs-lookup"><span data-stu-id="3b091-124">Accept</span></span>|<span data-ttu-id="3b091-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b091-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b091-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b091-126">Request body</span></span>
<span data-ttu-id="3b091-127">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b091-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="3b091-128">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b091-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="3b091-129">属性</span><span class="sxs-lookup"><span data-stu-id="3b091-129">Property</span></span>|<span data-ttu-id="3b091-130">类型</span><span class="sxs-lookup"><span data-stu-id="3b091-130">Type</span></span>|<span data-ttu-id="3b091-131">说明</span><span class="sxs-lookup"><span data-stu-id="3b091-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b091-132">id</span><span class="sxs-lookup"><span data-stu-id="3b091-132">id</span></span>|<span data-ttu-id="3b091-133">String</span><span class="sxs-lookup"><span data-stu-id="3b091-133">String</span></span>|<span data-ttu-id="3b091-134">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="3b091-134">The GUID for the object.</span></span>|
|<span data-ttu-id="3b091-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="3b091-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="3b091-136">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="3b091-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="3b091-137">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="3b091-137">Mobile device management authority.</span></span> <span data-ttu-id="3b091-138">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="3b091-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="3b091-139">响应</span><span class="sxs-lookup"><span data-stu-id="3b091-139">Response</span></span>
<span data-ttu-id="3b091-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b091-140">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b091-141">示例</span><span class="sxs-lookup"><span data-stu-id="3b091-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b091-142">请求</span><span class="sxs-lookup"><span data-stu-id="3b091-142">Request</span></span>
<span data-ttu-id="3b091-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b091-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="3b091-144">响应</span><span class="sxs-lookup"><span data-stu-id="3b091-144">Response</span></span>
<span data-ttu-id="3b091-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b091-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```




