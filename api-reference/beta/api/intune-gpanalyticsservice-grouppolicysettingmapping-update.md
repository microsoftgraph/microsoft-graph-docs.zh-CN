---
title: 更新 groupPolicySettingMapping
description: 更新 groupPolicySettingMapping 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a98970a6bef6a17ab134322d1b9d41bfcd195ef5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804574"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="38972-103">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="38972-103">Update groupPolicySettingMapping</span></span>

> <span data-ttu-id="38972-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38972-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38972-106">更新[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38972-106">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38972-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="38972-107">Prerequisites</span></span>
<span data-ttu-id="38972-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38972-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38972-110">Permission type</span></span>|<span data-ttu-id="38972-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38972-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38972-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38972-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38972-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38972-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38972-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38972-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38972-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38972-115">Not supported.</span></span>|
|<span data-ttu-id="38972-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38972-116">Application</span></span>|<span data-ttu-id="38972-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38972-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38972-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38972-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="38972-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38972-119">Request headers</span></span>
|<span data-ttu-id="38972-120">标头</span><span class="sxs-lookup"><span data-stu-id="38972-120">Header</span></span>|<span data-ttu-id="38972-121">值</span><span class="sxs-lookup"><span data-stu-id="38972-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38972-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38972-122">Authorization</span></span>|<span data-ttu-id="38972-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38972-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38972-124">接受</span><span class="sxs-lookup"><span data-stu-id="38972-124">Accept</span></span>|<span data-ttu-id="38972-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38972-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38972-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="38972-126">Request body</span></span>
<span data-ttu-id="38972-127">在请求正文中，提供[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38972-127">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="38972-128">下表显示创建[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38972-128">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="38972-129">属性</span><span class="sxs-lookup"><span data-stu-id="38972-129">Property</span></span>|<span data-ttu-id="38972-130">类型</span><span class="sxs-lookup"><span data-stu-id="38972-130">Type</span></span>|<span data-ttu-id="38972-131">说明</span><span class="sxs-lookup"><span data-stu-id="38972-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38972-132">id</span><span class="sxs-lookup"><span data-stu-id="38972-132">id</span></span>|<span data-ttu-id="38972-133">String</span><span class="sxs-lookup"><span data-stu-id="38972-133">String</span></span>|<span data-ttu-id="38972-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="38972-134">Not yet documented</span></span>|
|<span data-ttu-id="38972-135">parentId</span><span class="sxs-lookup"><span data-stu-id="38972-135">parentId</span></span>|<span data-ttu-id="38972-136">String</span><span class="sxs-lookup"><span data-stu-id="38972-136">String</span></span>|<span data-ttu-id="38972-137">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="38972-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="38972-138">childIdList</span><span class="sxs-lookup"><span data-stu-id="38972-138">childIdList</span></span>|<span data-ttu-id="38972-139">String collection</span><span class="sxs-lookup"><span data-stu-id="38972-139">String collection</span></span>|<span data-ttu-id="38972-140">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="38972-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="38972-141">settingName</span><span class="sxs-lookup"><span data-stu-id="38972-141">settingName</span></span>|<span data-ttu-id="38972-142">String</span><span class="sxs-lookup"><span data-stu-id="38972-142">String</span></span>|<span data-ttu-id="38972-143">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="38972-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="38972-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="38972-144">settingValue</span></span>|<span data-ttu-id="38972-145">String</span><span class="sxs-lookup"><span data-stu-id="38972-145">String</span></span>|<span data-ttu-id="38972-146">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="38972-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="38972-147">settingValueType</span><span class="sxs-lookup"><span data-stu-id="38972-147">settingValueType</span></span>|<span data-ttu-id="38972-148">String</span><span class="sxs-lookup"><span data-stu-id="38972-148">String</span></span>|<span data-ttu-id="38972-149">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="38972-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="38972-150">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="38972-150">settingDisplayName</span></span>|<span data-ttu-id="38972-151">String</span><span class="sxs-lookup"><span data-stu-id="38972-151">String</span></span>|<span data-ttu-id="38972-152">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="38972-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="38972-153">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="38972-153">settingDisplayValue</span></span>|<span data-ttu-id="38972-154">String</span><span class="sxs-lookup"><span data-stu-id="38972-154">String</span></span>|<span data-ttu-id="38972-155">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="38972-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="38972-156">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="38972-156">settingDisplayValueType</span></span>|<span data-ttu-id="38972-157">String</span><span class="sxs-lookup"><span data-stu-id="38972-157">String</span></span>|<span data-ttu-id="38972-158">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="38972-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="38972-159">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="38972-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="38972-160">String</span><span class="sxs-lookup"><span data-stu-id="38972-160">String</span></span>|<span data-ttu-id="38972-161">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="38972-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="38972-162">settingCategory</span><span class="sxs-lookup"><span data-stu-id="38972-162">settingCategory</span></span>|<span data-ttu-id="38972-163">String</span><span class="sxs-lookup"><span data-stu-id="38972-163">String</span></span>|<span data-ttu-id="38972-164">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="38972-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="38972-165">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="38972-165">mdmCspName</span></span>|<span data-ttu-id="38972-166">String</span><span class="sxs-lookup"><span data-stu-id="38972-166">String</span></span>|<span data-ttu-id="38972-167">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="38972-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="38972-168">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="38972-168">mdmSettingUri</span></span>|<span data-ttu-id="38972-169">String</span><span class="sxs-lookup"><span data-stu-id="38972-169">String</span></span>|<span data-ttu-id="38972-170">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="38972-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="38972-171">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="38972-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="38972-172">Int32</span><span class="sxs-lookup"><span data-stu-id="38972-172">Int32</span></span>|<span data-ttu-id="38972-173">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="38972-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="38972-174">settingType</span><span class="sxs-lookup"><span data-stu-id="38972-174">settingType</span></span>|[<span data-ttu-id="38972-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="38972-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="38972-176">组策略的设置类型（安全性或 admx）。</span><span class="sxs-lookup"><span data-stu-id="38972-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="38972-177">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="38972-177">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="38972-178">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="38972-178">isMdmSupported</span></span>|<span data-ttu-id="38972-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="38972-179">Boolean</span></span>|<span data-ttu-id="38972-180">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="38972-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="38972-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="38972-181">mdmSupportedState</span></span>|[<span data-ttu-id="38972-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="38972-182">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="38972-183">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="38972-183">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="38972-184">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="38972-184">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="38972-185">settingScope</span><span class="sxs-lookup"><span data-stu-id="38972-185">settingScope</span></span>|[<span data-ttu-id="38972-186">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="38972-186">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="38972-187">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="38972-187">The scope of the setting.</span></span> <span data-ttu-id="38972-188">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="38972-188">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="38972-189">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="38972-189">intuneSettingUriList</span></span>|<span data-ttu-id="38972-190">String collection</span><span class="sxs-lookup"><span data-stu-id="38972-190">String collection</span></span>|<span data-ttu-id="38972-191">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="38972-191">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="38972-192">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="38972-192">intuneSettingDefinitionId</span></span>|<span data-ttu-id="38972-193">String</span><span class="sxs-lookup"><span data-stu-id="38972-193">String</span></span>|<span data-ttu-id="38972-194">Intune 设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="38972-194">The Intune Setting Definition Id</span></span>|



## <a name="response"></a><span data-ttu-id="38972-195">响应</span><span class="sxs-lookup"><span data-stu-id="38972-195">Response</span></span>
<span data-ttu-id="38972-196">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38972-196">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38972-197">示例</span><span class="sxs-lookup"><span data-stu-id="38972-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="38972-198">请求</span><span class="sxs-lookup"><span data-stu-id="38972-198">Request</span></span>
<span data-ttu-id="38972-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38972-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 957

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
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="38972-200">响应</span><span class="sxs-lookup"><span data-stu-id="38972-200">Response</span></span>
<span data-ttu-id="38972-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38972-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1006

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
  "intuneSettingDefinitionId": "Intune Setting Definition Id value"
}
```




