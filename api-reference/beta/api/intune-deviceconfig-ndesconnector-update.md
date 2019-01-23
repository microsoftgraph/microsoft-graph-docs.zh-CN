---
title: 更新 ndesConnector
description: 更新 ndesConnector 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8c78502bb0670eca08b896bf1a0b732f94b669cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418419"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="c624f-103">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="c624f-103">Update ndesConnector</span></span>

> <span data-ttu-id="c624f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c624f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c624f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c624f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c624f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c624f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c624f-107">更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c624f-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c624f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c624f-108">Prerequisites</span></span>
<span data-ttu-id="c624f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c624f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c624f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c624f-111">Permission type</span></span>|<span data-ttu-id="c624f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c624f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c624f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c624f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c624f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c624f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c624f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c624f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c624f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c624f-116">Not supported.</span></span>|
|<span data-ttu-id="c624f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c624f-117">Application</span></span>|<span data-ttu-id="c624f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c624f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c624f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c624f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="c624f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c624f-120">Request headers</span></span>
|<span data-ttu-id="c624f-121">标头</span><span class="sxs-lookup"><span data-stu-id="c624f-121">Header</span></span>|<span data-ttu-id="c624f-122">值</span><span class="sxs-lookup"><span data-stu-id="c624f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c624f-123">授权</span><span class="sxs-lookup"><span data-stu-id="c624f-123">Authorization</span></span>|<span data-ttu-id="c624f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c624f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c624f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c624f-125">Accept</span></span>|<span data-ttu-id="c624f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c624f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c624f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c624f-127">Request body</span></span>
<span data-ttu-id="c624f-128">在请求正文中，提供[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c624f-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="c624f-129">下表显示时创建[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c624f-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="c624f-130">属性</span><span class="sxs-lookup"><span data-stu-id="c624f-130">Property</span></span>|<span data-ttu-id="c624f-131">类型</span><span class="sxs-lookup"><span data-stu-id="c624f-131">Type</span></span>|<span data-ttu-id="c624f-132">说明</span><span class="sxs-lookup"><span data-stu-id="c624f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c624f-133">id</span><span class="sxs-lookup"><span data-stu-id="c624f-133">id</span></span>|<span data-ttu-id="c624f-134">String</span><span class="sxs-lookup"><span data-stu-id="c624f-134">String</span></span>|<span data-ttu-id="c624f-135">NDES 连接符的键。</span><span class="sxs-lookup"><span data-stu-id="c624f-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="c624f-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c624f-136">lastConnectionDateTime</span></span>|<span data-ttu-id="c624f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c624f-137">DateTimeOffset</span></span>|<span data-ttu-id="c624f-138">Ndes 连接器的最后一个连接时间</span><span class="sxs-lookup"><span data-stu-id="c624f-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="c624f-139">state</span><span class="sxs-lookup"><span data-stu-id="c624f-139">state</span></span>|[<span data-ttu-id="c624f-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="c624f-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="c624f-141">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="c624f-141">Ndes Connector Status.</span></span> <span data-ttu-id="c624f-142">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="c624f-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="c624f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c624f-143">displayName</span></span>|<span data-ttu-id="c624f-144">String</span><span class="sxs-lookup"><span data-stu-id="c624f-144">String</span></span>|<span data-ttu-id="c624f-145">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="c624f-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="c624f-146">响应</span><span class="sxs-lookup"><span data-stu-id="c624f-146">Response</span></span>
<span data-ttu-id="c624f-147">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c624f-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c624f-148">示例</span><span class="sxs-lookup"><span data-stu-id="c624f-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c624f-149">请求</span><span class="sxs-lookup"><span data-stu-id="c624f-149">Request</span></span>
<span data-ttu-id="c624f-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c624f-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c624f-151">响应</span><span class="sxs-lookup"><span data-stu-id="c624f-151">Response</span></span>
<span data-ttu-id="c624f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c624f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




