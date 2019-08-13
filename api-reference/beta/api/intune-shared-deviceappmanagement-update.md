---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 89f77f0e39f8337136a428fb421143a65ff8ee35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351005"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="ebafd-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="ebafd-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="ebafd-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ebafd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ebafd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ebafd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebafd-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebafd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebafd-107">更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebafd-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ebafd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ebafd-108">Prerequisites</span></span>
<span data-ttu-id="ebafd-109">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="ebafd-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ebafd-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebafd-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ebafd-111">请注意, 相应的权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="ebafd-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="ebafd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebafd-112">Permission type</span></span>|<span data-ttu-id="ebafd-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ebafd-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="ebafd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebafd-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="ebafd-115">&nbsp;&nbsp; **应用**、**图书**、**载入**或**合作伙伴集成**</span><span class="sxs-lookup"><span data-stu-id="ebafd-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, or **Partner Integration**</span></span> | <span data-ttu-id="ebafd-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebafd-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ebafd-117">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="ebafd-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ebafd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebafd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ebafd-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebafd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebafd-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebafd-120">Not supported.</span></span> |
| <span data-ttu-id="ebafd-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebafd-121">Application</span></span> | <span data-ttu-id="ebafd-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebafd-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebafd-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebafd-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="ebafd-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebafd-124">Request headers</span></span>
|<span data-ttu-id="ebafd-125">标头</span><span class="sxs-lookup"><span data-stu-id="ebafd-125">Header</span></span>|<span data-ttu-id="ebafd-126">值</span><span class="sxs-lookup"><span data-stu-id="ebafd-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebafd-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebafd-127">Authorization</span></span>|<span data-ttu-id="ebafd-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ebafd-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebafd-129">接受</span><span class="sxs-lookup"><span data-stu-id="ebafd-129">Accept</span></span>|<span data-ttu-id="ebafd-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ebafd-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebafd-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebafd-131">Request body</span></span>
<span data-ttu-id="ebafd-132">在请求正文中，提供 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebafd-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="ebafd-133">下表显示创建 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ebafd-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="ebafd-134">属性</span><span class="sxs-lookup"><span data-stu-id="ebafd-134">Property</span></span>|<span data-ttu-id="ebafd-135">类型</span><span class="sxs-lookup"><span data-stu-id="ebafd-135">Type</span></span>|<span data-ttu-id="ebafd-136">说明</span><span class="sxs-lookup"><span data-stu-id="ebafd-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebafd-137">id</span><span class="sxs-lookup"><span data-stu-id="ebafd-137">id</span></span>|<span data-ttu-id="ebafd-138">String</span><span class="sxs-lookup"><span data-stu-id="ebafd-138">String</span></span>|<span data-ttu-id="ebafd-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ebafd-139">Key of the entity.</span></span>|
|<span data-ttu-id="ebafd-140">**入职**</span><span class="sxs-lookup"><span data-stu-id="ebafd-140">**On-boarding**</span></span>|
|<span data-ttu-id="ebafd-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="ebafd-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="ebafd-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebafd-142">Boolean</span></span>|<span data-ttu-id="ebafd-143">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="ebafd-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="ebafd-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="ebafd-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="ebafd-145">String</span><span class="sxs-lookup"><span data-stu-id="ebafd-145">String</span></span>|<span data-ttu-id="ebafd-146">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="ebafd-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="ebafd-147">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="ebafd-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="ebafd-148">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="ebafd-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="ebafd-149">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="ebafd-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="ebafd-150">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="ebafd-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="ebafd-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="ebafd-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="ebafd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebafd-152">DateTimeOffset</span></span>|<span data-ttu-id="ebafd-153">上次完成从适用于企业的 Microsoft Store 的应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="ebafd-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="ebafd-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ebafd-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ebafd-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebafd-155">DateTimeOffset</span></span>|<span data-ttu-id="ebafd-156">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="ebafd-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="ebafd-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="ebafd-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="ebafd-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="ebafd-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="ebafd-159">最终用户门户信息用于将应用程序从 Microsoft Store for Business to Intune 公司门户同步。</span><span class="sxs-lookup"><span data-stu-id="ebafd-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="ebafd-160">有三个选项可供选择\["仅限公司门户"、"公司门户和专用存储"、"仅专用存储\]"。</span><span class="sxs-lookup"><span data-stu-id="ebafd-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="ebafd-161">可取值为：`none`、`companyPortal`、`privateStore`。</span><span class="sxs-lookup"><span data-stu-id="ebafd-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="ebafd-162">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ebafd-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="ebafd-163">响应</span><span class="sxs-lookup"><span data-stu-id="ebafd-163">Response</span></span>
<span data-ttu-id="ebafd-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebafd-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebafd-165">示例</span><span class="sxs-lookup"><span data-stu-id="ebafd-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebafd-166">请求</span><span class="sxs-lookup"><span data-stu-id="ebafd-166">Request</span></span>

<span data-ttu-id="ebafd-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebafd-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="ebafd-168">响应</span><span class="sxs-lookup"><span data-stu-id="ebafd-168">Response</span></span>

<span data-ttu-id="ebafd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ebafd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```






