---
title: 更新 chromeOSOnboardingSettings
description: 更新 chromeOSOnboardingSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67d1d84e51500a5b3ade7dda7af2bdf4bdeb71f9
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611792"
---
# <a name="update-chromeosonboardingsettings"></a><span data-ttu-id="b0eae-103">更新 chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b0eae-103">Update chromeOSOnboardingSettings</span></span>

<span data-ttu-id="b0eae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0eae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0eae-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0eae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0eae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0eae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0eae-107">更新 [chromeOSOnboardingSettings 对象](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b0eae-107">Update the properties of a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0eae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0eae-108">Prerequisites</span></span>
<span data-ttu-id="b0eae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0eae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0eae-111">Permission type</span></span>|<span data-ttu-id="b0eae-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0eae-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0eae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0eae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0eae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0eae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0eae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0eae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0eae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0eae-116">Not supported.</span></span>|
|<span data-ttu-id="b0eae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0eae-117">Application</span></span>|<span data-ttu-id="b0eae-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0eae-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0eae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0eae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/chromeOSOnboardingSettings/{chromeOSOnboardingSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="b0eae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0eae-120">Request headers</span></span>
|<span data-ttu-id="b0eae-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0eae-121">Header</span></span>|<span data-ttu-id="b0eae-122">值</span><span class="sxs-lookup"><span data-stu-id="b0eae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0eae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0eae-123">Authorization</span></span>|<span data-ttu-id="b0eae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0eae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0eae-125">接受</span><span class="sxs-lookup"><span data-stu-id="b0eae-125">Accept</span></span>|<span data-ttu-id="b0eae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0eae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0eae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0eae-127">Request body</span></span>
<span data-ttu-id="b0eae-128">在请求正文中，提供 [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0eae-128">In the request body, supply a JSON representation for the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

<span data-ttu-id="b0eae-129">下表显示创建 [chromeOSOnboardingSettings 时所需的属性](../resources/intune-chromebooksync-chromeosonboardingsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="b0eae-129">The following table shows the properties that are required when you create the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md).</span></span>

|<span data-ttu-id="b0eae-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0eae-130">Property</span></span>|<span data-ttu-id="b0eae-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0eae-131">Type</span></span>|<span data-ttu-id="b0eae-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0eae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0eae-133">id</span><span class="sxs-lookup"><span data-stu-id="b0eae-133">id</span></span>|<span data-ttu-id="b0eae-134">String</span><span class="sxs-lookup"><span data-stu-id="b0eae-134">String</span></span>|<span data-ttu-id="b0eae-135">ChromebookTenant 的 ID</span><span class="sxs-lookup"><span data-stu-id="b0eae-135">The ChromebookTenant's Id</span></span>|
|<span data-ttu-id="b0eae-136">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0eae-136">ownerUserPrincipalName</span></span>|<span data-ttu-id="b0eae-137">String</span><span class="sxs-lookup"><span data-stu-id="b0eae-137">String</span></span>|<span data-ttu-id="b0eae-138">ChromebookTenant 的 OwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0eae-138">The ChromebookTenant's OwnerUserPrincipalName</span></span>|
|<span data-ttu-id="b0eae-139">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b0eae-139">onboardingStatus</span></span>|[<span data-ttu-id="b0eae-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b0eae-140">onboardingStatus</span></span>](../resources/intune-chromebooksync-onboardingstatus.md)|<span data-ttu-id="b0eae-141">ChromebookTenant 的 OnboardingStatus。</span><span class="sxs-lookup"><span data-stu-id="b0eae-141">The ChromebookTenant's OnboardingStatus.</span></span> <span data-ttu-id="b0eae-142">可取值为：`unknown`、`inprogress`、`onboarded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b0eae-142">Possible values are: `unknown`, `inprogress`, `onboarded`, `failed`.</span></span>|
|<span data-ttu-id="b0eae-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0eae-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b0eae-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0eae-144">DateTimeOffset</span></span>|<span data-ttu-id="b0eae-145">ChromebookTenant 的 LastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0eae-145">The ChromebookTenant's LastModifiedDateTime</span></span>|
|<span data-ttu-id="b0eae-146">lastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b0eae-146">lastDirectorySyncDateTime</span></span>|<span data-ttu-id="b0eae-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0eae-147">DateTimeOffset</span></span>|<span data-ttu-id="b0eae-148">ChromebookTenant 的 LastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b0eae-148">The ChromebookTenant's LastDirectorySyncDateTime</span></span>|



## <a name="response"></a><span data-ttu-id="b0eae-149">响应</span><span class="sxs-lookup"><span data-stu-id="b0eae-149">Response</span></span>
<span data-ttu-id="b0eae-150">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0eae-150">If successful, this method returns a `200 OK` response code and an updated [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0eae-151">示例</span><span class="sxs-lookup"><span data-stu-id="b0eae-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0eae-152">请求</span><span class="sxs-lookup"><span data-stu-id="b0eae-152">Request</span></span>
<span data-ttu-id="b0eae-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0eae-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings/{chromeOSOnboardingSettingsId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b0eae-154">响应</span><span class="sxs-lookup"><span data-stu-id="b0eae-154">Response</span></span>
<span data-ttu-id="b0eae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0eae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




