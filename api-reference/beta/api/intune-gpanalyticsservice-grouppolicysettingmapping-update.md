---
title: 更新 groupPolicySettingMapping
description: 更新 groupPolicySettingMapping 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75c94b0842afd1c7bd5b6e5c48160fa9b1e65e9e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277958"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="5d5ec-103">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="5d5ec-103">Update groupPolicySettingMapping</span></span>

<span data-ttu-id="5d5ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d5ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d5ec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d5ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d5ec-107">更新 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-107">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d5ec-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5d5ec-108">Prerequisites</span></span>
<span data-ttu-id="5d5ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d5ec-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d5ec-111">Permission type</span></span>|<span data-ttu-id="5d5ec-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d5ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d5ec-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d5ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d5ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d5ec-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d5ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d5ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-116">Not supported.</span></span>|
|<span data-ttu-id="5d5ec-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d5ec-117">Application</span></span>|<span data-ttu-id="5d5ec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5ec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d5ec-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d5ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="5d5ec-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d5ec-120">Request headers</span></span>
|<span data-ttu-id="5d5ec-121">标头</span><span class="sxs-lookup"><span data-stu-id="5d5ec-121">Header</span></span>|<span data-ttu-id="5d5ec-122">值</span><span class="sxs-lookup"><span data-stu-id="5d5ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d5ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d5ec-123">Authorization</span></span>|<span data-ttu-id="5d5ec-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d5ec-125">接受</span><span class="sxs-lookup"><span data-stu-id="5d5ec-125">Accept</span></span>|<span data-ttu-id="5d5ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d5ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d5ec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d5ec-127">Request body</span></span>
<span data-ttu-id="5d5ec-128">在请求正文中，提供 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-128">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="5d5ec-129">下表显示创建 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-129">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="5d5ec-130">属性</span><span class="sxs-lookup"><span data-stu-id="5d5ec-130">Property</span></span>|<span data-ttu-id="5d5ec-131">类型</span><span class="sxs-lookup"><span data-stu-id="5d5ec-131">Type</span></span>|<span data-ttu-id="5d5ec-132">说明</span><span class="sxs-lookup"><span data-stu-id="5d5ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d5ec-133">id</span><span class="sxs-lookup"><span data-stu-id="5d5ec-133">id</span></span>|<span data-ttu-id="5d5ec-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-134">String</span></span>|<span data-ttu-id="5d5ec-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5d5ec-135">Not yet documented</span></span>|
|<span data-ttu-id="5d5ec-136">parentId</span><span class="sxs-lookup"><span data-stu-id="5d5ec-136">parentId</span></span>|<span data-ttu-id="5d5ec-137">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-137">String</span></span>|<span data-ttu-id="5d5ec-138">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-138">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-139">childIdList</span><span class="sxs-lookup"><span data-stu-id="5d5ec-139">childIdList</span></span>|<span data-ttu-id="5d5ec-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="5d5ec-140">String collection</span></span>|<span data-ttu-id="5d5ec-141">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-141">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-142">settingName</span><span class="sxs-lookup"><span data-stu-id="5d5ec-142">settingName</span></span>|<span data-ttu-id="5d5ec-143">String</span><span class="sxs-lookup"><span data-stu-id="5d5ec-143">String</span></span>|<span data-ttu-id="5d5ec-144">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-144">The name of this group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-145">settingValue</span><span class="sxs-lookup"><span data-stu-id="5d5ec-145">settingValue</span></span>|<span data-ttu-id="5d5ec-146">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-146">String</span></span>|<span data-ttu-id="5d5ec-147">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-147">The value of this group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-148">settingValueType</span><span class="sxs-lookup"><span data-stu-id="5d5ec-148">settingValueType</span></span>|<span data-ttu-id="5d5ec-149">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-149">String</span></span>|<span data-ttu-id="5d5ec-150">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-150">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-151">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="5d5ec-151">settingDisplayName</span></span>|<span data-ttu-id="5d5ec-152">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-152">String</span></span>|<span data-ttu-id="5d5ec-153">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-153">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-154">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="5d5ec-154">settingDisplayValue</span></span>|<span data-ttu-id="5d5ec-155">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-155">String</span></span>|<span data-ttu-id="5d5ec-156">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-156">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-157">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="5d5ec-157">settingDisplayValueType</span></span>|<span data-ttu-id="5d5ec-158">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-158">String</span></span>|<span data-ttu-id="5d5ec-159">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-159">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="5d5ec-160">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="5d5ec-160">settingValueDisplayUnits</span></span>|<span data-ttu-id="5d5ec-161">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-161">String</span></span>|<span data-ttu-id="5d5ec-162">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="5d5ec-162">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="5d5ec-163">settingCategory</span><span class="sxs-lookup"><span data-stu-id="5d5ec-163">settingCategory</span></span>|<span data-ttu-id="5d5ec-164">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-164">String</span></span>|<span data-ttu-id="5d5ec-165">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-165">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="5d5ec-166">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="5d5ec-166">mdmCspName</span></span>|<span data-ttu-id="5d5ec-167">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-167">String</span></span>|<span data-ttu-id="5d5ec-168">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-168">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="5d5ec-169">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="5d5ec-169">mdmSettingUri</span></span>|<span data-ttu-id="5d5ec-170">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-170">String</span></span>|<span data-ttu-id="5d5ec-171">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-171">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="5d5ec-172">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="5d5ec-172">mdmMinimumOSVersion</span></span>|<span data-ttu-id="5d5ec-173">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5ec-173">Int32</span></span>|<span data-ttu-id="5d5ec-174">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-174">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="5d5ec-175">settingType</span><span class="sxs-lookup"><span data-stu-id="5d5ec-175">settingType</span></span>|[<span data-ttu-id="5d5ec-176">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="5d5ec-176">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="5d5ec-177">组策略的设置类型 (安全性或 admx) 。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-177">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="5d5ec-178">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-178">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="5d5ec-179">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="5d5ec-179">isMdmSupported</span></span>|<span data-ttu-id="5d5ec-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d5ec-180">Boolean</span></span>|<span data-ttu-id="5d5ec-181">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="5d5ec-181">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="5d5ec-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="5d5ec-182">mdmSupportedState</span></span>|[<span data-ttu-id="5d5ec-183">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="5d5ec-183">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="5d5ec-184">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-184">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="5d5ec-185">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-185">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="5d5ec-186">settingScope</span><span class="sxs-lookup"><span data-stu-id="5d5ec-186">settingScope</span></span>|[<span data-ttu-id="5d5ec-187">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="5d5ec-187">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="5d5ec-188">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-188">The scope of the setting.</span></span> <span data-ttu-id="5d5ec-189">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-189">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="5d5ec-190">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="5d5ec-190">intuneSettingUriList</span></span>|<span data-ttu-id="5d5ec-191">String 集合</span><span class="sxs-lookup"><span data-stu-id="5d5ec-191">String collection</span></span>|<span data-ttu-id="5d5ec-192">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="5d5ec-192">The list of Intune Setting URIs this group policy setting maps to</span></span>|
|<span data-ttu-id="5d5ec-193">intuneSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5d5ec-193">intuneSettingDefinitionId</span></span>|<span data-ttu-id="5d5ec-194">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-194">String</span></span>|<span data-ttu-id="5d5ec-195">Intune 设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="5d5ec-195">The Intune Setting Definition Id</span></span>|
|<span data-ttu-id="5d5ec-196">admxSettingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5d5ec-196">admxSettingDefinitionId</span></span>|<span data-ttu-id="5d5ec-197">字符串</span><span class="sxs-lookup"><span data-stu-id="5d5ec-197">String</span></span>|<span data-ttu-id="5d5ec-198">Admx 组策略 Id</span><span class="sxs-lookup"><span data-stu-id="5d5ec-198">Admx Group Policy Id</span></span>|



## <a name="response"></a><span data-ttu-id="5d5ec-199">响应</span><span class="sxs-lookup"><span data-stu-id="5d5ec-199">Response</span></span>
<span data-ttu-id="5d5ec-200">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-200">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d5ec-201">示例</span><span class="sxs-lookup"><span data-stu-id="5d5ec-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d5ec-202">请求</span><span class="sxs-lookup"><span data-stu-id="5d5ec-202">Request</span></span>
<span data-ttu-id="5d5ec-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d5ec-204">响应</span><span class="sxs-lookup"><span data-stu-id="5d5ec-204">Response</span></span>
<span data-ttu-id="5d5ec-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




