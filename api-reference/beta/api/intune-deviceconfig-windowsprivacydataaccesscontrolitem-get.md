---
title: 获取 windowsPrivacyDataAccessControlItem
description: 读取 windowsPrivacyDataAccessControlItem 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2d4060b372836a171afd5854b61628ecf9cce8e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43428736"
---
# <a name="get-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="47111-103">获取 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="47111-103">Get windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="47111-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47111-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47111-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47111-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47111-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47111-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47111-107">读取[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47111-107">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47111-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="47111-108">Prerequisites</span></span>
<span data-ttu-id="47111-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47111-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="47111-111">Permission type</span></span>|<span data-ttu-id="47111-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="47111-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47111-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47111-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47111-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47111-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47111-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47111-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47111-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="47111-116">Not supported.</span></span>|
|<span data-ttu-id="47111-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="47111-117">Application</span></span>|<span data-ttu-id="47111-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47111-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47111-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47111-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47111-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="47111-120">Optional query parameters</span></span>
<span data-ttu-id="47111-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="47111-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47111-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="47111-122">Request headers</span></span>
|<span data-ttu-id="47111-123">标头</span><span class="sxs-lookup"><span data-stu-id="47111-123">Header</span></span>|<span data-ttu-id="47111-124">值</span><span class="sxs-lookup"><span data-stu-id="47111-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47111-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="47111-125">Authorization</span></span>|<span data-ttu-id="47111-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47111-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47111-127">接受</span><span class="sxs-lookup"><span data-stu-id="47111-127">Accept</span></span>|<span data-ttu-id="47111-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47111-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47111-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="47111-129">Request body</span></span>
<span data-ttu-id="47111-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47111-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47111-131">响应</span><span class="sxs-lookup"><span data-stu-id="47111-131">Response</span></span>
<span data-ttu-id="47111-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47111-132">If successful, this method returns a `200 OK` response code and [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47111-133">示例</span><span class="sxs-lookup"><span data-stu-id="47111-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="47111-134">请求</span><span class="sxs-lookup"><span data-stu-id="47111-134">Request</span></span>
<span data-ttu-id="47111-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47111-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

### <a name="response"></a><span data-ttu-id="47111-136">响应</span><span class="sxs-lookup"><span data-stu-id="47111-136">Response</span></span>
<span data-ttu-id="47111-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47111-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
    "id": "03b15556-5556-03b1-5655-b1035655b103",
    "accessLevel": "forceAllow",
    "dataCategory": "accountInfo",
    "appPackageFamilyName": "App Package Family Name value",
    "appDisplayName": "App Display Name value"
  }
}
```



