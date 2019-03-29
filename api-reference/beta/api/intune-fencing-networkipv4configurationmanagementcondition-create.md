---
title: 创建 networkIPv4ConfigurationManagementCondition
description: 创建新的 networkIPv4ConfigurationManagementCondition 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e045c50df3e2ce74ed3bc4d4420c506ef5e7a651
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966171"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="66c5d-103">创建 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="66c5d-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="66c5d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66c5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66c5d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66c5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66c5d-106">创建新的[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66c5d-106">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66c5d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="66c5d-107">Prerequisites</span></span>
<span data-ttu-id="66c5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66c5d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66c5d-110">Permission type</span></span>|<span data-ttu-id="66c5d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66c5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66c5d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66c5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66c5d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66c5d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66c5d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66c5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66c5d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66c5d-115">Not supported.</span></span>|
|<span data-ttu-id="66c5d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66c5d-116">Application</span></span>|<span data-ttu-id="66c5d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="66c5d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66c5d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66c5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="66c5d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="66c5d-119">Request headers</span></span>
|<span data-ttu-id="66c5d-120">标头</span><span class="sxs-lookup"><span data-stu-id="66c5d-120">Header</span></span>|<span data-ttu-id="66c5d-121">值</span><span class="sxs-lookup"><span data-stu-id="66c5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66c5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66c5d-122">Authorization</span></span>|<span data-ttu-id="66c5d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66c5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66c5d-124">接受</span><span class="sxs-lookup"><span data-stu-id="66c5d-124">Accept</span></span>|<span data-ttu-id="66c5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66c5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66c5d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66c5d-126">Request body</span></span>
<span data-ttu-id="66c5d-127">在请求正文中, 提供 networkIPv4ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66c5d-127">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="66c5d-128">下表显示创建 networkIPv4ConfigurationManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66c5d-128">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="66c5d-129">属性</span><span class="sxs-lookup"><span data-stu-id="66c5d-129">Property</span></span>|<span data-ttu-id="66c5d-130">类型</span><span class="sxs-lookup"><span data-stu-id="66c5d-130">Type</span></span>|<span data-ttu-id="66c5d-131">说明</span><span class="sxs-lookup"><span data-stu-id="66c5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c5d-132">id</span><span class="sxs-lookup"><span data-stu-id="66c5d-132">id</span></span>|<span data-ttu-id="66c5d-133">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-133">String</span></span>|<span data-ttu-id="66c5d-134">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="66c5d-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="66c5d-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="66c5d-135">System generated value assigned when created.</span></span> <span data-ttu-id="66c5d-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="66c5d-137">uniqueName</span></span>|<span data-ttu-id="66c5d-138">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-138">String</span></span>|<span data-ttu-id="66c5d-139">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="66c5d-139">Unique name for the management condition.</span></span> <span data-ttu-id="66c5d-140">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="66c5d-140">Used in management condition expressions.</span></span> <span data-ttu-id="66c5d-141">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="66c5d-142">displayName</span></span>|<span data-ttu-id="66c5d-143">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-143">String</span></span>|<span data-ttu-id="66c5d-144">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="66c5d-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="66c5d-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-146">description</span><span class="sxs-lookup"><span data-stu-id="66c5d-146">description</span></span>|<span data-ttu-id="66c5d-147">字符串</span><span class="sxs-lookup"><span data-stu-id="66c5d-147">String</span></span>|<span data-ttu-id="66c5d-148">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="66c5d-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="66c5d-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66c5d-150">createdDateTime</span></span>|<span data-ttu-id="66c5d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c5d-151">DateTimeOffset</span></span>|<span data-ttu-id="66c5d-152">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="66c5d-152">The time the management condition was created.</span></span> <span data-ttu-id="66c5d-153">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="66c5d-153">Generated service side.</span></span> <span data-ttu-id="66c5d-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66c5d-155">modifiedDateTime</span></span>|<span data-ttu-id="66c5d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c5d-156">DateTimeOffset</span></span>|<span data-ttu-id="66c5d-157">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="66c5d-157">The time the management condition was last modified.</span></span> <span data-ttu-id="66c5d-158">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="66c5d-158">Updated service side.</span></span> <span data-ttu-id="66c5d-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-160">eTag</span><span class="sxs-lookup"><span data-stu-id="66c5d-160">eTag</span></span>|<span data-ttu-id="66c5d-161">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-161">String</span></span>|<span data-ttu-id="66c5d-162">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="66c5d-162">ETag of the management condition.</span></span> <span data-ttu-id="66c5d-163">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="66c5d-163">Updated service side.</span></span> <span data-ttu-id="66c5d-164">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66c5d-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66c5d-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="66c5d-165">applicablePlatforms</span></span>|<span data-ttu-id="66c5d-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="66c5d-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="66c5d-167">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="66c5d-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="66c5d-168">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="66c5d-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="66c5d-169">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="66c5d-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="66c5d-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="66c5d-170">ipV4Prefix</span></span>|<span data-ttu-id="66c5d-171">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-171">String</span></span>|<span data-ttu-id="66c5d-172">要连接到的 IPv4 子网。</span><span class="sxs-lookup"><span data-stu-id="66c5d-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="66c5d-173">例如, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="66c5d-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="66c5d-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="66c5d-174">ipV4Gateway</span></span>|<span data-ttu-id="66c5d-175">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-175">String</span></span>|<span data-ttu-id="66c5d-176">IPv4 网关地址。</span><span class="sxs-lookup"><span data-stu-id="66c5d-176">The IPv4 gateway address.</span></span> <span data-ttu-id="66c5d-177">例如10.0.0。0</span><span class="sxs-lookup"><span data-stu-id="66c5d-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="66c5d-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="66c5d-178">ipV4DHCPServer</span></span>|<span data-ttu-id="66c5d-179">String</span><span class="sxs-lookup"><span data-stu-id="66c5d-179">String</span></span>|<span data-ttu-id="66c5d-180">适配器的 DHCP 服务器的 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="66c5d-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="66c5d-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="66c5d-181">ipV4DNSServerList</span></span>|<span data-ttu-id="66c5d-182">String 集合</span><span class="sxs-lookup"><span data-stu-id="66c5d-182">String collection</span></span>|<span data-ttu-id="66c5d-183">为适配器配置的 IPv4 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="66c5d-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="66c5d-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="66c5d-184">dnsSuffixList</span></span>|<span data-ttu-id="66c5d-185">String 集合</span><span class="sxs-lookup"><span data-stu-id="66c5d-185">String collection</span></span>|<span data-ttu-id="66c5d-186">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="66c5d-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="66c5d-187">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="66c5d-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="66c5d-188">响应</span><span class="sxs-lookup"><span data-stu-id="66c5d-188">Response</span></span>
<span data-ttu-id="66c5d-189">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66c5d-189">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66c5d-190">示例</span><span class="sxs-lookup"><span data-stu-id="66c5d-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="66c5d-191">请求</span><span class="sxs-lookup"><span data-stu-id="66c5d-191">Request</span></span>
<span data-ttu-id="66c5d-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66c5d-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66c5d-193">响应</span><span class="sxs-lookup"><span data-stu-id="66c5d-193">Response</span></span>
<span data-ttu-id="66c5d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66c5d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




