---
title: 创建 groupPolicyMigrationReport
description: 创建新的 groupPolicyMigrationReport 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c0e52db29b0ce0545b42aa6951afdb4f887b511
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384134"
---
# <a name="create-grouppolicymigrationreport"></a><span data-ttu-id="67e0a-103">创建 groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="67e0a-103">Create groupPolicyMigrationReport</span></span>

<span data-ttu-id="67e0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67e0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67e0a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67e0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67e0a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67e0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67e0a-107">创建新的[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67e0a-107">Create a new [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67e0a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="67e0a-108">Prerequisites</span></span>
<span data-ttu-id="67e0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67e0a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="67e0a-111">Permission type</span></span>|<span data-ttu-id="67e0a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="67e0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67e0a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67e0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67e0a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67e0a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67e0a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67e0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67e0a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67e0a-116">Not supported.</span></span>|
|<span data-ttu-id="67e0a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="67e0a-117">Application</span></span>|<span data-ttu-id="67e0a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67e0a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67e0a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67e0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="67e0a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="67e0a-120">Request headers</span></span>
|<span data-ttu-id="67e0a-121">标头</span><span class="sxs-lookup"><span data-stu-id="67e0a-121">Header</span></span>|<span data-ttu-id="67e0a-122">值</span><span class="sxs-lookup"><span data-stu-id="67e0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67e0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67e0a-123">Authorization</span></span>|<span data-ttu-id="67e0a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67e0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67e0a-125">接受</span><span class="sxs-lookup"><span data-stu-id="67e0a-125">Accept</span></span>|<span data-ttu-id="67e0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67e0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67e0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="67e0a-127">Request body</span></span>
<span data-ttu-id="67e0a-128">在请求正文中，提供 groupPolicyMigrationReport 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67e0a-128">In the request body, supply a JSON representation for the groupPolicyMigrationReport object.</span></span>

<span data-ttu-id="67e0a-129">下表显示创建 groupPolicyMigrationReport 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67e0a-129">The following table shows the properties that are required when you create the groupPolicyMigrationReport.</span></span>

|<span data-ttu-id="67e0a-130">属性</span><span class="sxs-lookup"><span data-stu-id="67e0a-130">Property</span></span>|<span data-ttu-id="67e0a-131">类型</span><span class="sxs-lookup"><span data-stu-id="67e0a-131">Type</span></span>|<span data-ttu-id="67e0a-132">说明</span><span class="sxs-lookup"><span data-stu-id="67e0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67e0a-133">id</span><span class="sxs-lookup"><span data-stu-id="67e0a-133">id</span></span>|<span data-ttu-id="67e0a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="67e0a-134">String</span></span>|<span data-ttu-id="67e0a-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="67e0a-135">Not yet documented</span></span>|
|<span data-ttu-id="67e0a-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="67e0a-136">groupPolicyObjectId</span></span>|<span data-ttu-id="67e0a-137">Guid</span><span class="sxs-lookup"><span data-stu-id="67e0a-137">Guid</span></span>|<span data-ttu-id="67e0a-138">GPO Xml 内容中的组策略对象 GUID</span><span class="sxs-lookup"><span data-stu-id="67e0a-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="67e0a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="67e0a-139">displayName</span></span>|<span data-ttu-id="67e0a-140">String</span><span class="sxs-lookup"><span data-stu-id="67e0a-140">String</span></span>|<span data-ttu-id="67e0a-141">来自 GPO Xml 内容的组策略对象的名称</span><span class="sxs-lookup"><span data-stu-id="67e0a-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="67e0a-142">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="67e0a-142">ouDistinguishedName</span></span>|<span data-ttu-id="67e0a-143">字符串</span><span class="sxs-lookup"><span data-stu-id="67e0a-143">String</span></span>|<span data-ttu-id="67e0a-144">OU 的可分辨名称。</span><span class="sxs-lookup"><span data-stu-id="67e0a-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="67e0a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67e0a-145">createdDateTime</span></span>|<span data-ttu-id="67e0a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e0a-146">DateTimeOffset</span></span>|<span data-ttu-id="67e0a-147">GroupPolicyMigrationReport 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67e0a-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="67e0a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67e0a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="67e0a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e0a-149">DateTimeOffset</span></span>|<span data-ttu-id="67e0a-150">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67e0a-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="67e0a-151">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="67e0a-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="67e0a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e0a-152">DateTimeOffset</span></span>|<span data-ttu-id="67e0a-153">GroupPolicyMigrationReport 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67e0a-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="67e0a-154">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67e0a-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="67e0a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e0a-155">DateTimeOffset</span></span>|<span data-ttu-id="67e0a-156">上次修改 GroupPolicyMigrationReport 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67e0a-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="67e0a-157">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="67e0a-157">migrationReadiness</span></span>|[<span data-ttu-id="67e0a-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="67e0a-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="67e0a-159">相关联的组策略对象文件的 Intune 覆盖范围。</span><span class="sxs-lookup"><span data-stu-id="67e0a-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="67e0a-160">可取值为：`none`、`partial`、`complete`、`error`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="67e0a-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="67e0a-161">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="67e0a-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="67e0a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="67e0a-162">Boolean</span></span>|<span data-ttu-id="67e0a-163">来自 GPO Xml 内容的 AD 属性中的目标</span><span class="sxs-lookup"><span data-stu-id="67e0a-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="67e0a-164">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="67e0a-164">totalSettingsCount</span></span>|<span data-ttu-id="67e0a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="67e0a-165">Int32</span></span>|<span data-ttu-id="67e0a-166">GPO 文件中的组策略设置总数。</span><span class="sxs-lookup"><span data-stu-id="67e0a-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="67e0a-167">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="67e0a-167">supportedSettingsCount</span></span>|<span data-ttu-id="67e0a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="67e0a-168">Int32</span></span>|<span data-ttu-id="67e0a-169">Intune 支持的组策略设置的数量。</span><span class="sxs-lookup"><span data-stu-id="67e0a-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="67e0a-170">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="67e0a-170">supportedSettingsPercent</span></span>|<span data-ttu-id="67e0a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="67e0a-171">Int32</span></span>|<span data-ttu-id="67e0a-172">Intune 支持的组策略设置的百分比。</span><span class="sxs-lookup"><span data-stu-id="67e0a-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="67e0a-173">响应</span><span class="sxs-lookup"><span data-stu-id="67e0a-173">Response</span></span>
<span data-ttu-id="67e0a-174">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67e0a-174">If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67e0a-175">示例</span><span class="sxs-lookup"><span data-stu-id="67e0a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="67e0a-176">请求</span><span class="sxs-lookup"><span data-stu-id="67e0a-176">Request</span></span>
<span data-ttu-id="67e0a-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67e0a-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
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

### <a name="response"></a><span data-ttu-id="67e0a-178">响应</span><span class="sxs-lookup"><span data-stu-id="67e0a-178">Response</span></span>
<span data-ttu-id="67e0a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67e0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



