---
title: 更新组织
description: 更新 organization 对象的属性。
ms.openlocfilehash: 50167db2c2078421894fa86d7b24c0b93351616c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010777"
---
# <a name="update-organization"></a><span data-ttu-id="45f3a-103">更新 organization</span><span class="sxs-lookup"><span data-stu-id="45f3a-103">Update organization</span></span>

> <span data-ttu-id="45f3a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45f3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45f3a-105">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="45f3a-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45f3a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="45f3a-106">Prerequisites</span></span>
<span data-ttu-id="45f3a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="45f3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45f3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45f3a-109">Permission type</span></span>|<span data-ttu-id="45f3a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45f3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45f3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45f3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45f3a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f3a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45f3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45f3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45f3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45f3a-114">Not supported.</span></span>|
|<span data-ttu-id="45f3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45f3a-115">Application</span></span>|<span data-ttu-id="45f3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45f3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45f3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45f3a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="45f3a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="45f3a-118">Request headers</span></span>
|<span data-ttu-id="45f3a-119">标头</span><span class="sxs-lookup"><span data-stu-id="45f3a-119">Header</span></span>|<span data-ttu-id="45f3a-120">值</span><span class="sxs-lookup"><span data-stu-id="45f3a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45f3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45f3a-121">Authorization</span></span>|<span data-ttu-id="45f3a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45f3a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45f3a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="45f3a-123">Accept</span></span>|<span data-ttu-id="45f3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45f3a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45f3a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="45f3a-125">Request body</span></span>
<span data-ttu-id="45f3a-126">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45f3a-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="45f3a-127">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="45f3a-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="45f3a-128">属性</span><span class="sxs-lookup"><span data-stu-id="45f3a-128">Property</span></span>|<span data-ttu-id="45f3a-129">类型</span><span class="sxs-lookup"><span data-stu-id="45f3a-129">Type</span></span>|<span data-ttu-id="45f3a-130">说明</span><span class="sxs-lookup"><span data-stu-id="45f3a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f3a-131">id</span><span class="sxs-lookup"><span data-stu-id="45f3a-131">id</span></span>|<span data-ttu-id="45f3a-132">String</span><span class="sxs-lookup"><span data-stu-id="45f3a-132">String</span></span>|<span data-ttu-id="45f3a-133">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="45f3a-133">The GUID for the object.</span></span>|
|<span data-ttu-id="45f3a-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="45f3a-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="45f3a-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="45f3a-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="45f3a-136">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="45f3a-136">Mobile device management authority.</span></span> <span data-ttu-id="45f3a-137">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="45f3a-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="45f3a-138">响应</span><span class="sxs-lookup"><span data-stu-id="45f3a-138">Response</span></span>
<span data-ttu-id="45f3a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45f3a-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45f3a-140">示例</span><span class="sxs-lookup"><span data-stu-id="45f3a-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="45f3a-141">请求</span><span class="sxs-lookup"><span data-stu-id="45f3a-141">Request</span></span>
<span data-ttu-id="45f3a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45f3a-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="45f3a-143">响应</span><span class="sxs-lookup"><span data-stu-id="45f3a-143">Response</span></span>
<span data-ttu-id="45f3a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45f3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



