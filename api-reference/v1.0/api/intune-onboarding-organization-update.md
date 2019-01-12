---
title: 更新组织
description: 更新 organization 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 023bc7bdedfce2fc18784cd027bc0f041d7b8527
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928974"
---
# <a name="update-organization"></a><span data-ttu-id="575bc-103">更新 organization</span><span class="sxs-lookup"><span data-stu-id="575bc-103">Update organization</span></span>

> <span data-ttu-id="575bc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="575bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="575bc-105">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="575bc-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="575bc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="575bc-106">Prerequisites</span></span>
<span data-ttu-id="575bc-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="575bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="575bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="575bc-109">Permission type</span></span>|<span data-ttu-id="575bc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="575bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="575bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="575bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="575bc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="575bc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="575bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="575bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="575bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="575bc-114">Not supported.</span></span>|
|<span data-ttu-id="575bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="575bc-115">Application</span></span>|<span data-ttu-id="575bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="575bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="575bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="575bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="575bc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="575bc-118">Request headers</span></span>
|<span data-ttu-id="575bc-119">标头</span><span class="sxs-lookup"><span data-stu-id="575bc-119">Header</span></span>|<span data-ttu-id="575bc-120">值</span><span class="sxs-lookup"><span data-stu-id="575bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="575bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="575bc-121">Authorization</span></span>|<span data-ttu-id="575bc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="575bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="575bc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="575bc-123">Accept</span></span>|<span data-ttu-id="575bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="575bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="575bc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="575bc-125">Request body</span></span>
<span data-ttu-id="575bc-126">在请求正文中，提供 [organization](../resources/intune-onboarding-organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="575bc-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="575bc-127">下表显示创建 [organization](../resources/intune-onboarding-organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="575bc-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="575bc-128">属性</span><span class="sxs-lookup"><span data-stu-id="575bc-128">Property</span></span>|<span data-ttu-id="575bc-129">类型</span><span class="sxs-lookup"><span data-stu-id="575bc-129">Type</span></span>|<span data-ttu-id="575bc-130">说明</span><span class="sxs-lookup"><span data-stu-id="575bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="575bc-131">id</span><span class="sxs-lookup"><span data-stu-id="575bc-131">id</span></span>|<span data-ttu-id="575bc-132">String</span><span class="sxs-lookup"><span data-stu-id="575bc-132">String</span></span>|<span data-ttu-id="575bc-133">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="575bc-133">The GUID for the object.</span></span>|
|<span data-ttu-id="575bc-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="575bc-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="575bc-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="575bc-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="575bc-136">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="575bc-136">Mobile device management authority.</span></span> <span data-ttu-id="575bc-137">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="575bc-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="575bc-138">响应</span><span class="sxs-lookup"><span data-stu-id="575bc-138">Response</span></span>
<span data-ttu-id="575bc-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune-onboarding-organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="575bc-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="575bc-140">示例</span><span class="sxs-lookup"><span data-stu-id="575bc-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="575bc-141">请求</span><span class="sxs-lookup"><span data-stu-id="575bc-141">Request</span></span>
<span data-ttu-id="575bc-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="575bc-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="575bc-143">响应</span><span class="sxs-lookup"><span data-stu-id="575bc-143">Response</span></span>
<span data-ttu-id="575bc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="575bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



