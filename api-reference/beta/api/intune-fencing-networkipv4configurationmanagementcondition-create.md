---
title: 创建 networkIPv4ConfigurationManagementCondition
description: 创建新的 networkIPv4ConfigurationManagementCondition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be7b103dc67f8de11bee0b2059342f5180afa7d6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153599"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="4f647-103">创建 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="4f647-103">Create networkIPv4ConfigurationManagementCondition</span></span>

<span data-ttu-id="4f647-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f647-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f647-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f647-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f647-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f647-107">创建新的 [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f647-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f647-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f647-108">Prerequisites</span></span>
<span data-ttu-id="4f647-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f647-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f647-111">Permission type</span></span>|<span data-ttu-id="4f647-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f647-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f647-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f647-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f647-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f647-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f647-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f647-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f647-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f647-116">Not supported.</span></span>|
|<span data-ttu-id="4f647-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f647-117">Application</span></span>|<span data-ttu-id="4f647-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f647-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f647-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f647-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="4f647-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f647-120">Request headers</span></span>
|<span data-ttu-id="4f647-121">标头</span><span class="sxs-lookup"><span data-stu-id="4f647-121">Header</span></span>|<span data-ttu-id="4f647-122">值</span><span class="sxs-lookup"><span data-stu-id="4f647-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f647-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f647-123">Authorization</span></span>|<span data-ttu-id="4f647-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f647-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f647-125">接受</span><span class="sxs-lookup"><span data-stu-id="4f647-125">Accept</span></span>|<span data-ttu-id="4f647-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f647-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f647-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f647-127">Request body</span></span>
<span data-ttu-id="4f647-128">在请求正文中，提供 networkIPv4ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f647-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="4f647-129">下表显示创建 networkIPv4ConfigurationManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4f647-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="4f647-130">属性</span><span class="sxs-lookup"><span data-stu-id="4f647-130">Property</span></span>|<span data-ttu-id="4f647-131">类型</span><span class="sxs-lookup"><span data-stu-id="4f647-131">Type</span></span>|<span data-ttu-id="4f647-132">说明</span><span class="sxs-lookup"><span data-stu-id="4f647-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f647-133">id</span><span class="sxs-lookup"><span data-stu-id="4f647-133">id</span></span>|<span data-ttu-id="4f647-134">String</span><span class="sxs-lookup"><span data-stu-id="4f647-134">String</span></span>|<span data-ttu-id="4f647-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f647-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="4f647-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="4f647-136">System generated value assigned when created.</span></span> <span data-ttu-id="4f647-137">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="4f647-138">uniqueName</span></span>|<span data-ttu-id="4f647-139">String</span><span class="sxs-lookup"><span data-stu-id="4f647-139">String</span></span>|<span data-ttu-id="4f647-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="4f647-140">Unique name for the management condition.</span></span> <span data-ttu-id="4f647-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="4f647-141">Used in management condition expressions.</span></span> <span data-ttu-id="4f647-142">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4f647-143">displayName</span></span>|<span data-ttu-id="4f647-144">String</span><span class="sxs-lookup"><span data-stu-id="4f647-144">String</span></span>|<span data-ttu-id="4f647-145">管理员定义的管理条件名称。</span><span class="sxs-lookup"><span data-stu-id="4f647-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="4f647-146">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-147">说明</span><span class="sxs-lookup"><span data-stu-id="4f647-147">description</span></span>|<span data-ttu-id="4f647-148">String</span><span class="sxs-lookup"><span data-stu-id="4f647-148">String</span></span>|<span data-ttu-id="4f647-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="4f647-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="4f647-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f647-151">createdDateTime</span></span>|<span data-ttu-id="4f647-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f647-152">DateTimeOffset</span></span>|<span data-ttu-id="4f647-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="4f647-153">The time the management condition was created.</span></span> <span data-ttu-id="4f647-154">生成的服务器端。</span><span class="sxs-lookup"><span data-stu-id="4f647-154">Generated service side.</span></span> <span data-ttu-id="4f647-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f647-156">modifiedDateTime</span></span>|<span data-ttu-id="4f647-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f647-157">DateTimeOffset</span></span>|<span data-ttu-id="4f647-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="4f647-158">The time the management condition was last modified.</span></span> <span data-ttu-id="4f647-159">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="4f647-159">Updated service side.</span></span> <span data-ttu-id="4f647-160">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-161">eTag</span><span class="sxs-lookup"><span data-stu-id="4f647-161">eTag</span></span>|<span data-ttu-id="4f647-162">String</span><span class="sxs-lookup"><span data-stu-id="4f647-162">String</span></span>|<span data-ttu-id="4f647-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="4f647-163">ETag of the management condition.</span></span> <span data-ttu-id="4f647-164">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="4f647-164">Updated service side.</span></span> <span data-ttu-id="4f647-165">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="4f647-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="4f647-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="4f647-166">applicablePlatforms</span></span>|<span data-ttu-id="4f647-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f647-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="4f647-168">此管理条件的适用平台。</span><span class="sxs-lookup"><span data-stu-id="4f647-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="4f647-169">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="4f647-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="4f647-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="4f647-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="4f647-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="4f647-171">ipV4Prefix</span></span>|<span data-ttu-id="4f647-172">String</span><span class="sxs-lookup"><span data-stu-id="4f647-172">String</span></span>|<span data-ttu-id="4f647-173">要连接到的 IPv4 子网。</span><span class="sxs-lookup"><span data-stu-id="4f647-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="4f647-174">例如 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="4f647-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="4f647-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="4f647-175">ipV4Gateway</span></span>|<span data-ttu-id="4f647-176">String</span><span class="sxs-lookup"><span data-stu-id="4f647-176">String</span></span>|<span data-ttu-id="4f647-177">IPv4 网关地址。</span><span class="sxs-lookup"><span data-stu-id="4f647-177">The IPv4 gateway address.</span></span> <span data-ttu-id="4f647-178">例如 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="4f647-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="4f647-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="4f647-179">ipV4DHCPServer</span></span>|<span data-ttu-id="4f647-180">String</span><span class="sxs-lookup"><span data-stu-id="4f647-180">String</span></span>|<span data-ttu-id="4f647-181">适配器的 DHCP 服务器的 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="4f647-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="4f647-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="4f647-182">ipV4DNSServerList</span></span>|<span data-ttu-id="4f647-183">String collection</span><span class="sxs-lookup"><span data-stu-id="4f647-183">String collection</span></span>|<span data-ttu-id="4f647-184">为适配器配置的 IPv4 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="4f647-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="4f647-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="4f647-185">dnsSuffixList</span></span>|<span data-ttu-id="4f647-186">String collection</span><span class="sxs-lookup"><span data-stu-id="4f647-186">String collection</span></span>|<span data-ttu-id="4f647-187">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="4f647-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="4f647-188">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="4f647-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="4f647-189">响应</span><span class="sxs-lookup"><span data-stu-id="4f647-189">Response</span></span>
<span data-ttu-id="4f647-190">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f647-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f647-191">示例</span><span class="sxs-lookup"><span data-stu-id="4f647-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f647-192">请求</span><span class="sxs-lookup"><span data-stu-id="4f647-192">Request</span></span>
<span data-ttu-id="4f647-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f647-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f647-194">响应</span><span class="sxs-lookup"><span data-stu-id="4f647-194">Response</span></span>
<span data-ttu-id="4f647-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f647-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




