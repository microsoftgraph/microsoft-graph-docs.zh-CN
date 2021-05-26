---
title: 创建 chromeOSOnboardingSettings
description: 创建新的 chromeOSOnboardingSettings 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a359b9bd0f638e147af8119ee7ca07a27db0c2e8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665720"
---
# <a name="create-chromeosonboardingsettings"></a><span data-ttu-id="e08bc-103">创建 chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="e08bc-103">Create chromeOSOnboardingSettings</span></span>

<span data-ttu-id="e08bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e08bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e08bc-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e08bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e08bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e08bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e08bc-107">创建新的 [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e08bc-107">Create a new [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e08bc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e08bc-108">Prerequisites</span></span>
<span data-ttu-id="e08bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e08bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e08bc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e08bc-111">Permission type</span></span>|<span data-ttu-id="e08bc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e08bc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e08bc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e08bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e08bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e08bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e08bc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e08bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e08bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e08bc-116">Not supported.</span></span>|
|<span data-ttu-id="e08bc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e08bc-117">Application</span></span>|<span data-ttu-id="e08bc-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e08bc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e08bc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e08bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="e08bc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e08bc-120">Request headers</span></span>
|<span data-ttu-id="e08bc-121">标头</span><span class="sxs-lookup"><span data-stu-id="e08bc-121">Header</span></span>|<span data-ttu-id="e08bc-122">值</span><span class="sxs-lookup"><span data-stu-id="e08bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e08bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e08bc-123">Authorization</span></span>|<span data-ttu-id="e08bc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e08bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e08bc-125">接受</span><span class="sxs-lookup"><span data-stu-id="e08bc-125">Accept</span></span>|<span data-ttu-id="e08bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e08bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e08bc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e08bc-127">Request body</span></span>
<span data-ttu-id="e08bc-128">在请求正文中，提供 chromeOSOnboardingSettings 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e08bc-128">In the request body, supply a JSON representation for the chromeOSOnboardingSettings object.</span></span>

<span data-ttu-id="e08bc-129">下表显示创建 chromeOSOnboardingSettings 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e08bc-129">The following table shows the properties that are required when you create the chromeOSOnboardingSettings.</span></span>

|<span data-ttu-id="e08bc-130">属性</span><span class="sxs-lookup"><span data-stu-id="e08bc-130">Property</span></span>|<span data-ttu-id="e08bc-131">类型</span><span class="sxs-lookup"><span data-stu-id="e08bc-131">Type</span></span>|<span data-ttu-id="e08bc-132">说明</span><span class="sxs-lookup"><span data-stu-id="e08bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e08bc-133">id</span><span class="sxs-lookup"><span data-stu-id="e08bc-133">id</span></span>|<span data-ttu-id="e08bc-134">String</span><span class="sxs-lookup"><span data-stu-id="e08bc-134">String</span></span>|<span data-ttu-id="e08bc-135">ChromebookTenant 的 ID</span><span class="sxs-lookup"><span data-stu-id="e08bc-135">The ChromebookTenant's Id</span></span>|
|<span data-ttu-id="e08bc-136">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e08bc-136">ownerUserPrincipalName</span></span>|<span data-ttu-id="e08bc-137">String</span><span class="sxs-lookup"><span data-stu-id="e08bc-137">String</span></span>|<span data-ttu-id="e08bc-138">ChromebookTenant 的 OwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e08bc-138">The ChromebookTenant's OwnerUserPrincipalName</span></span>|
|<span data-ttu-id="e08bc-139">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="e08bc-139">onboardingStatus</span></span>|[<span data-ttu-id="e08bc-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="e08bc-140">onboardingStatus</span></span>](../resources/intune-chromebooksync-onboardingstatus.md)|<span data-ttu-id="e08bc-141">ChromebookTenant 的 OnboardingStatus。</span><span class="sxs-lookup"><span data-stu-id="e08bc-141">The ChromebookTenant's OnboardingStatus.</span></span> <span data-ttu-id="e08bc-142">可取值为：`unknown`、`inprogress`、`onboarded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="e08bc-142">Possible values are: `unknown`, `inprogress`, `onboarded`, `failed`.</span></span>|
|<span data-ttu-id="e08bc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e08bc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e08bc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e08bc-144">DateTimeOffset</span></span>|<span data-ttu-id="e08bc-145">ChromebookTenant 的 LastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e08bc-145">The ChromebookTenant's LastModifiedDateTime</span></span>|
|<span data-ttu-id="e08bc-146">lastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e08bc-146">lastDirectorySyncDateTime</span></span>|<span data-ttu-id="e08bc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e08bc-147">DateTimeOffset</span></span>|<span data-ttu-id="e08bc-148">ChromebookTenant 的 LastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e08bc-148">The ChromebookTenant's LastDirectorySyncDateTime</span></span>|



## <a name="response"></a><span data-ttu-id="e08bc-149">响应</span><span class="sxs-lookup"><span data-stu-id="e08bc-149">Response</span></span>
<span data-ttu-id="e08bc-150">如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e08bc-150">If successful, this method returns a `201 Created` response code and a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e08bc-151">示例</span><span class="sxs-lookup"><span data-stu-id="e08bc-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e08bc-152">请求</span><span class="sxs-lookup"><span data-stu-id="e08bc-152">Request</span></span>
<span data-ttu-id="e08bc-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e08bc-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e08bc-154">响应</span><span class="sxs-lookup"><span data-stu-id="e08bc-154">Response</span></span>
<span data-ttu-id="e08bc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e08bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "0344255d-255d-0344-5d25-44035d254403",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```




