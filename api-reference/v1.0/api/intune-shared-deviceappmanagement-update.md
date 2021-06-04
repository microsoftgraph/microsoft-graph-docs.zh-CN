---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 419bdc52dd9dbc7b67528b4a8b109bb309547f95
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732438"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="cd181-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="cd181-103">Update deviceAppManagement</span></span>

<span data-ttu-id="cd181-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd181-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd181-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd181-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd181-106">更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd181-106">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd181-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd181-107">Prerequisites</span></span>
<span data-ttu-id="cd181-108">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="cd181-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cd181-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd181-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="cd181-110">请注意，相应的权限因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="cd181-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="cd181-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd181-111">Permission type</span></span>|<span data-ttu-id="cd181-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd181-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd181-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd181-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd181-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd181-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd181-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd181-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd181-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd181-116">Not supported.</span></span>|
|<span data-ttu-id="cd181-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd181-117">Application</span></span>|<span data-ttu-id="cd181-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd181-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd181-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd181-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="cd181-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd181-120">Request headers</span></span>
|<span data-ttu-id="cd181-121">标头</span><span class="sxs-lookup"><span data-stu-id="cd181-121">Header</span></span>|<span data-ttu-id="cd181-122">值</span><span class="sxs-lookup"><span data-stu-id="cd181-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd181-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd181-123">Authorization</span></span>|<span data-ttu-id="cd181-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd181-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd181-125">接受</span><span class="sxs-lookup"><span data-stu-id="cd181-125">Accept</span></span>|<span data-ttu-id="cd181-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd181-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd181-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd181-127">Request body</span></span>
<span data-ttu-id="cd181-128">在请求正文中，提供 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd181-128">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="cd181-129">下表显示创建 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd181-129">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="cd181-130">属性</span><span class="sxs-lookup"><span data-stu-id="cd181-130">Property</span></span>|<span data-ttu-id="cd181-131">类型</span><span class="sxs-lookup"><span data-stu-id="cd181-131">Type</span></span>|<span data-ttu-id="cd181-132">说明</span><span class="sxs-lookup"><span data-stu-id="cd181-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd181-133">id</span><span class="sxs-lookup"><span data-stu-id="cd181-133">id</span></span>|<span data-ttu-id="cd181-134">String</span><span class="sxs-lookup"><span data-stu-id="cd181-134">String</span></span>|<span data-ttu-id="cd181-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd181-135">Key of the entity.</span></span>|
|<span data-ttu-id="cd181-136">**载入**</span><span class="sxs-lookup"><span data-stu-id="cd181-136">**Onboarding**</span></span>|
|<span data-ttu-id="cd181-137">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="cd181-137">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="cd181-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd181-138">Boolean</span></span>|<span data-ttu-id="cd181-139">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="cd181-139">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="cd181-140">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="cd181-140">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="cd181-141">String</span><span class="sxs-lookup"><span data-stu-id="cd181-141">String</span></span>|<span data-ttu-id="cd181-142">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="cd181-142">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="cd181-143">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="cd181-143">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="cd181-144">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="cd181-144">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="cd181-145">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="cd181-145">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="cd181-146">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="cd181-146">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="cd181-147">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="cd181-147">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="cd181-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd181-148">DateTimeOffset</span></span>|<span data-ttu-id="cd181-149">上次完成从适用于企业的 Microsoft Store 的应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="cd181-149">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="cd181-150">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cd181-150">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="cd181-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd181-151">DateTimeOffset</span></span>|<span data-ttu-id="cd181-152">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="cd181-152">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="cd181-153">响应</span><span class="sxs-lookup"><span data-stu-id="cd181-153">Response</span></span>
<span data-ttu-id="cd181-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd181-154">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="cd181-155">示例请求</span><span class="sxs-lookup"><span data-stu-id="cd181-155">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="cd181-156">示例响应</span><span class="sxs-lookup"><span data-stu-id="cd181-156">Example response</span></span>

<span data-ttu-id="cd181-157">为简洁起见，可能会截断此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd181-157">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cd181-158">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd181-158">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```









