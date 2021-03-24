---
title: 创建 groupPolicySettingMapping
description: 创建新的 groupPolicySettingMapping 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26639ae0547cc9cb81c10b370f1323b4d5f8663c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135521"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="3a5de-103">创建 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="3a5de-103">Create groupPolicySettingMapping</span></span>

<span data-ttu-id="3a5de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a5de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a5de-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a5de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a5de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a5de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a5de-107">创建新的 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a5de-107">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a5de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3a5de-108">Prerequisites</span></span>
<span data-ttu-id="3a5de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a5de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a5de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a5de-111">Permission type</span></span>|<span data-ttu-id="3a5de-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a5de-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a5de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a5de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a5de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a5de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a5de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a5de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a5de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a5de-116">Not supported.</span></span>|
|<span data-ttu-id="3a5de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a5de-117">Application</span></span>|<span data-ttu-id="3a5de-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a5de-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a5de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a5de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="3a5de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a5de-120">Request headers</span></span>
|<span data-ttu-id="3a5de-121">标头</span><span class="sxs-lookup"><span data-stu-id="3a5de-121">Header</span></span>|<span data-ttu-id="3a5de-122">值</span><span class="sxs-lookup"><span data-stu-id="3a5de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a5de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a5de-123">Authorization</span></span>|<span data-ttu-id="3a5de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3a5de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a5de-125">接受</span><span class="sxs-lookup"><span data-stu-id="3a5de-125">Accept</span></span>|<span data-ttu-id="3a5de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a5de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a5de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a5de-127">Request body</span></span>
<span data-ttu-id="3a5de-128">在请求正文中，提供 groupPolicySettingMapping 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a5de-128">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="3a5de-129">下表显示创建 groupPolicySettingMapping 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3a5de-129">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="3a5de-130">属性</span><span class="sxs-lookup"><span data-stu-id="3a5de-130">Property</span></span>|<span data-ttu-id="3a5de-131">类型</span><span class="sxs-lookup"><span data-stu-id="3a5de-131">Type</span></span>|<span data-ttu-id="3a5de-132">说明</span><span class="sxs-lookup"><span data-stu-id="3a5de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a5de-133">id</span><span class="sxs-lookup"><span data-stu-id="3a5de-133">id</span></span>|<span data-ttu-id="3a5de-134">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-134">String</span></span>|<span data-ttu-id="3a5de-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3a5de-135">Not yet documented</span></span>|
|<span data-ttu-id="3a5de-136">parentId</span><span class="sxs-lookup"><span data-stu-id="3a5de-136">parentId</span></span>|<span data-ttu-id="3a5de-137">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-137">String</span></span>|<span data-ttu-id="3a5de-138">组策略设置的父 ID。</span><span class="sxs-lookup"><span data-stu-id="3a5de-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="3a5de-139">childIdList</span><span class="sxs-lookup"><span data-stu-id="3a5de-139">childIdList</span></span>|<span data-ttu-id="3a5de-140">String collection</span><span class="sxs-lookup"><span data-stu-id="3a5de-140">String collection</span></span>|<span data-ttu-id="3a5de-141">组策略设置的子 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="3a5de-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="3a5de-142">settingName</span><span class="sxs-lookup"><span data-stu-id="3a5de-142">settingName</span></span>|<span data-ttu-id="3a5de-143">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-143">String</span></span>|<span data-ttu-id="3a5de-144">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="3a5de-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="3a5de-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="3a5de-145">settingValue</span></span>|<span data-ttu-id="3a5de-146">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-146">String</span></span>|<span data-ttu-id="3a5de-147">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="3a5de-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="3a5de-148">settingValueType</span><span class="sxs-lookup"><span data-stu-id="3a5de-148">settingValueType</span></span>|<span data-ttu-id="3a5de-149">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-149">String</span></span>|<span data-ttu-id="3a5de-150">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="3a5de-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="3a5de-151">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a5de-151">settingDisplayName</span></span>|<span data-ttu-id="3a5de-152">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-152">String</span></span>|<span data-ttu-id="3a5de-153">此显示名称策略设置的成员。</span><span class="sxs-lookup"><span data-stu-id="3a5de-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="3a5de-154">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="3a5de-154">settingDisplayValue</span></span>|<span data-ttu-id="3a5de-155">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-155">String</span></span>|<span data-ttu-id="3a5de-156">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="3a5de-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="3a5de-157">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="3a5de-157">settingDisplayValueType</span></span>|<span data-ttu-id="3a5de-158">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-158">String</span></span>|<span data-ttu-id="3a5de-159">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="3a5de-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="3a5de-160">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="3a5de-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="3a5de-161">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-161">String</span></span>|<span data-ttu-id="3a5de-162">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="3a5de-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="3a5de-163">settingCategory</span><span class="sxs-lookup"><span data-stu-id="3a5de-163">settingCategory</span></span>|<span data-ttu-id="3a5de-164">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-164">String</span></span>|<span data-ttu-id="3a5de-165">组策略设置位于的类别。</span><span class="sxs-lookup"><span data-stu-id="3a5de-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="3a5de-166">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="3a5de-166">mdmCspName</span></span>|<span data-ttu-id="3a5de-167">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-167">String</span></span>|<span data-ttu-id="3a5de-168">此组策略设置映射到的云解决方案提供商名称。</span><span class="sxs-lookup"><span data-stu-id="3a5de-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="3a5de-169">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="3a5de-169">mdmSettingUri</span></span>|<span data-ttu-id="3a5de-170">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-170">String</span></span>|<span data-ttu-id="3a5de-171">此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="3a5de-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="3a5de-172">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="3a5de-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="3a5de-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3a5de-173">Int32</span></span>|<span data-ttu-id="3a5de-174">此 mdm 设置支持的最低操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3a5de-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="3a5de-175">settingType</span><span class="sxs-lookup"><span data-stu-id="3a5de-175">settingType</span></span>|[<span data-ttu-id="3a5de-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="3a5de-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="3a5de-177">设置类型 (安全或 admx) 组策略。</span><span class="sxs-lookup"><span data-stu-id="3a5de-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="3a5de-178">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="3a5de-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="3a5de-179">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="3a5de-179">isMdmSupported</span></span>|<span data-ttu-id="3a5de-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a5de-180">Boolean</span></span>|<span data-ttu-id="3a5de-181">指示 Intune 是否支持该设置</span><span class="sxs-lookup"><span data-stu-id="3a5de-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="3a5de-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="3a5de-182">mdmSupportedState</span></span>|[<span data-ttu-id="3a5de-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="3a5de-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="3a5de-184">指示设置在 Mdm 中是否受支持。</span><span class="sxs-lookup"><span data-stu-id="3a5de-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="3a5de-185">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="3a5de-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="3a5de-186">settingScope</span><span class="sxs-lookup"><span data-stu-id="3a5de-186">settingScope</span></span>|[<span data-ttu-id="3a5de-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="3a5de-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="3a5de-188">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="3a5de-188">The scope of the setting.</span></span> <span data-ttu-id="3a5de-189">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="3a5de-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="3a5de-190">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="3a5de-190">intuneSettingUriList</span></span>|<span data-ttu-id="3a5de-191">String collection</span><span class="sxs-lookup"><span data-stu-id="3a5de-191">String collection</span></span>|<span data-ttu-id="3a5de-192">此组策略设置映射到的 Intune 设置 URI 列表</span><span class="sxs-lookup"><span data-stu-id="3a5de-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="3a5de-193">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3a5de-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="3a5de-194">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-194">String</span></span>|<span data-ttu-id="3a5de-195">Intune 设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="3a5de-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="3a5de-196">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3a5de-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="3a5de-197">String</span><span class="sxs-lookup"><span data-stu-id="3a5de-197">String</span></span>|<span data-ttu-id="3a5de-198">Admx 组策略 ID</span><span class="sxs-lookup"><span data-stu-id="3a5de-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="3a5de-199">响应</span><span class="sxs-lookup"><span data-stu-id="3a5de-199">Response</span></span>
<span data-ttu-id="3a5de-200">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a5de-200">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a5de-201">示例</span><span class="sxs-lookup"><span data-stu-id="3a5de-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a5de-202">请求</span><span class="sxs-lookup"><span data-stu-id="3a5de-202">Request</span></span>
<span data-ttu-id="3a5de-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a5de-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
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

### <a name="response"></a><span data-ttu-id="3a5de-204">响应</span><span class="sxs-lookup"><span data-stu-id="3a5de-204">Response</span></span>
<span data-ttu-id="3a5de-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a5de-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




