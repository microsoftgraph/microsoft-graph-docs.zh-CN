---
title: 更新 deviceManagementDomainJoinConnector
description: 更新 deviceManagementDomainJoinConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3507f878ce94950c702ad61ca377aa7aaafb1c2d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152738"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="9d753-103">更新 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="9d753-103">Update deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="9d753-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d753-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d753-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d753-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d753-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d753-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d753-107">更新 [deviceManagementDomainJoinConnector 对象](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9d753-107">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d753-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d753-108">Prerequisites</span></span>
<span data-ttu-id="9d753-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d753-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d753-111">Permission type</span></span>|<span data-ttu-id="9d753-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d753-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d753-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d753-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d753-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d753-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d753-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d753-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d753-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d753-116">Not supported.</span></span>|
|<span data-ttu-id="9d753-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d753-117">Application</span></span>|<span data-ttu-id="9d753-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d753-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d753-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d753-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="9d753-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d753-120">Request headers</span></span>
|<span data-ttu-id="9d753-121">标头</span><span class="sxs-lookup"><span data-stu-id="9d753-121">Header</span></span>|<span data-ttu-id="9d753-122">值</span><span class="sxs-lookup"><span data-stu-id="9d753-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d753-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d753-123">Authorization</span></span>|<span data-ttu-id="9d753-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d753-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d753-125">接受</span><span class="sxs-lookup"><span data-stu-id="9d753-125">Accept</span></span>|<span data-ttu-id="9d753-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d753-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d753-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d753-127">Request body</span></span>
<span data-ttu-id="9d753-128">在请求正文中，提供 [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d753-128">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="9d753-129">下表显示创建 [deviceManagementDomainJoinConnector 时所需的属性](../resources/intune-odj-devicemanagementdomainjoinconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="9d753-129">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="9d753-130">属性</span><span class="sxs-lookup"><span data-stu-id="9d753-130">Property</span></span>|<span data-ttu-id="9d753-131">类型</span><span class="sxs-lookup"><span data-stu-id="9d753-131">Type</span></span>|<span data-ttu-id="9d753-132">说明</span><span class="sxs-lookup"><span data-stu-id="9d753-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d753-133">id</span><span class="sxs-lookup"><span data-stu-id="9d753-133">id</span></span>|<span data-ttu-id="9d753-134">String</span><span class="sxs-lookup"><span data-stu-id="9d753-134">String</span></span>|<span data-ttu-id="9d753-135">表示连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9d753-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="9d753-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9d753-136">displayName</span></span>|<span data-ttu-id="9d753-137">String</span><span class="sxs-lookup"><span data-stu-id="9d753-137">String</span></span>|<span data-ttu-id="9d753-138">连接器显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d753-138">The connector display name.</span></span>|
|<span data-ttu-id="9d753-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="9d753-139">lastConnectionDateTime</span></span>|<span data-ttu-id="9d753-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d753-140">DateTimeOffset</span></span>|<span data-ttu-id="9d753-141">上次连接器联系 Intune 的时间。</span><span class="sxs-lookup"><span data-stu-id="9d753-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="9d753-142">state</span><span class="sxs-lookup"><span data-stu-id="9d753-142">state</span></span>|[<span data-ttu-id="9d753-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="9d753-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="9d753-144">连接器状态。</span><span class="sxs-lookup"><span data-stu-id="9d753-144">The connector state.</span></span> <span data-ttu-id="9d753-145">可取值为：`active`、`error`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="9d753-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="9d753-146">version</span><span class="sxs-lookup"><span data-stu-id="9d753-146">version</span></span>|<span data-ttu-id="9d753-147">String</span><span class="sxs-lookup"><span data-stu-id="9d753-147">String</span></span>|<span data-ttu-id="9d753-148">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="9d753-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="9d753-149">响应</span><span class="sxs-lookup"><span data-stu-id="9d753-149">Response</span></span>
<span data-ttu-id="9d753-150">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d753-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d753-151">示例</span><span class="sxs-lookup"><span data-stu-id="9d753-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d753-152">请求</span><span class="sxs-lookup"><span data-stu-id="9d753-152">Request</span></span>
<span data-ttu-id="9d753-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d753-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="9d753-154">响应</span><span class="sxs-lookup"><span data-stu-id="9d753-154">Response</span></span>
<span data-ttu-id="9d753-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d753-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```




