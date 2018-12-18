---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: tfitzmac
ms.openlocfilehash: c5fc5159af1493fac1e8f280c899914edfd490b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309378"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="b2f77-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="b2f77-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="b2f77-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b2f77-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2f77-105">更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b2f77-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2f77-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2f77-106">Prerequisites</span></span>
<span data-ttu-id="b2f77-107">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b2f77-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b2f77-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2f77-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b2f77-109">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="b2f77-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b2f77-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2f77-110">Permission type</span></span>|<span data-ttu-id="b2f77-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2f77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2f77-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2f77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2f77-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2f77-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2f77-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2f77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2f77-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2f77-115">Not supported.</span></span>|
|<span data-ttu-id="b2f77-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2f77-116">Application</span></span>|<span data-ttu-id="b2f77-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2f77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2f77-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2f77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="b2f77-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2f77-119">Request headers</span></span>
|<span data-ttu-id="b2f77-120">标头</span><span class="sxs-lookup"><span data-stu-id="b2f77-120">Header</span></span>|<span data-ttu-id="b2f77-121">值</span><span class="sxs-lookup"><span data-stu-id="b2f77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2f77-122">授权</span><span class="sxs-lookup"><span data-stu-id="b2f77-122">Authorization</span></span>|<span data-ttu-id="b2f77-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2f77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2f77-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2f77-124">Accept</span></span>|<span data-ttu-id="b2f77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2f77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2f77-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2f77-126">Request body</span></span>
<span data-ttu-id="b2f77-127">在请求正文中，提供 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2f77-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="b2f77-128">下表显示创建 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2f77-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="b2f77-129">属性</span><span class="sxs-lookup"><span data-stu-id="b2f77-129">Property</span></span>|<span data-ttu-id="b2f77-130">类型</span><span class="sxs-lookup"><span data-stu-id="b2f77-130">Type</span></span>|<span data-ttu-id="b2f77-131">说明</span><span class="sxs-lookup"><span data-stu-id="b2f77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f77-132">id</span><span class="sxs-lookup"><span data-stu-id="b2f77-132">id</span></span>|<span data-ttu-id="b2f77-133">String</span><span class="sxs-lookup"><span data-stu-id="b2f77-133">String</span></span>|<span data-ttu-id="b2f77-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b2f77-134">Key of the entity.</span></span>|
|<span data-ttu-id="b2f77-135">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="b2f77-135">**Onboarding**</span></span>|
|<span data-ttu-id="b2f77-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="b2f77-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="b2f77-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2f77-137">Boolean</span></span>|<span data-ttu-id="b2f77-138">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="b2f77-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="b2f77-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="b2f77-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="b2f77-140">String</span><span class="sxs-lookup"><span data-stu-id="b2f77-140">String</span></span>|<span data-ttu-id="b2f77-141">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="b2f77-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="b2f77-142">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="b2f77-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="b2f77-143">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b2f77-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="b2f77-144">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="b2f77-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="b2f77-145">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="b2f77-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="b2f77-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="b2f77-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="b2f77-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2f77-147">DateTimeOffset</span></span>|<span data-ttu-id="b2f77-148">从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。</span><span class="sxs-lookup"><span data-stu-id="b2f77-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="b2f77-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b2f77-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b2f77-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2f77-150">DateTimeOffset</span></span>|<span data-ttu-id="b2f77-151">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="b2f77-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="b2f77-152">响应</span><span class="sxs-lookup"><span data-stu-id="b2f77-152">Response</span></span>
<span data-ttu-id="b2f77-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2f77-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="b2f77-154">示例请求</span><span class="sxs-lookup"><span data-stu-id="b2f77-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="b2f77-155">响应示例</span><span class="sxs-lookup"><span data-stu-id="b2f77-155">Example response</span></span>

<span data-ttu-id="b2f77-156">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="b2f77-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2f77-157">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2f77-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



