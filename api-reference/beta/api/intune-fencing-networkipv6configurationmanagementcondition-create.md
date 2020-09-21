---
title: 创建 networkIPv6ConfigurationManagementCondition
description: 创建新的 networkIPv6ConfigurationManagementCondition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3fec737657928d92f1c3ff2975e2b1a0922c7d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969982"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="dda6d-103">创建 networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="dda6d-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="dda6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dda6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dda6d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dda6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dda6d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dda6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dda6d-107">创建新的 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dda6d-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dda6d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dda6d-108">Prerequisites</span></span>
<span data-ttu-id="dda6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dda6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dda6d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dda6d-111">Permission type</span></span>|<span data-ttu-id="dda6d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dda6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dda6d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dda6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dda6d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda6d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dda6d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dda6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dda6d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dda6d-116">Not supported.</span></span>|
|<span data-ttu-id="dda6d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dda6d-117">Application</span></span>|<span data-ttu-id="dda6d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda6d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dda6d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dda6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="dda6d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dda6d-120">Request headers</span></span>
|<span data-ttu-id="dda6d-121">标头</span><span class="sxs-lookup"><span data-stu-id="dda6d-121">Header</span></span>|<span data-ttu-id="dda6d-122">值</span><span class="sxs-lookup"><span data-stu-id="dda6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dda6d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dda6d-123">Authorization</span></span>|<span data-ttu-id="dda6d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dda6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dda6d-125">接受</span><span class="sxs-lookup"><span data-stu-id="dda6d-125">Accept</span></span>|<span data-ttu-id="dda6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dda6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dda6d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dda6d-127">Request body</span></span>
<span data-ttu-id="dda6d-128">在请求正文中，提供 networkIPv6ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dda6d-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="dda6d-129">下表显示创建 networkIPv6ConfigurationManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dda6d-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="dda6d-130">属性</span><span class="sxs-lookup"><span data-stu-id="dda6d-130">Property</span></span>|<span data-ttu-id="dda6d-131">类型</span><span class="sxs-lookup"><span data-stu-id="dda6d-131">Type</span></span>|<span data-ttu-id="dda6d-132">说明</span><span class="sxs-lookup"><span data-stu-id="dda6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dda6d-133">id</span><span class="sxs-lookup"><span data-stu-id="dda6d-133">id</span></span>|<span data-ttu-id="dda6d-134">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-134">String</span></span>|<span data-ttu-id="dda6d-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dda6d-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="dda6d-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="dda6d-136">System generated value assigned when created.</span></span> <span data-ttu-id="dda6d-137">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="dda6d-138">uniqueName</span></span>|<span data-ttu-id="dda6d-139">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-139">String</span></span>|<span data-ttu-id="dda6d-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="dda6d-140">Unique name for the management condition.</span></span> <span data-ttu-id="dda6d-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="dda6d-141">Used in management condition expressions.</span></span> <span data-ttu-id="dda6d-142">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="dda6d-143">displayName</span></span>|<span data-ttu-id="dda6d-144">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-144">String</span></span>|<span data-ttu-id="dda6d-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="dda6d-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="dda6d-146">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-147">description</span><span class="sxs-lookup"><span data-stu-id="dda6d-147">description</span></span>|<span data-ttu-id="dda6d-148">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-148">String</span></span>|<span data-ttu-id="dda6d-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="dda6d-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="dda6d-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dda6d-151">createdDateTime</span></span>|<span data-ttu-id="dda6d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dda6d-152">DateTimeOffset</span></span>|<span data-ttu-id="dda6d-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="dda6d-153">The time the management condition was created.</span></span> <span data-ttu-id="dda6d-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="dda6d-154">Generated service side.</span></span> <span data-ttu-id="dda6d-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dda6d-156">modifiedDateTime</span></span>|<span data-ttu-id="dda6d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dda6d-157">DateTimeOffset</span></span>|<span data-ttu-id="dda6d-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="dda6d-158">The time the management condition was last modified.</span></span> <span data-ttu-id="dda6d-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="dda6d-159">Updated service side.</span></span> <span data-ttu-id="dda6d-160">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-161">eTag</span><span class="sxs-lookup"><span data-stu-id="dda6d-161">eTag</span></span>|<span data-ttu-id="dda6d-162">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-162">String</span></span>|<span data-ttu-id="dda6d-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="dda6d-163">ETag of the management condition.</span></span> <span data-ttu-id="dda6d-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="dda6d-164">Updated service side.</span></span> <span data-ttu-id="dda6d-165">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dda6d-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dda6d-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="dda6d-166">applicablePlatforms</span></span>|<span data-ttu-id="dda6d-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dda6d-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="dda6d-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="dda6d-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="dda6d-169">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="dda6d-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="dda6d-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="dda6d-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="dda6d-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="dda6d-171">ipV6Prefix</span></span>|<span data-ttu-id="dda6d-172">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-172">String</span></span>|<span data-ttu-id="dda6d-173">要连接到的 IPv6 子网。</span><span class="sxs-lookup"><span data-stu-id="dda6d-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="dda6d-174">例如2001： db8：：/32</span><span class="sxs-lookup"><span data-stu-id="dda6d-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="dda6d-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="dda6d-175">ipV6Gateway</span></span>|<span data-ttu-id="dda6d-176">String</span><span class="sxs-lookup"><span data-stu-id="dda6d-176">String</span></span>|<span data-ttu-id="dda6d-177">IPv6 网关地址。</span><span class="sxs-lookup"><span data-stu-id="dda6d-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="dda6d-178">例如2001： db8：：1</span><span class="sxs-lookup"><span data-stu-id="dda6d-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="dda6d-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="dda6d-179">ipV6DNSServerList</span></span>|<span data-ttu-id="dda6d-180">String collection</span><span class="sxs-lookup"><span data-stu-id="dda6d-180">String collection</span></span>|<span data-ttu-id="dda6d-181">为适配器配置的 IPv6 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="dda6d-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="dda6d-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="dda6d-182">dnsSuffixList</span></span>|<span data-ttu-id="dda6d-183">String collection</span><span class="sxs-lookup"><span data-stu-id="dda6d-183">String collection</span></span>|<span data-ttu-id="dda6d-184">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="dda6d-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="dda6d-185">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="dda6d-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="dda6d-186">响应</span><span class="sxs-lookup"><span data-stu-id="dda6d-186">Response</span></span>
<span data-ttu-id="dda6d-187">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dda6d-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dda6d-188">示例</span><span class="sxs-lookup"><span data-stu-id="dda6d-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="dda6d-189">请求</span><span class="sxs-lookup"><span data-stu-id="dda6d-189">Request</span></span>
<span data-ttu-id="dda6d-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dda6d-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dda6d-191">响应</span><span class="sxs-lookup"><span data-stu-id="dda6d-191">Response</span></span>
<span data-ttu-id="dda6d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dda6d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```






