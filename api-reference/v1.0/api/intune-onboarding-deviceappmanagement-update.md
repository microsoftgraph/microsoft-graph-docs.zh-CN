---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc443e6f6d99a220c9e5b9a3bc88cd4cf30ec013
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759485"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="1ba38-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="1ba38-103">Update deviceAppManagement</span></span>

<span data-ttu-id="1ba38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ba38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ba38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ba38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ba38-106">更新 [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba38-106">Update the properties of a [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ba38-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ba38-107">Prerequisites</span></span>
<span data-ttu-id="1ba38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ba38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba38-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ba38-110">Permission type</span></span>|<span data-ttu-id="1ba38-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ba38-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ba38-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ba38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ba38-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba38-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ba38-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ba38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ba38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ba38-115">Not supported.</span></span>|
|<span data-ttu-id="1ba38-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ba38-116">Application</span></span>|<span data-ttu-id="1ba38-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba38-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ba38-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ba38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="1ba38-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ba38-119">Request headers</span></span>
|<span data-ttu-id="1ba38-120">标头</span><span class="sxs-lookup"><span data-stu-id="1ba38-120">Header</span></span>|<span data-ttu-id="1ba38-121">值</span><span class="sxs-lookup"><span data-stu-id="1ba38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ba38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba38-122">Authorization</span></span>|<span data-ttu-id="1ba38-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ba38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ba38-124">接受</span><span class="sxs-lookup"><span data-stu-id="1ba38-124">Accept</span></span>|<span data-ttu-id="1ba38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ba38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ba38-126">Request body</span></span>
<span data-ttu-id="1ba38-127">在请求正文中，提供 [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ba38-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="1ba38-128">下表显示创建 [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba38-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span></span>

|<span data-ttu-id="1ba38-129">属性</span><span class="sxs-lookup"><span data-stu-id="1ba38-129">Property</span></span>|<span data-ttu-id="1ba38-130">类型</span><span class="sxs-lookup"><span data-stu-id="1ba38-130">Type</span></span>|<span data-ttu-id="1ba38-131">说明</span><span class="sxs-lookup"><span data-stu-id="1ba38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ba38-132">id</span><span class="sxs-lookup"><span data-stu-id="1ba38-132">id</span></span>|<span data-ttu-id="1ba38-133">String</span><span class="sxs-lookup"><span data-stu-id="1ba38-133">String</span></span>|<span data-ttu-id="1ba38-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1ba38-134">Not yet documented</span></span>|
|<span data-ttu-id="1ba38-135">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1ba38-135">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1ba38-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ba38-136">DateTimeOffset</span></span>|<span data-ttu-id="1ba38-137">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="1ba38-137">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="1ba38-138">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="1ba38-138">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="1ba38-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba38-139">Boolean</span></span>|<span data-ttu-id="1ba38-140">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ba38-140">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="1ba38-141">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="1ba38-141">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="1ba38-142">String</span><span class="sxs-lookup"><span data-stu-id="1ba38-142">String</span></span>|<span data-ttu-id="1ba38-143">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="1ba38-143">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="1ba38-144">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="1ba38-144">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="1ba38-145">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1ba38-145">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="1ba38-146">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="1ba38-146">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="1ba38-147">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="1ba38-147">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="1ba38-148">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="1ba38-148">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="1ba38-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ba38-149">DateTimeOffset</span></span>|<span data-ttu-id="1ba38-150">上次完成从适用于企业的 Microsoft Store 的应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="1ba38-150">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="1ba38-151">响应</span><span class="sxs-lookup"><span data-stu-id="1ba38-151">Response</span></span>
<span data-ttu-id="1ba38-152">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ba38-152">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ba38-153">示例</span><span class="sxs-lookup"><span data-stu-id="1ba38-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ba38-154">请求</span><span class="sxs-lookup"><span data-stu-id="1ba38-154">Request</span></span>
<span data-ttu-id="1ba38-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ba38-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 394

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1ba38-156">响应</span><span class="sxs-lookup"><span data-stu-id="1ba38-156">Response</span></span>
<span data-ttu-id="1ba38-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ba38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```




