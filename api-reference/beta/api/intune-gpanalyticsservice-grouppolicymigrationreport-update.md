---
title: 更新 groupPolicyMigrationReport
description: 更新 groupPolicyMigrationReport 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74eb28e0f4d0fed12399e1563661e25a1a2c92c1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159009"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="55711-103">更新 groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="55711-103">Update groupPolicyMigrationReport</span></span>

<span data-ttu-id="55711-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55711-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55711-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55711-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55711-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55711-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55711-107">更新 [groupPolicyMigrationReport 对象](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="55711-107">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55711-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="55711-108">Prerequisites</span></span>
<span data-ttu-id="55711-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55711-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="55711-111">Permission type</span></span>|<span data-ttu-id="55711-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55711-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55711-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55711-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55711-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55711-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55711-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55711-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55711-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55711-116">Not supported.</span></span>|
|<span data-ttu-id="55711-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="55711-117">Application</span></span>|<span data-ttu-id="55711-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55711-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55711-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55711-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="55711-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="55711-120">Request headers</span></span>
|<span data-ttu-id="55711-121">标头</span><span class="sxs-lookup"><span data-stu-id="55711-121">Header</span></span>|<span data-ttu-id="55711-122">值</span><span class="sxs-lookup"><span data-stu-id="55711-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55711-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55711-123">Authorization</span></span>|<span data-ttu-id="55711-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55711-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55711-125">接受</span><span class="sxs-lookup"><span data-stu-id="55711-125">Accept</span></span>|<span data-ttu-id="55711-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55711-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55711-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="55711-127">Request body</span></span>
<span data-ttu-id="55711-128">在请求正文中，提供 [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55711-128">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="55711-129">下表显示创建 [groupPolicyMigrationReport 时所需的属性](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)。</span><span class="sxs-lookup"><span data-stu-id="55711-129">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="55711-130">属性</span><span class="sxs-lookup"><span data-stu-id="55711-130">Property</span></span>|<span data-ttu-id="55711-131">类型</span><span class="sxs-lookup"><span data-stu-id="55711-131">Type</span></span>|<span data-ttu-id="55711-132">说明</span><span class="sxs-lookup"><span data-stu-id="55711-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55711-133">id</span><span class="sxs-lookup"><span data-stu-id="55711-133">id</span></span>|<span data-ttu-id="55711-134">String</span><span class="sxs-lookup"><span data-stu-id="55711-134">String</span></span>|<span data-ttu-id="55711-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="55711-135">Not yet documented</span></span>|
|<span data-ttu-id="55711-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="55711-136">groupPolicyObjectId</span></span>|<span data-ttu-id="55711-137">Guid</span><span class="sxs-lookup"><span data-stu-id="55711-137">Guid</span></span>|<span data-ttu-id="55711-138">GPO Xml 内容的组策略对象 GUID</span><span class="sxs-lookup"><span data-stu-id="55711-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="55711-139">displayName</span><span class="sxs-lookup"><span data-stu-id="55711-139">displayName</span></span>|<span data-ttu-id="55711-140">String</span><span class="sxs-lookup"><span data-stu-id="55711-140">String</span></span>|<span data-ttu-id="55711-141">GPO Xml 内容中的组策略对象的名称</span><span class="sxs-lookup"><span data-stu-id="55711-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="55711-142">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="55711-142">ouDistinguishedName</span></span>|<span data-ttu-id="55711-143">String</span><span class="sxs-lookup"><span data-stu-id="55711-143">String</span></span>|<span data-ttu-id="55711-144">OU 的可分辨名称。</span><span class="sxs-lookup"><span data-stu-id="55711-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="55711-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55711-145">createdDateTime</span></span>|<span data-ttu-id="55711-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55711-146">DateTimeOffset</span></span>|<span data-ttu-id="55711-147">创建 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55711-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="55711-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55711-148">lastModifiedDateTime</span></span>|<span data-ttu-id="55711-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55711-149">DateTimeOffset</span></span>|<span data-ttu-id="55711-150">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55711-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="55711-151">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="55711-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="55711-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55711-152">DateTimeOffset</span></span>|<span data-ttu-id="55711-153">创建 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55711-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="55711-154">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55711-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="55711-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55711-155">DateTimeOffset</span></span>|<span data-ttu-id="55711-156">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55711-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="55711-157">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="55711-157">migrationReadiness</span></span>|[<span data-ttu-id="55711-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="55711-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="55711-159">关联的组策略对象文件的 Intune 覆盖范围。</span><span class="sxs-lookup"><span data-stu-id="55711-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="55711-160">可取值为：`none`、`partial`、`complete`、`error`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="55711-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="55711-161">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="55711-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="55711-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="55711-162">Boolean</span></span>|<span data-ttu-id="55711-163">GPO Xml 内容中的 AD 中的目标属性</span><span class="sxs-lookup"><span data-stu-id="55711-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="55711-164">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="55711-164">totalSettingsCount</span></span>|<span data-ttu-id="55711-165">Int32</span><span class="sxs-lookup"><span data-stu-id="55711-165">Int32</span></span>|<span data-ttu-id="55711-166">GPO 文件中组策略设置的总数。</span><span class="sxs-lookup"><span data-stu-id="55711-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="55711-167">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="55711-167">supportedSettingsCount</span></span>|<span data-ttu-id="55711-168">Int32</span><span class="sxs-lookup"><span data-stu-id="55711-168">Int32</span></span>|<span data-ttu-id="55711-169">Intune 支持的组策略设置的数量。</span><span class="sxs-lookup"><span data-stu-id="55711-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="55711-170">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="55711-170">supportedSettingsPercent</span></span>|<span data-ttu-id="55711-171">Int32</span><span class="sxs-lookup"><span data-stu-id="55711-171">Int32</span></span>|<span data-ttu-id="55711-172">Intune 支持的组策略设置的百分比。</span><span class="sxs-lookup"><span data-stu-id="55711-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="55711-173">响应</span><span class="sxs-lookup"><span data-stu-id="55711-173">Response</span></span>
<span data-ttu-id="55711-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55711-174">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55711-175">示例</span><span class="sxs-lookup"><span data-stu-id="55711-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="55711-176">请求</span><span class="sxs-lookup"><span data-stu-id="55711-176">Request</span></span>
<span data-ttu-id="55711-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55711-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55711-178">响应</span><span class="sxs-lookup"><span data-stu-id="55711-178">Response</span></span>
<span data-ttu-id="55711-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55711-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




