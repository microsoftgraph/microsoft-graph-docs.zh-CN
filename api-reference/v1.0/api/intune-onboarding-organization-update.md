---
title: 更新组织
description: 更新 organization 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 195aac351138cc133fbb48877b2e68d27a77954f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024026"
---
# <a name="update-organization"></a><span data-ttu-id="0683a-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="0683a-103">Update organization</span></span>

> <span data-ttu-id="0683a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0683a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0683a-105">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0683a-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0683a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0683a-106">Prerequisites</span></span>
<span data-ttu-id="0683a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0683a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0683a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0683a-109">Permission type</span></span>|<span data-ttu-id="0683a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0683a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0683a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0683a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0683a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0683a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0683a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0683a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0683a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0683a-114">Not supported.</span></span>|
|<span data-ttu-id="0683a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0683a-115">Application</span></span>|<span data-ttu-id="0683a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0683a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0683a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0683a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="0683a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0683a-118">Request headers</span></span>
|<span data-ttu-id="0683a-119">标头</span><span class="sxs-lookup"><span data-stu-id="0683a-119">Header</span></span>|<span data-ttu-id="0683a-120">值</span><span class="sxs-lookup"><span data-stu-id="0683a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0683a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0683a-121">Authorization</span></span>|<span data-ttu-id="0683a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0683a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0683a-123">接受</span><span class="sxs-lookup"><span data-stu-id="0683a-123">Accept</span></span>|<span data-ttu-id="0683a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0683a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0683a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0683a-125">Request body</span></span>
<span data-ttu-id="0683a-126">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0683a-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="0683a-127">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0683a-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="0683a-128">属性</span><span class="sxs-lookup"><span data-stu-id="0683a-128">Property</span></span>|<span data-ttu-id="0683a-129">类型</span><span class="sxs-lookup"><span data-stu-id="0683a-129">Type</span></span>|<span data-ttu-id="0683a-130">说明</span><span class="sxs-lookup"><span data-stu-id="0683a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0683a-131">id</span><span class="sxs-lookup"><span data-stu-id="0683a-131">id</span></span>|<span data-ttu-id="0683a-132">String</span><span class="sxs-lookup"><span data-stu-id="0683a-132">String</span></span>|<span data-ttu-id="0683a-133">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="0683a-133">The GUID for the object.</span></span>|
|<span data-ttu-id="0683a-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="0683a-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="0683a-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="0683a-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="0683a-136">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="0683a-136">Mobile device management authority.</span></span> <span data-ttu-id="0683a-137">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="0683a-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="0683a-138">响应</span><span class="sxs-lookup"><span data-stu-id="0683a-138">Response</span></span>
<span data-ttu-id="0683a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0683a-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0683a-140">示例</span><span class="sxs-lookup"><span data-stu-id="0683a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0683a-141">请求</span><span class="sxs-lookup"><span data-stu-id="0683a-141">Request</span></span>
<span data-ttu-id="0683a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0683a-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="0683a-143">响应</span><span class="sxs-lookup"><span data-stu-id="0683a-143">Response</span></span>
<span data-ttu-id="0683a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0683a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



