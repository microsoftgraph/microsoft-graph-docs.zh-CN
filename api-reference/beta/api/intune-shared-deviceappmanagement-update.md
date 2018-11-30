---
title: 更新 deviceAppManagement
description: 更新 deviceAppManagement 对象的属性。
ms.openlocfilehash: e842e81f098a42e064be1aa00616a84d7f08eb34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046666"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="7b620-103">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7b620-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="7b620-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b620-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b620-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b620-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b620-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7b620-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b620-107">更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b620-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b620-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b620-108">Prerequisites</span></span>
<span data-ttu-id="7b620-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7b620-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7b620-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b620-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7b620-111">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="7b620-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="7b620-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b620-112">Permission type</span></span>|<span data-ttu-id="7b620-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b620-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="7b620-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b620-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="7b620-115">&nbsp;&nbsp; **应用程序**、**书籍**或**入职培训**</span><span class="sxs-lookup"><span data-stu-id="7b620-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="7b620-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b620-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="7b620-117">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="7b620-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7b620-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b620-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="7b620-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b620-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b620-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b620-120">Not supported.</span></span> |
| <span data-ttu-id="7b620-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b620-121">Application</span></span> | <span data-ttu-id="7b620-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b620-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b620-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b620-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="7b620-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b620-124">Request headers</span></span>
|<span data-ttu-id="7b620-125">标头</span><span class="sxs-lookup"><span data-stu-id="7b620-125">Header</span></span>|<span data-ttu-id="7b620-126">值</span><span class="sxs-lookup"><span data-stu-id="7b620-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b620-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b620-127">Authorization</span></span>|<span data-ttu-id="7b620-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b620-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b620-129">Accept</span><span class="sxs-lookup"><span data-stu-id="7b620-129">Accept</span></span>|<span data-ttu-id="7b620-130">application/json</span><span class="sxs-lookup"><span data-stu-id="7b620-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b620-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b620-131">Request body</span></span>
<span data-ttu-id="7b620-132">在请求正文中，提供 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b620-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="7b620-133">下表显示创建 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b620-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="7b620-134">属性</span><span class="sxs-lookup"><span data-stu-id="7b620-134">Property</span></span>|<span data-ttu-id="7b620-135">类型</span><span class="sxs-lookup"><span data-stu-id="7b620-135">Type</span></span>|<span data-ttu-id="7b620-136">说明</span><span class="sxs-lookup"><span data-stu-id="7b620-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b620-137">id</span><span class="sxs-lookup"><span data-stu-id="7b620-137">id</span></span>|<span data-ttu-id="7b620-138">String</span><span class="sxs-lookup"><span data-stu-id="7b620-138">String</span></span>|<span data-ttu-id="7b620-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b620-139">Key of the entity.</span></span>|
|<span data-ttu-id="7b620-140">**在白板**</span><span class="sxs-lookup"><span data-stu-id="7b620-140">**On-boarding**</span></span>|
|<span data-ttu-id="7b620-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="7b620-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="7b620-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b620-142">Boolean</span></span>|<span data-ttu-id="7b620-143">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="7b620-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="7b620-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="7b620-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="7b620-145">String</span><span class="sxs-lookup"><span data-stu-id="7b620-145">String</span></span>|<span data-ttu-id="7b620-146">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="7b620-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="7b620-147">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="7b620-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="7b620-148">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="7b620-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="7b620-149">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="7b620-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="7b620-150">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="7b620-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="7b620-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="7b620-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="7b620-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b620-152">DateTimeOffset</span></span>|<span data-ttu-id="7b620-153">从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。</span><span class="sxs-lookup"><span data-stu-id="7b620-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="7b620-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7b620-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="7b620-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b620-155">DateTimeOffset</span></span>|<span data-ttu-id="7b620-156">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="7b620-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="7b620-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="7b620-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="7b620-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="7b620-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="7b620-159">最终用户门户信息用于同步 Intune 的公司门户从 Microsoft 存储的业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="7b620-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="7b620-160">有三个选项，可以从中进行选取\[公司仅门户、 公司门户和专用存储、 仅专用存储\]。</span><span class="sxs-lookup"><span data-stu-id="7b620-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="7b620-161">可取值为：`none`、`companyPortal`、`privateStore`。</span><span class="sxs-lookup"><span data-stu-id="7b620-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="7b620-162">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7b620-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="7b620-163">响应</span><span class="sxs-lookup"><span data-stu-id="7b620-163">Response</span></span>
<span data-ttu-id="7b620-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b620-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b620-165">示例</span><span class="sxs-lookup"><span data-stu-id="7b620-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b620-166">请求</span><span class="sxs-lookup"><span data-stu-id="7b620-166">Request</span></span>

<span data-ttu-id="7b620-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b620-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="7b620-168">响应</span><span class="sxs-lookup"><span data-stu-id="7b620-168">Response</span></span>

<span data-ttu-id="7b620-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b620-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



