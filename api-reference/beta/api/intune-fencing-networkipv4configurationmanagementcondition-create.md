---
title: 创建 networkIPv4ConfigurationManagementCondition
description: 创建新的 networkIPv4ConfigurationManagementCondition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f93f955628f2379ce191cbb8fd584d52866eaf3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054075"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="568d3-103">创建 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="568d3-103">Create networkIPv4ConfigurationManagementCondition</span></span>

<span data-ttu-id="568d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="568d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="568d3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="568d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="568d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="568d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="568d3-107">创建新的 [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="568d3-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="568d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="568d3-108">Prerequisites</span></span>
<span data-ttu-id="568d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="568d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="568d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="568d3-111">Permission type</span></span>|<span data-ttu-id="568d3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="568d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="568d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="568d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="568d3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568d3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="568d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="568d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="568d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="568d3-116">Not supported.</span></span>|
|<span data-ttu-id="568d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="568d3-117">Application</span></span>|<span data-ttu-id="568d3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568d3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="568d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="568d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="568d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="568d3-120">Request headers</span></span>
|<span data-ttu-id="568d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="568d3-121">Header</span></span>|<span data-ttu-id="568d3-122">值</span><span class="sxs-lookup"><span data-stu-id="568d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="568d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="568d3-123">Authorization</span></span>|<span data-ttu-id="568d3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="568d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="568d3-125">接受</span><span class="sxs-lookup"><span data-stu-id="568d3-125">Accept</span></span>|<span data-ttu-id="568d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="568d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="568d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="568d3-127">Request body</span></span>
<span data-ttu-id="568d3-128">在请求正文中，提供 networkIPv4ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="568d3-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="568d3-129">下表显示创建 networkIPv4ConfigurationManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="568d3-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="568d3-130">属性</span><span class="sxs-lookup"><span data-stu-id="568d3-130">Property</span></span>|<span data-ttu-id="568d3-131">类型</span><span class="sxs-lookup"><span data-stu-id="568d3-131">Type</span></span>|<span data-ttu-id="568d3-132">说明</span><span class="sxs-lookup"><span data-stu-id="568d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="568d3-133">id</span><span class="sxs-lookup"><span data-stu-id="568d3-133">id</span></span>|<span data-ttu-id="568d3-134">String</span><span class="sxs-lookup"><span data-stu-id="568d3-134">String</span></span>|<span data-ttu-id="568d3-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="568d3-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="568d3-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="568d3-136">System generated value assigned when created.</span></span> <span data-ttu-id="568d3-137">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="568d3-138">uniqueName</span></span>|<span data-ttu-id="568d3-139">String</span><span class="sxs-lookup"><span data-stu-id="568d3-139">String</span></span>|<span data-ttu-id="568d3-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="568d3-140">Unique name for the management condition.</span></span> <span data-ttu-id="568d3-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="568d3-141">Used in management condition expressions.</span></span> <span data-ttu-id="568d3-142">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-143">displayName</span><span class="sxs-lookup"><span data-stu-id="568d3-143">displayName</span></span>|<span data-ttu-id="568d3-144">String</span><span class="sxs-lookup"><span data-stu-id="568d3-144">String</span></span>|<span data-ttu-id="568d3-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="568d3-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="568d3-146">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-147">说明</span><span class="sxs-lookup"><span data-stu-id="568d3-147">description</span></span>|<span data-ttu-id="568d3-148">String</span><span class="sxs-lookup"><span data-stu-id="568d3-148">String</span></span>|<span data-ttu-id="568d3-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="568d3-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="568d3-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="568d3-151">createdDateTime</span></span>|<span data-ttu-id="568d3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="568d3-152">DateTimeOffset</span></span>|<span data-ttu-id="568d3-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="568d3-153">The time the management condition was created.</span></span> <span data-ttu-id="568d3-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="568d3-154">Generated service side.</span></span> <span data-ttu-id="568d3-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="568d3-156">modifiedDateTime</span></span>|<span data-ttu-id="568d3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="568d3-157">DateTimeOffset</span></span>|<span data-ttu-id="568d3-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="568d3-158">The time the management condition was last modified.</span></span> <span data-ttu-id="568d3-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="568d3-159">Updated service side.</span></span> <span data-ttu-id="568d3-160">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-161">eTag</span><span class="sxs-lookup"><span data-stu-id="568d3-161">eTag</span></span>|<span data-ttu-id="568d3-162">String</span><span class="sxs-lookup"><span data-stu-id="568d3-162">String</span></span>|<span data-ttu-id="568d3-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="568d3-163">ETag of the management condition.</span></span> <span data-ttu-id="568d3-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="568d3-164">Updated service side.</span></span> <span data-ttu-id="568d3-165">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="568d3-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="568d3-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="568d3-166">applicablePlatforms</span></span>|<span data-ttu-id="568d3-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="568d3-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="568d3-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="568d3-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="568d3-169">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="568d3-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="568d3-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="568d3-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="568d3-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="568d3-171">ipV4Prefix</span></span>|<span data-ttu-id="568d3-172">String</span><span class="sxs-lookup"><span data-stu-id="568d3-172">String</span></span>|<span data-ttu-id="568d3-173">要连接到的 IPv4 子网。</span><span class="sxs-lookup"><span data-stu-id="568d3-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="568d3-174">例如，10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="568d3-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="568d3-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="568d3-175">ipV4Gateway</span></span>|<span data-ttu-id="568d3-176">String</span><span class="sxs-lookup"><span data-stu-id="568d3-176">String</span></span>|<span data-ttu-id="568d3-177">IPv4 网关地址。</span><span class="sxs-lookup"><span data-stu-id="568d3-177">The IPv4 gateway address.</span></span> <span data-ttu-id="568d3-178">例如10.0.0。0</span><span class="sxs-lookup"><span data-stu-id="568d3-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="568d3-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="568d3-179">ipV4DHCPServer</span></span>|<span data-ttu-id="568d3-180">String</span><span class="sxs-lookup"><span data-stu-id="568d3-180">String</span></span>|<span data-ttu-id="568d3-181">适配器的 DHCP 服务器的 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="568d3-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="568d3-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="568d3-182">ipV4DNSServerList</span></span>|<span data-ttu-id="568d3-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="568d3-183">String collection</span></span>|<span data-ttu-id="568d3-184">为适配器配置的 IPv4 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="568d3-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="568d3-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="568d3-185">dnsSuffixList</span></span>|<span data-ttu-id="568d3-186">String 集合</span><span class="sxs-lookup"><span data-stu-id="568d3-186">String collection</span></span>|<span data-ttu-id="568d3-187">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="568d3-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="568d3-188">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="568d3-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="568d3-189">响应</span><span class="sxs-lookup"><span data-stu-id="568d3-189">Response</span></span>
<span data-ttu-id="568d3-190">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="568d3-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="568d3-191">示例</span><span class="sxs-lookup"><span data-stu-id="568d3-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="568d3-192">请求</span><span class="sxs-lookup"><span data-stu-id="568d3-192">Request</span></span>
<span data-ttu-id="568d3-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="568d3-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="568d3-194">响应</span><span class="sxs-lookup"><span data-stu-id="568d3-194">Response</span></span>
<span data-ttu-id="568d3-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="568d3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```






