---
title: 更新 networkIPv4ConfigurationManagementCondition
description: 更新 networkIPv4ConfigurationManagementCondition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 455f0631331f67c161b543cd85dc30c97d75ac1a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149432"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="76cc5-103">更新 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="76cc5-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="76cc5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76cc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76cc5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76cc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76cc5-106">更新[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76cc5-106">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76cc5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="76cc5-107">Prerequisites</span></span>
<span data-ttu-id="76cc5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="76cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="76cc5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="76cc5-110">Permission type</span></span>|<span data-ttu-id="76cc5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76cc5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76cc5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76cc5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76cc5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76cc5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76cc5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76cc5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76cc5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="76cc5-115">Not supported.</span></span>|
|<span data-ttu-id="76cc5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="76cc5-116">Application</span></span>|<span data-ttu-id="76cc5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="76cc5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76cc5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76cc5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="76cc5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="76cc5-119">Request headers</span></span>
|<span data-ttu-id="76cc5-120">标头</span><span class="sxs-lookup"><span data-stu-id="76cc5-120">Header</span></span>|<span data-ttu-id="76cc5-121">值</span><span class="sxs-lookup"><span data-stu-id="76cc5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76cc5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76cc5-122">Authorization</span></span>|<span data-ttu-id="76cc5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76cc5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76cc5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="76cc5-124">Accept</span></span>|<span data-ttu-id="76cc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76cc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76cc5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="76cc5-126">Request body</span></span>
<span data-ttu-id="76cc5-127">在请求正文中, 提供[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76cc5-127">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="76cc5-128">下表显示创建[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="76cc5-128">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="76cc5-129">属性</span><span class="sxs-lookup"><span data-stu-id="76cc5-129">Property</span></span>|<span data-ttu-id="76cc5-130">类型</span><span class="sxs-lookup"><span data-stu-id="76cc5-130">Type</span></span>|<span data-ttu-id="76cc5-131">说明</span><span class="sxs-lookup"><span data-stu-id="76cc5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76cc5-132">id</span><span class="sxs-lookup"><span data-stu-id="76cc5-132">id</span></span>|<span data-ttu-id="76cc5-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="76cc5-133">String</span></span>|<span data-ttu-id="76cc5-134">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="76cc5-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="76cc5-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="76cc5-135">System generated value assigned when created.</span></span> <span data-ttu-id="76cc5-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="76cc5-137">uniqueName</span></span>|<span data-ttu-id="76cc5-138">字符串</span><span class="sxs-lookup"><span data-stu-id="76cc5-138">String</span></span>|<span data-ttu-id="76cc5-139">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="76cc5-139">Unique name for the management condition.</span></span> <span data-ttu-id="76cc5-140">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="76cc5-140">Used in management condition expressions.</span></span> <span data-ttu-id="76cc5-141">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="76cc5-142">displayName</span></span>|<span data-ttu-id="76cc5-143">字符串</span><span class="sxs-lookup"><span data-stu-id="76cc5-143">String</span></span>|<span data-ttu-id="76cc5-144">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="76cc5-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="76cc5-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-146">说明</span><span class="sxs-lookup"><span data-stu-id="76cc5-146">description</span></span>|<span data-ttu-id="76cc5-147">字符串</span><span class="sxs-lookup"><span data-stu-id="76cc5-147">String</span></span>|<span data-ttu-id="76cc5-148">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="76cc5-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="76cc5-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76cc5-150">createdDateTime</span></span>|<span data-ttu-id="76cc5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76cc5-151">DateTimeOffset</span></span>|<span data-ttu-id="76cc5-152">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="76cc5-152">The time the management condition was created.</span></span> <span data-ttu-id="76cc5-153">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="76cc5-153">Generated service side.</span></span> <span data-ttu-id="76cc5-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76cc5-155">modifiedDateTime</span></span>|<span data-ttu-id="76cc5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76cc5-156">DateTimeOffset</span></span>|<span data-ttu-id="76cc5-157">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="76cc5-157">The time the management condition was last modified.</span></span> <span data-ttu-id="76cc5-158">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="76cc5-158">Updated service side.</span></span> <span data-ttu-id="76cc5-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-160">eTag</span><span class="sxs-lookup"><span data-stu-id="76cc5-160">eTag</span></span>|<span data-ttu-id="76cc5-161">String</span><span class="sxs-lookup"><span data-stu-id="76cc5-161">String</span></span>|<span data-ttu-id="76cc5-162">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="76cc5-162">ETag of the management condition.</span></span> <span data-ttu-id="76cc5-163">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="76cc5-163">Updated service side.</span></span> <span data-ttu-id="76cc5-164">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="76cc5-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="76cc5-165">applicablePlatforms</span></span>|<span data-ttu-id="76cc5-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="76cc5-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="76cc5-167">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="76cc5-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="76cc5-168">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="76cc5-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="76cc5-169">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="76cc5-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="76cc5-170">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="76cc5-170">ipV4Prefix</span></span>|<span data-ttu-id="76cc5-171">字符串</span><span class="sxs-lookup"><span data-stu-id="76cc5-171">String</span></span>|<span data-ttu-id="76cc5-172">要连接到的 IPv4 子网。</span><span class="sxs-lookup"><span data-stu-id="76cc5-172">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="76cc5-173">例如, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="76cc5-173">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="76cc5-174">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="76cc5-174">ipV4Gateway</span></span>|<span data-ttu-id="76cc5-175">字符串</span><span class="sxs-lookup"><span data-stu-id="76cc5-175">String</span></span>|<span data-ttu-id="76cc5-176">IPv4 网关地址。</span><span class="sxs-lookup"><span data-stu-id="76cc5-176">The IPv4 gateway address.</span></span> <span data-ttu-id="76cc5-177">例如10.0.0。0</span><span class="sxs-lookup"><span data-stu-id="76cc5-177">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="76cc5-178">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="76cc5-178">ipV4DHCPServer</span></span>|<span data-ttu-id="76cc5-179">字符串</span><span class="sxs-lookup"><span data-stu-id="76cc5-179">String</span></span>|<span data-ttu-id="76cc5-180">适配器的 DHCP 服务器的 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="76cc5-180">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="76cc5-181">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="76cc5-181">ipV4DNSServerList</span></span>|<span data-ttu-id="76cc5-182">String collection</span><span class="sxs-lookup"><span data-stu-id="76cc5-182">String collection</span></span>|<span data-ttu-id="76cc5-183">为适配器配置的 IPv4 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="76cc5-183">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="76cc5-184">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="76cc5-184">dnsSuffixList</span></span>|<span data-ttu-id="76cc5-185">String collection</span><span class="sxs-lookup"><span data-stu-id="76cc5-185">String collection</span></span>|<span data-ttu-id="76cc5-186">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="76cc5-186">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="76cc5-187">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="76cc5-187">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="76cc5-188">响应</span><span class="sxs-lookup"><span data-stu-id="76cc5-188">Response</span></span>
<span data-ttu-id="76cc5-189">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="76cc5-189">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76cc5-190">示例</span><span class="sxs-lookup"><span data-stu-id="76cc5-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="76cc5-191">请求</span><span class="sxs-lookup"><span data-stu-id="76cc5-191">Request</span></span>
<span data-ttu-id="76cc5-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76cc5-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="76cc5-193">响应</span><span class="sxs-lookup"><span data-stu-id="76cc5-193">Response</span></span>
<span data-ttu-id="76cc5-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76cc5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




