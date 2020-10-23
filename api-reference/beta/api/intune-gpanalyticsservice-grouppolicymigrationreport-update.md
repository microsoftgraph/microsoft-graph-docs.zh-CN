---
title: 更新 groupPolicyMigrationReport
description: 更新 groupPolicyMigrationReport 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f56e27f41c2cecc19ab890612e30cb50146d3e0e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685630"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="f32ff-103">更新 groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="f32ff-103">Update groupPolicyMigrationReport</span></span>

<span data-ttu-id="f32ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f32ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f32ff-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f32ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f32ff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f32ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f32ff-107">更新 [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f32ff-107">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f32ff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f32ff-108">Prerequisites</span></span>
<span data-ttu-id="f32ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f32ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f32ff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f32ff-111">Permission type</span></span>|<span data-ttu-id="f32ff-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f32ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f32ff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f32ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f32ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f32ff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f32ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f32ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f32ff-116">Not supported.</span></span>|
|<span data-ttu-id="f32ff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f32ff-117">Application</span></span>|<span data-ttu-id="f32ff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32ff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f32ff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f32ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="f32ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f32ff-120">Request headers</span></span>
|<span data-ttu-id="f32ff-121">标头</span><span class="sxs-lookup"><span data-stu-id="f32ff-121">Header</span></span>|<span data-ttu-id="f32ff-122">值</span><span class="sxs-lookup"><span data-stu-id="f32ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f32ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f32ff-123">Authorization</span></span>|<span data-ttu-id="f32ff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f32ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f32ff-125">接受</span><span class="sxs-lookup"><span data-stu-id="f32ff-125">Accept</span></span>|<span data-ttu-id="f32ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f32ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f32ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f32ff-127">Request body</span></span>
<span data-ttu-id="f32ff-128">在请求正文中，提供 [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f32ff-128">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="f32ff-129">下表显示创建 [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f32ff-129">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="f32ff-130">属性</span><span class="sxs-lookup"><span data-stu-id="f32ff-130">Property</span></span>|<span data-ttu-id="f32ff-131">类型</span><span class="sxs-lookup"><span data-stu-id="f32ff-131">Type</span></span>|<span data-ttu-id="f32ff-132">说明</span><span class="sxs-lookup"><span data-stu-id="f32ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f32ff-133">id</span><span class="sxs-lookup"><span data-stu-id="f32ff-133">id</span></span>|<span data-ttu-id="f32ff-134">String</span><span class="sxs-lookup"><span data-stu-id="f32ff-134">String</span></span>|<span data-ttu-id="f32ff-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f32ff-135">Not yet documented</span></span>|
|<span data-ttu-id="f32ff-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="f32ff-136">groupPolicyObjectId</span></span>|<span data-ttu-id="f32ff-137">Guid</span><span class="sxs-lookup"><span data-stu-id="f32ff-137">Guid</span></span>|<span data-ttu-id="f32ff-138">GPO Xml 内容中的组策略对象 GUID</span><span class="sxs-lookup"><span data-stu-id="f32ff-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="f32ff-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f32ff-139">displayName</span></span>|<span data-ttu-id="f32ff-140">String</span><span class="sxs-lookup"><span data-stu-id="f32ff-140">String</span></span>|<span data-ttu-id="f32ff-141">来自 GPO Xml 内容的组策略对象的名称</span><span class="sxs-lookup"><span data-stu-id="f32ff-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="f32ff-142">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="f32ff-142">ouDistinguishedName</span></span>|<span data-ttu-id="f32ff-143">String</span><span class="sxs-lookup"><span data-stu-id="f32ff-143">String</span></span>|<span data-ttu-id="f32ff-144">OU 的可分辨名称。</span><span class="sxs-lookup"><span data-stu-id="f32ff-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="f32ff-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f32ff-145">createdDateTime</span></span>|<span data-ttu-id="f32ff-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32ff-146">DateTimeOffset</span></span>|<span data-ttu-id="f32ff-147">GroupPolicyMigrationReport 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f32ff-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="f32ff-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f32ff-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f32ff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32ff-149">DateTimeOffset</span></span>|<span data-ttu-id="f32ff-150">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f32ff-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="f32ff-151">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f32ff-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="f32ff-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32ff-152">DateTimeOffset</span></span>|<span data-ttu-id="f32ff-153">GroupPolicyMigrationReport 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f32ff-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="f32ff-154">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f32ff-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="f32ff-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32ff-155">DateTimeOffset</span></span>|<span data-ttu-id="f32ff-156">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f32ff-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="f32ff-157">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="f32ff-157">migrationReadiness</span></span>|[<span data-ttu-id="f32ff-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="f32ff-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="f32ff-159">相关联的组策略对象文件的 Intune 覆盖范围。</span><span class="sxs-lookup"><span data-stu-id="f32ff-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="f32ff-160">可取值为：`none`、`partial`、`complete`、`error`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="f32ff-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="f32ff-161">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="f32ff-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="f32ff-162">布尔</span><span class="sxs-lookup"><span data-stu-id="f32ff-162">Boolean</span></span>|<span data-ttu-id="f32ff-163">来自 GPO Xml 内容的 AD 属性中的目标</span><span class="sxs-lookup"><span data-stu-id="f32ff-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="f32ff-164">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="f32ff-164">totalSettingsCount</span></span>|<span data-ttu-id="f32ff-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f32ff-165">Int32</span></span>|<span data-ttu-id="f32ff-166">GPO 文件中的组策略设置总数。</span><span class="sxs-lookup"><span data-stu-id="f32ff-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="f32ff-167">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="f32ff-167">supportedSettingsCount</span></span>|<span data-ttu-id="f32ff-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f32ff-168">Int32</span></span>|<span data-ttu-id="f32ff-169">Intune 支持的组策略设置的数量。</span><span class="sxs-lookup"><span data-stu-id="f32ff-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="f32ff-170">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="f32ff-170">supportedSettingsPercent</span></span>|<span data-ttu-id="f32ff-171">Int32</span><span class="sxs-lookup"><span data-stu-id="f32ff-171">Int32</span></span>|<span data-ttu-id="f32ff-172">Intune 支持的组策略设置的百分比。</span><span class="sxs-lookup"><span data-stu-id="f32ff-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="f32ff-173">响应</span><span class="sxs-lookup"><span data-stu-id="f32ff-173">Response</span></span>
<span data-ttu-id="f32ff-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f32ff-174">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f32ff-175">示例</span><span class="sxs-lookup"><span data-stu-id="f32ff-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="f32ff-176">请求</span><span class="sxs-lookup"><span data-stu-id="f32ff-176">Request</span></span>
<span data-ttu-id="f32ff-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f32ff-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f32ff-178">响应</span><span class="sxs-lookup"><span data-stu-id="f32ff-178">Response</span></span>
<span data-ttu-id="f32ff-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f32ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





