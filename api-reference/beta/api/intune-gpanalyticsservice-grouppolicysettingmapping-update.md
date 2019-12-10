---
title: 更新 groupPolicySettingMapping
description: 更新 groupPolicySettingMapping 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68d5b1f3c48229677889f47c8adfff73e5821e7b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943240"
---
# <a name="update-grouppolicysettingmapping"></a><span data-ttu-id="db821-103">更新 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="db821-103">Update groupPolicySettingMapping</span></span>

> <span data-ttu-id="db821-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db821-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db821-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db821-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db821-106">更新[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db821-106">Update the properties of a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db821-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db821-107">Prerequisites</span></span>
<span data-ttu-id="db821-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db821-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db821-110">Permission type</span></span>|<span data-ttu-id="db821-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db821-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db821-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db821-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db821-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db821-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db821-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db821-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db821-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db821-115">Not supported.</span></span>|
|<span data-ttu-id="db821-116">Application</span><span class="sxs-lookup"><span data-stu-id="db821-116">Application</span></span>|<span data-ttu-id="db821-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db821-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db821-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db821-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a><span data-ttu-id="db821-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db821-119">Request headers</span></span>
|<span data-ttu-id="db821-120">标头</span><span class="sxs-lookup"><span data-stu-id="db821-120">Header</span></span>|<span data-ttu-id="db821-121">值</span><span class="sxs-lookup"><span data-stu-id="db821-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db821-122">授权</span><span class="sxs-lookup"><span data-stu-id="db821-122">Authorization</span></span>|<span data-ttu-id="db821-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db821-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db821-124">接受</span><span class="sxs-lookup"><span data-stu-id="db821-124">Accept</span></span>|<span data-ttu-id="db821-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db821-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db821-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db821-126">Request body</span></span>
<span data-ttu-id="db821-127">在请求正文中，提供[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db821-127">In the request body, supply a JSON representation for the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

<span data-ttu-id="db821-128">下表显示创建[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db821-128">The following table shows the properties that are required when you create the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).</span></span>

|<span data-ttu-id="db821-129">属性</span><span class="sxs-lookup"><span data-stu-id="db821-129">Property</span></span>|<span data-ttu-id="db821-130">类型</span><span class="sxs-lookup"><span data-stu-id="db821-130">Type</span></span>|<span data-ttu-id="db821-131">说明</span><span class="sxs-lookup"><span data-stu-id="db821-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db821-132">id</span><span class="sxs-lookup"><span data-stu-id="db821-132">id</span></span>|<span data-ttu-id="db821-133">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-133">String</span></span>|<span data-ttu-id="db821-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="db821-134">Not yet documented</span></span>|
|<span data-ttu-id="db821-135">parentId</span><span class="sxs-lookup"><span data-stu-id="db821-135">parentId</span></span>|<span data-ttu-id="db821-136">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-136">String</span></span>|<span data-ttu-id="db821-137">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="db821-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="db821-138">childIdList</span><span class="sxs-lookup"><span data-stu-id="db821-138">childIdList</span></span>|<span data-ttu-id="db821-139">String collection</span><span class="sxs-lookup"><span data-stu-id="db821-139">String collection</span></span>|<span data-ttu-id="db821-140">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="db821-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="db821-141">settingName</span><span class="sxs-lookup"><span data-stu-id="db821-141">settingName</span></span>|<span data-ttu-id="db821-142">String</span><span class="sxs-lookup"><span data-stu-id="db821-142">String</span></span>|<span data-ttu-id="db821-143">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="db821-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="db821-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="db821-144">settingValue</span></span>|<span data-ttu-id="db821-145">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-145">String</span></span>|<span data-ttu-id="db821-146">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="db821-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="db821-147">settingValueType</span><span class="sxs-lookup"><span data-stu-id="db821-147">settingValueType</span></span>|<span data-ttu-id="db821-148">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-148">String</span></span>|<span data-ttu-id="db821-149">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="db821-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="db821-150">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="db821-150">settingDisplayName</span></span>|<span data-ttu-id="db821-151">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-151">String</span></span>|<span data-ttu-id="db821-152">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="db821-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="db821-153">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="db821-153">settingDisplayValue</span></span>|<span data-ttu-id="db821-154">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-154">String</span></span>|<span data-ttu-id="db821-155">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="db821-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="db821-156">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="db821-156">settingDisplayValueType</span></span>|<span data-ttu-id="db821-157">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-157">String</span></span>|<span data-ttu-id="db821-158">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="db821-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="db821-159">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="db821-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="db821-160">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-160">String</span></span>|<span data-ttu-id="db821-161">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="db821-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="db821-162">settingCategory</span><span class="sxs-lookup"><span data-stu-id="db821-162">settingCategory</span></span>|<span data-ttu-id="db821-163">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-163">String</span></span>|<span data-ttu-id="db821-164">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="db821-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="db821-165">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="db821-165">mdmCspName</span></span>|<span data-ttu-id="db821-166">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-166">String</span></span>|<span data-ttu-id="db821-167">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="db821-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="db821-168">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="db821-168">mdmSettingUri</span></span>|<span data-ttu-id="db821-169">字符串</span><span class="sxs-lookup"><span data-stu-id="db821-169">String</span></span>|<span data-ttu-id="db821-170">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="db821-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="db821-171">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="db821-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="db821-172">Int32</span><span class="sxs-lookup"><span data-stu-id="db821-172">Int32</span></span>|<span data-ttu-id="db821-173">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="db821-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="db821-174">settingType</span><span class="sxs-lookup"><span data-stu-id="db821-174">settingType</span></span>|[<span data-ttu-id="db821-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="db821-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="db821-176">组策略的设置类型（安全性或 admx）。</span><span class="sxs-lookup"><span data-stu-id="db821-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="db821-177">可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。</span><span class="sxs-lookup"><span data-stu-id="db821-177">Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.</span></span>|
|<span data-ttu-id="db821-178">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="db821-178">isMdmSupported</span></span>|<span data-ttu-id="db821-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="db821-179">Boolean</span></span>|<span data-ttu-id="db821-180">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="db821-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="db821-181">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="db821-181">mdmSupportedState</span></span>|[<span data-ttu-id="db821-182">mdmSupportedState</span><span class="sxs-lookup"><span data-stu-id="db821-182">mdmSupportedState</span></span>](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|<span data-ttu-id="db821-183">指示是否支持 Mdm 中的设置。</span><span class="sxs-lookup"><span data-stu-id="db821-183">Indicates if the setting is supported in Mdm or not.</span></span> <span data-ttu-id="db821-184">可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。</span><span class="sxs-lookup"><span data-stu-id="db821-184">Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.</span></span>|
|<span data-ttu-id="db821-185">settingScope</span><span class="sxs-lookup"><span data-stu-id="db821-185">settingScope</span></span>|[<span data-ttu-id="db821-186">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="db821-186">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="db821-187">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="db821-187">The scope of the setting.</span></span> <span data-ttu-id="db821-188">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="db821-188">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="db821-189">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="db821-189">intuneSettingUriList</span></span>|<span data-ttu-id="db821-190">String collection</span><span class="sxs-lookup"><span data-stu-id="db821-190">String collection</span></span>|<span data-ttu-id="db821-191">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="db821-191">The list of Intune Setting URIs this group policy setting maps to</span></span>|



## <a name="response"></a><span data-ttu-id="db821-192">响应</span><span class="sxs-lookup"><span data-stu-id="db821-192">Response</span></span>
<span data-ttu-id="db821-193">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。</span><span class="sxs-lookup"><span data-stu-id="db821-193">If successful, this method returns a `200 OK` response code and an updated [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db821-194">示例</span><span class="sxs-lookup"><span data-stu-id="db821-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="db821-195">请求</span><span class="sxs-lookup"><span data-stu-id="db821-195">Request</span></span>
<span data-ttu-id="db821-196">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db821-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 887

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="db821-197">响应</span><span class="sxs-lookup"><span data-stu-id="db821-197">Response</span></span>
<span data-ttu-id="db821-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db821-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 936

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
  ]
}
```





