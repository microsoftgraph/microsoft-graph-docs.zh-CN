---
title: 更新 groupPolicySettingMapping
description: 更新 groupPolicySettingMapping 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82575a97badaba93f179c841502727e07ebff0af
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149826"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="3e6f3-103">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="3e6f3-103">Update groupPolicySettingMapping</span></span>

<span data-ttu-id="3e6f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e6f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e6f3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e6f3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e6f3-107">更新 [groupPolicySettingMapping 对象](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-107">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e6f3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3e6f3-108">Prerequisites</span></span>
<span data-ttu-id="3e6f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e6f3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e6f3-111">Permission type</span></span>|<span data-ttu-id="3e6f3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e6f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e6f3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e6f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e6f3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e6f3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e6f3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e6f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e6f3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-116">Not supported.</span></span>|
|<span data-ttu-id="3e6f3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e6f3-117">Application</span></span>|<span data-ttu-id="3e6f3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e6f3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e6f3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e6f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="3e6f3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e6f3-120">Request headers</span></span>
|<span data-ttu-id="3e6f3-121">标头</span><span class="sxs-lookup"><span data-stu-id="3e6f3-121">Header</span></span>|<span data-ttu-id="3e6f3-122">值</span><span class="sxs-lookup"><span data-stu-id="3e6f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e6f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e6f3-123">Authorization</span></span>|<span data-ttu-id="3e6f3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e6f3-125">接受</span><span class="sxs-lookup"><span data-stu-id="3e6f3-125">Accept</span></span>|<span data-ttu-id="3e6f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e6f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e6f3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e6f3-127">Request body</span></span>
<span data-ttu-id="3e6f3-128">在请求正文中，提供 [groupPolicySettingMapping 对象的](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-128">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="3e6f3-129">下表显示创建 [groupPolicySettingMapping 时所需的属性](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-129">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="3e6f3-130">属性</span><span class="sxs-lookup"><span data-stu-id="3e6f3-130">Property</span></span>|<span data-ttu-id="3e6f3-131">类型</span><span class="sxs-lookup"><span data-stu-id="3e6f3-131">Type</span></span>|<span data-ttu-id="3e6f3-132">说明</span><span class="sxs-lookup"><span data-stu-id="3e6f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e6f3-133">id</span><span class="sxs-lookup"><span data-stu-id="3e6f3-133">id</span></span>|<span data-ttu-id="3e6f3-134">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-134">String</span></span>|<span data-ttu-id="3e6f3-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3e6f3-135">Not yet documented</span></span>|
|<span data-ttu-id="3e6f3-136">parentId</span><span class="sxs-lookup"><span data-stu-id="3e6f3-136">parentId</span></span>|<span data-ttu-id="3e6f3-137">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-137">String</span></span>|<span data-ttu-id="3e6f3-138">组策略设置的父 ID。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-139">childIdList</span><span class="sxs-lookup"><span data-stu-id="3e6f3-139">childIdList</span></span>|<span data-ttu-id="3e6f3-140">String collection</span><span class="sxs-lookup"><span data-stu-id="3e6f3-140">String collection</span></span>|<span data-ttu-id="3e6f3-141">组策略设置的子 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-142">settingName</span><span class="sxs-lookup"><span data-stu-id="3e6f3-142">settingName</span></span>|<span data-ttu-id="3e6f3-143">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-143">String</span></span>|<span data-ttu-id="3e6f3-144">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="3e6f3-145">settingValue</span></span>|<span data-ttu-id="3e6f3-146">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-146">String</span></span>|<span data-ttu-id="3e6f3-147">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-148">settingValueType</span><span class="sxs-lookup"><span data-stu-id="3e6f3-148">settingValueType</span></span>|<span data-ttu-id="3e6f3-149">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-149">String</span></span>|<span data-ttu-id="3e6f3-150">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-151">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e6f3-151">settingDisplayName</span></span>|<span data-ttu-id="3e6f3-152">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-152">String</span></span>|<span data-ttu-id="3e6f3-153">此显示名称策略设置的成员。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-154">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="3e6f3-154">settingDisplayValue</span></span>|<span data-ttu-id="3e6f3-155">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-155">String</span></span>|<span data-ttu-id="3e6f3-156">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-157">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="3e6f3-157">settingDisplayValueType</span></span>|<span data-ttu-id="3e6f3-158">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-158">String</span></span>|<span data-ttu-id="3e6f3-159">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="3e6f3-160">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="3e6f3-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="3e6f3-161">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-161">String</span></span>|<span data-ttu-id="3e6f3-162">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="3e6f3-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="3e6f3-163">settingCategory</span><span class="sxs-lookup"><span data-stu-id="3e6f3-163">settingCategory</span></span>|<span data-ttu-id="3e6f3-164">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-164">String</span></span>|<span data-ttu-id="3e6f3-165">组策略设置位于的类别。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="3e6f3-166">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="3e6f3-166">mdmCspName</span></span>|<span data-ttu-id="3e6f3-167">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-167">String</span></span>|<span data-ttu-id="3e6f3-168">此组策略设置映射到的云解决方案提供商名称。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="3e6f3-169">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="3e6f3-169">mdmSettingUri</span></span>|<span data-ttu-id="3e6f3-170">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-170">String</span></span>|<span data-ttu-id="3e6f3-171">此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="3e6f3-172">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="3e6f3-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="3e6f3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3e6f3-173">Int32</span></span>|<span data-ttu-id="3e6f3-174">此 mdm 设置支持的最低操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="3e6f3-175">settingType</span><span class="sxs-lookup"><span data-stu-id="3e6f3-175">settingType</span></span>|[<span data-ttu-id="3e6f3-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="3e6f3-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="3e6f3-177">设置类型 (安全或 admx) 组策略。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="3e6f3-178">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="3e6f3-179">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="3e6f3-179">isMdmSupported</span></span>|<span data-ttu-id="3e6f3-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e6f3-180">Boolean</span></span>|<span data-ttu-id="3e6f3-181">指示 Intune 是否支持该设置</span><span class="sxs-lookup"><span data-stu-id="3e6f3-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="3e6f3-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="3e6f3-182">mdmSupportedState</span></span>|[<span data-ttu-id="3e6f3-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="3e6f3-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="3e6f3-184">指示设置在 Mdm 中是否受支持。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="3e6f3-185">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="3e6f3-186">settingScope</span><span class="sxs-lookup"><span data-stu-id="3e6f3-186">settingScope</span></span>|[<span data-ttu-id="3e6f3-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="3e6f3-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="3e6f3-188">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-188">The scope of the setting.</span></span> <span data-ttu-id="3e6f3-189">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="3e6f3-190">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="3e6f3-190">intuneSettingUriList</span></span>|<span data-ttu-id="3e6f3-191">String collection</span><span class="sxs-lookup"><span data-stu-id="3e6f3-191">String collection</span></span>|<span data-ttu-id="3e6f3-192">此组策略设置映射到的 Intune 设置 URI 列表</span><span class="sxs-lookup"><span data-stu-id="3e6f3-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="3e6f3-193">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3e6f3-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="3e6f3-194">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-194">String</span></span>|<span data-ttu-id="3e6f3-195">Intune 设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="3e6f3-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="3e6f3-196">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3e6f3-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="3e6f3-197">String</span><span class="sxs-lookup"><span data-stu-id="3e6f3-197">String</span></span>|<span data-ttu-id="3e6f3-198">Admx 组策略 ID</span><span class="sxs-lookup"><span data-stu-id="3e6f3-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="3e6f3-199">响应</span><span class="sxs-lookup"><span data-stu-id="3e6f3-199">Response</span></span>
<span data-ttu-id="3e6f3-200">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-200">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e6f3-201">示例</span><span class="sxs-lookup"><span data-stu-id="3e6f3-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e6f3-202">请求</span><span class="sxs-lookup"><span data-stu-id="3e6f3-202">Request</span></span>
<span data-ttu-id="3e6f3-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 1023

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="3e6f3-204">响应</span><span class="sxs-lookup"><span data-stu-id="3e6f3-204">Response</span></span>
<span data-ttu-id="3e6f3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e6f3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1072

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```




