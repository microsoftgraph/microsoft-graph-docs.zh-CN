---
title: 创建 windowsPhone81CustomConfiguration
description: 创建新的 windowsPhone81CustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe02cc2ab54753c9825bb007f480529c17cf8210
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991991"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="7b25b-103">创建 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b25b-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="7b25b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b25b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b25b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b25b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b25b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7b25b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b25b-107">创建新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b25b-107">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b25b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b25b-108">Prerequisites</span></span>
<span data-ttu-id="7b25b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7b25b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b25b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b25b-111">Permission type</span></span>|<span data-ttu-id="7b25b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b25b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b25b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b25b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b25b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b25b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b25b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b25b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b25b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b25b-116">Not supported.</span></span>|
|<span data-ttu-id="7b25b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b25b-117">Application</span></span>|<span data-ttu-id="7b25b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b25b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b25b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b25b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b25b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b25b-120">Request headers</span></span>
|<span data-ttu-id="7b25b-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b25b-121">Header</span></span>|<span data-ttu-id="7b25b-122">值</span><span class="sxs-lookup"><span data-stu-id="7b25b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b25b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b25b-123">Authorization</span></span>|<span data-ttu-id="7b25b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b25b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b25b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b25b-125">Accept</span></span>|<span data-ttu-id="7b25b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b25b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b25b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b25b-127">Request body</span></span>
<span data-ttu-id="7b25b-128">在请求正文中，提供 windowsPhone81CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b25b-128">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="7b25b-129">下表显示了创建 windowsPhone81CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b25b-129">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="7b25b-130">属性</span><span class="sxs-lookup"><span data-stu-id="7b25b-130">Property</span></span>|<span data-ttu-id="7b25b-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b25b-131">Type</span></span>|<span data-ttu-id="7b25b-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b25b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b25b-133">id</span><span class="sxs-lookup"><span data-stu-id="7b25b-133">id</span></span>|<span data-ttu-id="7b25b-134">String</span><span class="sxs-lookup"><span data-stu-id="7b25b-134">String</span></span>|<span data-ttu-id="7b25b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b25b-135">Key of the entity.</span></span> <span data-ttu-id="7b25b-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b25b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7b25b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b25b-138">DateTimeOffset</span></span>|<span data-ttu-id="7b25b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7b25b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7b25b-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b25b-141">roleScopeTagIds</span></span>|<span data-ttu-id="7b25b-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="7b25b-142">String collection</span></span>|<span data-ttu-id="7b25b-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="7b25b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b25b-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7b25b-145">supportsScopeTags</span></span>|<span data-ttu-id="7b25b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b25b-146">Boolean</span></span>|<span data-ttu-id="7b25b-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="7b25b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b25b-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="7b25b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b25b-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="7b25b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b25b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b25b-150">This property is read-only.</span></span> <span data-ttu-id="7b25b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b25b-152">createdDateTime</span></span>|<span data-ttu-id="7b25b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b25b-153">DateTimeOffset</span></span>|<span data-ttu-id="7b25b-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7b25b-154">DateTime the object was created.</span></span> <span data-ttu-id="7b25b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-156">description</span><span class="sxs-lookup"><span data-stu-id="7b25b-156">description</span></span>|<span data-ttu-id="7b25b-157">String</span><span class="sxs-lookup"><span data-stu-id="7b25b-157">String</span></span>|<span data-ttu-id="7b25b-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7b25b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b25b-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7b25b-160">displayName</span></span>|<span data-ttu-id="7b25b-161">String</span><span class="sxs-lookup"><span data-stu-id="7b25b-161">String</span></span>|<span data-ttu-id="7b25b-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7b25b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b25b-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-164">version</span><span class="sxs-lookup"><span data-stu-id="7b25b-164">version</span></span>|<span data-ttu-id="7b25b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7b25b-165">Int32</span></span>|<span data-ttu-id="7b25b-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7b25b-166">Version of the device configuration.</span></span> <span data-ttu-id="7b25b-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b25b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b25b-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="7b25b-168">omaSettings</span></span>|<span data-ttu-id="7b25b-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b25b-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="7b25b-170">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="7b25b-170">OMA settings.</span></span> <span data-ttu-id="7b25b-171">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="7b25b-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7b25b-172">响应</span><span class="sxs-lookup"><span data-stu-id="7b25b-172">Response</span></span>
<span data-ttu-id="7b25b-173">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b25b-173">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b25b-174">示例</span><span class="sxs-lookup"><span data-stu-id="7b25b-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b25b-175">请求</span><span class="sxs-lookup"><span data-stu-id="7b25b-175">Request</span></span>
<span data-ttu-id="7b25b-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b25b-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7b25b-177">响应</span><span class="sxs-lookup"><span data-stu-id="7b25b-177">Response</span></span>
<span data-ttu-id="7b25b-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b25b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```





