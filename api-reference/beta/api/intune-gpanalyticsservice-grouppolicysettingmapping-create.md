---
title: 创建 groupPolicySettingMapping
description: 创建新的 groupPolicySettingMapping 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efa2f00c5bdc11e46e88e43aa6244bc2120fe5f1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535770"
---
# <a name="create-grouppolicysettingmapping"></a><span data-ttu-id="2caa0-103">创建 groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="2caa0-103">Create groupPolicySettingMapping</span></span>

> <span data-ttu-id="2caa0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2caa0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2caa0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2caa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2caa0-106">创建新的[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2caa0-106">Create a new [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2caa0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2caa0-107">Prerequisites</span></span>
<span data-ttu-id="2caa0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2caa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2caa0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2caa0-110">Permission type</span></span>|<span data-ttu-id="2caa0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2caa0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2caa0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2caa0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2caa0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2caa0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2caa0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2caa0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2caa0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2caa0-115">Not supported.</span></span>|
|<span data-ttu-id="2caa0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2caa0-116">Application</span></span>|<span data-ttu-id="2caa0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2caa0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2caa0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2caa0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="2caa0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2caa0-119">Request headers</span></span>
|<span data-ttu-id="2caa0-120">标头</span><span class="sxs-lookup"><span data-stu-id="2caa0-120">Header</span></span>|<span data-ttu-id="2caa0-121">值</span><span class="sxs-lookup"><span data-stu-id="2caa0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2caa0-122">授权</span><span class="sxs-lookup"><span data-stu-id="2caa0-122">Authorization</span></span>|<span data-ttu-id="2caa0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2caa0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2caa0-124">接受</span><span class="sxs-lookup"><span data-stu-id="2caa0-124">Accept</span></span>|<span data-ttu-id="2caa0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2caa0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2caa0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2caa0-126">Request body</span></span>
<span data-ttu-id="2caa0-127">在请求正文中，提供 groupPolicySettingMapping 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2caa0-127">In the request body, supply a JSON representation for the groupPolicySettingMapping object.</span></span>

<span data-ttu-id="2caa0-128">下表显示创建 groupPolicySettingMapping 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2caa0-128">The following table shows the properties that are required when you create the groupPolicySettingMapping.</span></span>

|<span data-ttu-id="2caa0-129">属性</span><span class="sxs-lookup"><span data-stu-id="2caa0-129">Property</span></span>|<span data-ttu-id="2caa0-130">类型</span><span class="sxs-lookup"><span data-stu-id="2caa0-130">Type</span></span>|<span data-ttu-id="2caa0-131">说明</span><span class="sxs-lookup"><span data-stu-id="2caa0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2caa0-132">id</span><span class="sxs-lookup"><span data-stu-id="2caa0-132">id</span></span>|<span data-ttu-id="2caa0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-133">String</span></span>|<span data-ttu-id="2caa0-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2caa0-134">Not yet documented</span></span>|
|<span data-ttu-id="2caa0-135">parentId</span><span class="sxs-lookup"><span data-stu-id="2caa0-135">parentId</span></span>|<span data-ttu-id="2caa0-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-136">String</span></span>|<span data-ttu-id="2caa0-137">组策略设置的父 Id。</span><span class="sxs-lookup"><span data-stu-id="2caa0-137">Parent Id of the group policy setting.</span></span>|
|<span data-ttu-id="2caa0-138">childIdList</span><span class="sxs-lookup"><span data-stu-id="2caa0-138">childIdList</span></span>|<span data-ttu-id="2caa0-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="2caa0-139">String collection</span></span>|<span data-ttu-id="2caa0-140">组策略设置的子 Id 列表。</span><span class="sxs-lookup"><span data-stu-id="2caa0-140">List of Child Ids of the group policy setting.</span></span>|
|<span data-ttu-id="2caa0-141">settingName</span><span class="sxs-lookup"><span data-stu-id="2caa0-141">settingName</span></span>|<span data-ttu-id="2caa0-142">String</span><span class="sxs-lookup"><span data-stu-id="2caa0-142">String</span></span>|<span data-ttu-id="2caa0-143">此组策略设置的名称。</span><span class="sxs-lookup"><span data-stu-id="2caa0-143">The name of this group policy setting.</span></span>|
|<span data-ttu-id="2caa0-144">settingValue</span><span class="sxs-lookup"><span data-stu-id="2caa0-144">settingValue</span></span>|<span data-ttu-id="2caa0-145">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-145">String</span></span>|<span data-ttu-id="2caa0-146">此组策略设置的值。</span><span class="sxs-lookup"><span data-stu-id="2caa0-146">The value of this group policy setting.</span></span>|
|<span data-ttu-id="2caa0-147">settingValueType</span><span class="sxs-lookup"><span data-stu-id="2caa0-147">settingValueType</span></span>|<span data-ttu-id="2caa0-148">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-148">String</span></span>|<span data-ttu-id="2caa0-149">此组策略设置的值类型。</span><span class="sxs-lookup"><span data-stu-id="2caa0-149">The value type of this group policy setting.</span></span>|
|<span data-ttu-id="2caa0-150">settingDisplayName</span><span class="sxs-lookup"><span data-stu-id="2caa0-150">settingDisplayName</span></span>|<span data-ttu-id="2caa0-151">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-151">String</span></span>|<span data-ttu-id="2caa0-152">此组策略设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2caa0-152">The display name of this group policy setting.</span></span>|
|<span data-ttu-id="2caa0-153">settingDisplayValue</span><span class="sxs-lookup"><span data-stu-id="2caa0-153">settingDisplayValue</span></span>|<span data-ttu-id="2caa0-154">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-154">String</span></span>|<span data-ttu-id="2caa0-155">此组策略设置的显示值。</span><span class="sxs-lookup"><span data-stu-id="2caa0-155">The display value of this group policy setting.</span></span>|
|<span data-ttu-id="2caa0-156">settingDisplayValueType</span><span class="sxs-lookup"><span data-stu-id="2caa0-156">settingDisplayValueType</span></span>|<span data-ttu-id="2caa0-157">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-157">String</span></span>|<span data-ttu-id="2caa0-158">此组策略设置的显示值类型。</span><span class="sxs-lookup"><span data-stu-id="2caa0-158">The display value type of this group policy setting.</span></span>|
|<span data-ttu-id="2caa0-159">settingValueDisplayUnits</span><span class="sxs-lookup"><span data-stu-id="2caa0-159">settingValueDisplayUnits</span></span>|<span data-ttu-id="2caa0-160">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-160">String</span></span>|<span data-ttu-id="2caa0-161">此组策略设置值的显示单位</span><span class="sxs-lookup"><span data-stu-id="2caa0-161">The display units of this group policy setting value</span></span>|
|<span data-ttu-id="2caa0-162">settingCategory</span><span class="sxs-lookup"><span data-stu-id="2caa0-162">settingCategory</span></span>|<span data-ttu-id="2caa0-163">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-163">String</span></span>|<span data-ttu-id="2caa0-164">组策略设置所属的类别。</span><span class="sxs-lookup"><span data-stu-id="2caa0-164">The category the group policy setting is in.</span></span>|
|<span data-ttu-id="2caa0-165">mdmCspName</span><span class="sxs-lookup"><span data-stu-id="2caa0-165">mdmCspName</span></span>|<span data-ttu-id="2caa0-166">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-166">String</span></span>|<span data-ttu-id="2caa0-167">将此组策略设置映射到的 CSP 名称。</span><span class="sxs-lookup"><span data-stu-id="2caa0-167">The CSP name this group policy setting maps to.</span></span>|
|<span data-ttu-id="2caa0-168">mdmSettingUri</span><span class="sxs-lookup"><span data-stu-id="2caa0-168">mdmSettingUri</span></span>|<span data-ttu-id="2caa0-169">字符串</span><span class="sxs-lookup"><span data-stu-id="2caa0-169">String</span></span>|<span data-ttu-id="2caa0-170">将此组策略设置映射到的 MDM CSP URI。</span><span class="sxs-lookup"><span data-stu-id="2caa0-170">The MDM CSP URI this group policy setting maps to.</span></span>|
|<span data-ttu-id="2caa0-171">mdmMinimumOSVersion</span><span class="sxs-lookup"><span data-stu-id="2caa0-171">mdmMinimumOSVersion</span></span>|<span data-ttu-id="2caa0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="2caa0-172">Int32</span></span>|<span data-ttu-id="2caa0-173">此 mdm 设置支持的最低 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="2caa0-173">The minimum OS version this mdm setting supports.</span></span>|
|<span data-ttu-id="2caa0-174">settingType</span><span class="sxs-lookup"><span data-stu-id="2caa0-174">settingType</span></span>|[<span data-ttu-id="2caa0-175">groupPolicySettingType</span><span class="sxs-lookup"><span data-stu-id="2caa0-175">groupPolicySettingType</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|<span data-ttu-id="2caa0-176">组策略的设置类型（安全性或 admx）。</span><span class="sxs-lookup"><span data-stu-id="2caa0-176">The setting type (security or admx) of the Group Policy.</span></span> <span data-ttu-id="2caa0-177">可取值为：`unknown`、`policy`、`account`。</span><span class="sxs-lookup"><span data-stu-id="2caa0-177">Possible values are: `unknown`, `policy`, `account`.</span></span>|
|<span data-ttu-id="2caa0-178">isMdmSupported</span><span class="sxs-lookup"><span data-stu-id="2caa0-178">isMdmSupported</span></span>|<span data-ttu-id="2caa0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2caa0-179">Boolean</span></span>|<span data-ttu-id="2caa0-180">指示此设置是否由 Intune 支持</span><span class="sxs-lookup"><span data-stu-id="2caa0-180">Indicates if the setting is supported by Intune or not</span></span>|
|<span data-ttu-id="2caa0-181">settingScope</span><span class="sxs-lookup"><span data-stu-id="2caa0-181">settingScope</span></span>|[<span data-ttu-id="2caa0-182">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="2caa0-182">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="2caa0-183">设置的范围。</span><span class="sxs-lookup"><span data-stu-id="2caa0-183">The scope of the setting.</span></span> <span data-ttu-id="2caa0-184">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="2caa0-184">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="2caa0-185">intuneSettingUriList</span><span class="sxs-lookup"><span data-stu-id="2caa0-185">intuneSettingUriList</span></span>|<span data-ttu-id="2caa0-186">String 集合</span><span class="sxs-lookup"><span data-stu-id="2caa0-186">String collection</span></span>|<span data-ttu-id="2caa0-187">此组策略设置映射到的 Intune 设置 Uri 列表</span><span class="sxs-lookup"><span data-stu-id="2caa0-187">The list of Intune Setting URIs this group policy setting maps to</span></span>|



## <a name="response"></a><span data-ttu-id="2caa0-188">响应</span><span class="sxs-lookup"><span data-stu-id="2caa0-188">Response</span></span>
<span data-ttu-id="2caa0-189">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2caa0-189">If successful, this method returns a `201 Created` response code and a [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2caa0-190">示例</span><span class="sxs-lookup"><span data-stu-id="2caa0-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="2caa0-191">请求</span><span class="sxs-lookup"><span data-stu-id="2caa0-191">Request</span></span>
<span data-ttu-id="2caa0-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2caa0-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 850

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
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="2caa0-193">响应</span><span class="sxs-lookup"><span data-stu-id="2caa0-193">Response</span></span>
<span data-ttu-id="2caa0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2caa0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 899

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
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```






