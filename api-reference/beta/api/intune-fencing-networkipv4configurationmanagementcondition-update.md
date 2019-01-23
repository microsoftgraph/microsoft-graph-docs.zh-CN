---
title: 更新 networkIPv4ConfigurationManagementCondition
description: 更新 networkIPv4ConfigurationManagementCondition 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ba949cacb4bdfe26de809f3baeaaece68918eab9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402081"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="cc1eb-103">更新 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cc1eb-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="cc1eb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc1eb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc1eb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc1eb-107">更新[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc1eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc1eb-108">Prerequisites</span></span>
<span data-ttu-id="cc1eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc1eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc1eb-111">Permission type</span></span>|<span data-ttu-id="cc1eb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc1eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc1eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc1eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc1eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc1eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc1eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc1eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc1eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-116">Not supported.</span></span>|
|<span data-ttu-id="cc1eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc1eb-117">Application</span></span>|<span data-ttu-id="cc1eb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc1eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc1eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="cc1eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc1eb-120">Request headers</span></span>
|<span data-ttu-id="cc1eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="cc1eb-121">Header</span></span>|<span data-ttu-id="cc1eb-122">值</span><span class="sxs-lookup"><span data-stu-id="cc1eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc1eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc1eb-123">Authorization</span></span>|<span data-ttu-id="cc1eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc1eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc1eb-125">Accept</span></span>|<span data-ttu-id="cc1eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc1eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc1eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc1eb-127">Request body</span></span>
<span data-ttu-id="cc1eb-128">在请求正文中，提供[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="cc1eb-129">下表显示时创建[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="cc1eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="cc1eb-130">Property</span></span>|<span data-ttu-id="cc1eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="cc1eb-131">Type</span></span>|<span data-ttu-id="cc1eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="cc1eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc1eb-133">id</span><span class="sxs-lookup"><span data-stu-id="cc1eb-133">id</span></span>|<span data-ttu-id="cc1eb-134">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-134">String</span></span>|<span data-ttu-id="cc1eb-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="cc1eb-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-136">System generated value assigned when created.</span></span> <span data-ttu-id="cc1eb-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-138">唯一名称</span><span class="sxs-lookup"><span data-stu-id="cc1eb-138">uniqueName</span></span>|<span data-ttu-id="cc1eb-139">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-139">String</span></span>|<span data-ttu-id="cc1eb-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-140">Unique name for the management condition.</span></span> <span data-ttu-id="cc1eb-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-141">Used in management condition expressions.</span></span> <span data-ttu-id="cc1eb-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cc1eb-143">displayName</span></span>|<span data-ttu-id="cc1eb-144">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-144">String</span></span>|<span data-ttu-id="cc1eb-145">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="cc1eb-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-147">说明</span><span class="sxs-lookup"><span data-stu-id="cc1eb-147">description</span></span>|<span data-ttu-id="cc1eb-148">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-148">String</span></span>|<span data-ttu-id="cc1eb-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="cc1eb-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc1eb-151">createdDateTime</span></span>|<span data-ttu-id="cc1eb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc1eb-152">DateTimeOffset</span></span>|<span data-ttu-id="cc1eb-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-153">The time the management condition was created.</span></span> <span data-ttu-id="cc1eb-154">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-154">Generated service side.</span></span> <span data-ttu-id="cc1eb-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc1eb-156">modifiedDateTime</span></span>|<span data-ttu-id="cc1eb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc1eb-157">DateTimeOffset</span></span>|<span data-ttu-id="cc1eb-158">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-158">The time the management condition was last modified.</span></span> <span data-ttu-id="cc1eb-159">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-159">Updated service side.</span></span> <span data-ttu-id="cc1eb-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-161">eTag</span><span class="sxs-lookup"><span data-stu-id="cc1eb-161">eTag</span></span>|<span data-ttu-id="cc1eb-162">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-162">String</span></span>|<span data-ttu-id="cc1eb-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-163">ETag of the management condition.</span></span> <span data-ttu-id="cc1eb-164">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-164">Updated service side.</span></span> <span data-ttu-id="cc1eb-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc1eb-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc1eb-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cc1eb-166">applicablePlatforms</span></span>|<span data-ttu-id="cc1eb-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc1eb-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cc1eb-168">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="cc1eb-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="cc1eb-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="cc1eb-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="cc1eb-171">ipV4Prefix</span></span>|<span data-ttu-id="cc1eb-172">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-172">String</span></span>|<span data-ttu-id="cc1eb-173">要连接到的 IPv4 子网。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="cc1eb-174">例如 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="cc1eb-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="cc1eb-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="cc1eb-175">ipV4Gateway</span></span>|<span data-ttu-id="cc1eb-176">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-176">String</span></span>|<span data-ttu-id="cc1eb-177">IPv4 网关地址。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-177">The IPv4 gateway address.</span></span> <span data-ttu-id="cc1eb-178">例如 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="cc1eb-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="cc1eb-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="cc1eb-179">ipV4DHCPServer</span></span>|<span data-ttu-id="cc1eb-180">String</span><span class="sxs-lookup"><span data-stu-id="cc1eb-180">String</span></span>|<span data-ttu-id="cc1eb-181">为此适配器 DHCP 服务器的 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="cc1eb-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="cc1eb-182">ipV4DNSServerList</span></span>|<span data-ttu-id="cc1eb-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="cc1eb-183">String collection</span></span>|<span data-ttu-id="cc1eb-184">配置为此适配器 IPv4 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="cc1eb-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="cc1eb-185">dnsSuffixList</span></span>|<span data-ttu-id="cc1eb-186">String 集合</span><span class="sxs-lookup"><span data-stu-id="cc1eb-186">String collection</span></span>|<span data-ttu-id="cc1eb-187">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="cc1eb-188">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="cc1eb-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="cc1eb-189">响应</span><span class="sxs-lookup"><span data-stu-id="cc1eb-189">Response</span></span>
<span data-ttu-id="cc1eb-190">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc1eb-191">示例</span><span class="sxs-lookup"><span data-stu-id="cc1eb-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc1eb-192">请求</span><span class="sxs-lookup"><span data-stu-id="cc1eb-192">Request</span></span>
<span data-ttu-id="cc1eb-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc1eb-194">响应</span><span class="sxs-lookup"><span data-stu-id="cc1eb-194">Response</span></span>
<span data-ttu-id="cc1eb-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc1eb-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




