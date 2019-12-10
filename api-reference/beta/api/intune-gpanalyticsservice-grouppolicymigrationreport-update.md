---
title: 更新 groupPolicyMigrationReport
description: 更新 groupPolicyMigrationReport 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 092d65482bbcbebb810ed004fae80cd42afff103
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943275"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="76610-103">更新 groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="76610-103">Update groupPolicyMigrationReport</span></span>

> <span data-ttu-id="76610-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76610-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76610-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76610-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76610-106">更新[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76610-106">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76610-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="76610-107">Prerequisites</span></span>
<span data-ttu-id="76610-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76610-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="76610-110">Permission type</span></span>|<span data-ttu-id="76610-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76610-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76610-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76610-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76610-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76610-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76610-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76610-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76610-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="76610-115">Not supported.</span></span>|
|<span data-ttu-id="76610-116">Application</span><span class="sxs-lookup"><span data-stu-id="76610-116">Application</span></span>|<span data-ttu-id="76610-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76610-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76610-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76610-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="76610-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="76610-119">Request headers</span></span>
|<span data-ttu-id="76610-120">标头</span><span class="sxs-lookup"><span data-stu-id="76610-120">Header</span></span>|<span data-ttu-id="76610-121">值</span><span class="sxs-lookup"><span data-stu-id="76610-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76610-122">授权</span><span class="sxs-lookup"><span data-stu-id="76610-122">Authorization</span></span>|<span data-ttu-id="76610-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76610-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76610-124">接受</span><span class="sxs-lookup"><span data-stu-id="76610-124">Accept</span></span>|<span data-ttu-id="76610-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76610-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76610-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="76610-126">Request body</span></span>
<span data-ttu-id="76610-127">在请求正文中，提供[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76610-127">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="76610-128">下表显示创建[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="76610-128">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="76610-129">属性</span><span class="sxs-lookup"><span data-stu-id="76610-129">Property</span></span>|<span data-ttu-id="76610-130">类型</span><span class="sxs-lookup"><span data-stu-id="76610-130">Type</span></span>|<span data-ttu-id="76610-131">说明</span><span class="sxs-lookup"><span data-stu-id="76610-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76610-132">id</span><span class="sxs-lookup"><span data-stu-id="76610-132">id</span></span>|<span data-ttu-id="76610-133">字符串</span><span class="sxs-lookup"><span data-stu-id="76610-133">String</span></span>|<span data-ttu-id="76610-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="76610-134">Not yet documented</span></span>|
|<span data-ttu-id="76610-135">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="76610-135">groupPolicyObjectId</span></span>|<span data-ttu-id="76610-136">Guid</span><span class="sxs-lookup"><span data-stu-id="76610-136">Guid</span></span>|<span data-ttu-id="76610-137">GPO Xml 内容中的组策略对象 GUID</span><span class="sxs-lookup"><span data-stu-id="76610-137">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="76610-138">displayName</span><span class="sxs-lookup"><span data-stu-id="76610-138">displayName</span></span>|<span data-ttu-id="76610-139">String</span><span class="sxs-lookup"><span data-stu-id="76610-139">String</span></span>|<span data-ttu-id="76610-140">来自 GPO Xml 内容的组策略对象的名称</span><span class="sxs-lookup"><span data-stu-id="76610-140">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="76610-141">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="76610-141">ouDistinguishedName</span></span>|<span data-ttu-id="76610-142">字符串</span><span class="sxs-lookup"><span data-stu-id="76610-142">String</span></span>|<span data-ttu-id="76610-143">OU 的可分辨名称。</span><span class="sxs-lookup"><span data-stu-id="76610-143">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="76610-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76610-144">createdDateTime</span></span>|<span data-ttu-id="76610-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76610-145">DateTimeOffset</span></span>|<span data-ttu-id="76610-146">GroupPolicyMigrationReport 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76610-146">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="76610-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76610-147">lastModifiedDateTime</span></span>|<span data-ttu-id="76610-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76610-148">DateTimeOffset</span></span>|<span data-ttu-id="76610-149">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76610-149">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="76610-150">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="76610-150">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="76610-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76610-151">DateTimeOffset</span></span>|<span data-ttu-id="76610-152">GroupPolicyMigrationReport 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76610-152">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="76610-153">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76610-153">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="76610-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76610-154">DateTimeOffset</span></span>|<span data-ttu-id="76610-155">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76610-155">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="76610-156">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="76610-156">migrationReadiness</span></span>|[<span data-ttu-id="76610-157">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="76610-157">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="76610-158">相关联的组策略对象文件的 Intune 覆盖范围。</span><span class="sxs-lookup"><span data-stu-id="76610-158">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="76610-159">可取值为：`none`、`partial`、`complete`、`error`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="76610-159">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="76610-160">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="76610-160">targetedInActiveDirectory</span></span>|<span data-ttu-id="76610-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="76610-161">Boolean</span></span>|<span data-ttu-id="76610-162">来自 GPO Xml 内容的 AD 属性中的目标</span><span class="sxs-lookup"><span data-stu-id="76610-162">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="76610-163">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="76610-163">totalSettingsCount</span></span>|<span data-ttu-id="76610-164">Int32</span><span class="sxs-lookup"><span data-stu-id="76610-164">Int32</span></span>|<span data-ttu-id="76610-165">GPO 文件中的组策略设置总数。</span><span class="sxs-lookup"><span data-stu-id="76610-165">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="76610-166">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="76610-166">supportedSettingsCount</span></span>|<span data-ttu-id="76610-167">Int32</span><span class="sxs-lookup"><span data-stu-id="76610-167">Int32</span></span>|<span data-ttu-id="76610-168">Intune 支持的组策略设置的数量。</span><span class="sxs-lookup"><span data-stu-id="76610-168">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="76610-169">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="76610-169">supportedSettingsPercent</span></span>|<span data-ttu-id="76610-170">Int32</span><span class="sxs-lookup"><span data-stu-id="76610-170">Int32</span></span>|<span data-ttu-id="76610-171">Intune 支持的组策略设置的百分比。</span><span class="sxs-lookup"><span data-stu-id="76610-171">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="76610-172">响应</span><span class="sxs-lookup"><span data-stu-id="76610-172">Response</span></span>
<span data-ttu-id="76610-173">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象。</span><span class="sxs-lookup"><span data-stu-id="76610-173">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76610-174">示例</span><span class="sxs-lookup"><span data-stu-id="76610-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="76610-175">请求</span><span class="sxs-lookup"><span data-stu-id="76610-175">Request</span></span>
<span data-ttu-id="76610-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76610-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### <a name="response"></a><span data-ttu-id="76610-177">响应</span><span class="sxs-lookup"><span data-stu-id="76610-177">Response</span></span>
<span data-ttu-id="76610-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76610-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```





