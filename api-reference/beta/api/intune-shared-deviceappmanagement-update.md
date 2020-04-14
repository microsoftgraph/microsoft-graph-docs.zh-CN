---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21362c0df13afe04f0dee6bf5fccc25661c833f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391132"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="a63a7-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a63a7-103">Update deviceAppManagement</span></span>

<span data-ttu-id="a63a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a63a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a63a7-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a63a7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a63a7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a63a7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a63a7-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a63a7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a63a7-108">更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a63a7-108">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a63a7-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="a63a7-109">Prerequisites</span></span>
<span data-ttu-id="a63a7-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="a63a7-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a63a7-111">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a63a7-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="a63a7-112">请注意，相应的权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="a63a7-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="a63a7-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a63a7-113">Permission type</span></span>|<span data-ttu-id="a63a7-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a63a7-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="a63a7-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a63a7-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="a63a7-116">&nbsp;&nbsp; **应用**、**图书**、**加入**、**合作伙伴集成**或**策略集**</span><span class="sxs-lookup"><span data-stu-id="a63a7-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="a63a7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a63a7-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="a63a7-118">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="a63a7-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a63a7-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a63a7-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="a63a7-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a63a7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a63a7-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a63a7-121">Not supported.</span></span> |
| <span data-ttu-id="a63a7-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="a63a7-122">Application</span></span> | |
| <span data-ttu-id="a63a7-123">&nbsp;&nbsp; **应用**、**图书**、**加入**、**合作伙伴集成**或**策略集**</span><span class="sxs-lookup"><span data-stu-id="a63a7-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="a63a7-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a63a7-124">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="a63a7-125">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="a63a7-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a63a7-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a63a7-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a63a7-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a63a7-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="a63a7-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="a63a7-128">Request headers</span></span>
|<span data-ttu-id="a63a7-129">标头</span><span class="sxs-lookup"><span data-stu-id="a63a7-129">Header</span></span>|<span data-ttu-id="a63a7-130">值</span><span class="sxs-lookup"><span data-stu-id="a63a7-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a63a7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a63a7-131">Authorization</span></span>|<span data-ttu-id="a63a7-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a63a7-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a63a7-133">接受</span><span class="sxs-lookup"><span data-stu-id="a63a7-133">Accept</span></span>|<span data-ttu-id="a63a7-134">application/json</span><span class="sxs-lookup"><span data-stu-id="a63a7-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a63a7-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="a63a7-135">Request body</span></span>
<span data-ttu-id="a63a7-136">在请求正文中，提供 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a63a7-136">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="a63a7-137">下表显示创建 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a63a7-137">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="a63a7-138">属性</span><span class="sxs-lookup"><span data-stu-id="a63a7-138">Property</span></span>|<span data-ttu-id="a63a7-139">类型</span><span class="sxs-lookup"><span data-stu-id="a63a7-139">Type</span></span>|<span data-ttu-id="a63a7-140">说明</span><span class="sxs-lookup"><span data-stu-id="a63a7-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a63a7-141">id</span><span class="sxs-lookup"><span data-stu-id="a63a7-141">id</span></span>|<span data-ttu-id="a63a7-142">字符串</span><span class="sxs-lookup"><span data-stu-id="a63a7-142">String</span></span>|<span data-ttu-id="a63a7-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a63a7-143">Key of the entity.</span></span>|
|<span data-ttu-id="a63a7-144">**入职**</span><span class="sxs-lookup"><span data-stu-id="a63a7-144">**On-boarding**</span></span>|
|<span data-ttu-id="a63a7-145">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="a63a7-145">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="a63a7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a63a7-146">Boolean</span></span>|<span data-ttu-id="a63a7-147">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="a63a7-147">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="a63a7-148">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="a63a7-148">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="a63a7-149">String</span><span class="sxs-lookup"><span data-stu-id="a63a7-149">String</span></span>|<span data-ttu-id="a63a7-150">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="a63a7-150">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="a63a7-151">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="a63a7-151">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="a63a7-152">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a63a7-152">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="a63a7-153">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="a63a7-153">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="a63a7-154">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="a63a7-154">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="a63a7-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="a63a7-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="a63a7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a63a7-156">DateTimeOffset</span></span>|<span data-ttu-id="a63a7-157">上次完成从适用于企业的 Microsoft Store 的应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="a63a7-157">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="a63a7-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a63a7-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a63a7-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a63a7-159">DateTimeOffset</span></span>|<span data-ttu-id="a63a7-160">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="a63a7-160">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="a63a7-161">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="a63a7-161">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="a63a7-162">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="a63a7-162">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="a63a7-163">最终用户门户信息用于将应用程序从 Microsoft Store for Business to Intune 公司门户同步。</span><span class="sxs-lookup"><span data-stu-id="a63a7-163">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="a63a7-164">有三个选项可供选择\["仅限公司门户"、"公司门户和专用存储"、"仅专用存储\]"。</span><span class="sxs-lookup"><span data-stu-id="a63a7-164">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="a63a7-165">可取值为：`none`、`companyPortal`、`privateStore`。</span><span class="sxs-lookup"><span data-stu-id="a63a7-165">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="a63a7-166">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a63a7-166">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="a63a7-167">响应</span><span class="sxs-lookup"><span data-stu-id="a63a7-167">Response</span></span>
<span data-ttu-id="a63a7-168">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a63a7-168">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a63a7-169">示例</span><span class="sxs-lookup"><span data-stu-id="a63a7-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="a63a7-170">请求</span><span class="sxs-lookup"><span data-stu-id="a63a7-170">Request</span></span>

<span data-ttu-id="a63a7-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a63a7-171">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="a63a7-172">响应</span><span class="sxs-lookup"><span data-stu-id="a63a7-172">Response</span></span>

<span data-ttu-id="a63a7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a63a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```









