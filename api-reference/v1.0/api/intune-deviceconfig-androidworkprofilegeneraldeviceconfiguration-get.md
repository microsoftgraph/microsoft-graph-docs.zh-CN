---
title: 获取 androidWorkProfileGeneralDeviceConfiguration
description: 读取属性和 androidWorkProfileGeneralDeviceConfiguration 对象的关系。
author: tfitzmac
ms.openlocfilehash: 61a8516a2f6dc5263c3976c0827f4acfd758831d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27300831"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="59100-103">获取 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="59100-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="59100-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="59100-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59100-105">读取属性和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="59100-105">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59100-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="59100-106">Prerequisites</span></span>
<span data-ttu-id="59100-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="59100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59100-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="59100-109">Permission type</span></span>|<span data-ttu-id="59100-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59100-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59100-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59100-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59100-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="59100-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="59100-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59100-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59100-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="59100-114">Not supported.</span></span>|
|<span data-ttu-id="59100-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="59100-115">Application</span></span>|<span data-ttu-id="59100-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59100-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59100-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59100-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59100-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59100-118">Optional query parameters</span></span>
<span data-ttu-id="59100-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59100-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59100-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="59100-120">Request headers</span></span>
|<span data-ttu-id="59100-121">标头</span><span class="sxs-lookup"><span data-stu-id="59100-121">Header</span></span>|<span data-ttu-id="59100-122">值</span><span class="sxs-lookup"><span data-stu-id="59100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59100-123">授权</span><span class="sxs-lookup"><span data-stu-id="59100-123">Authorization</span></span>|<span data-ttu-id="59100-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="59100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59100-125">Accept</span><span class="sxs-lookup"><span data-stu-id="59100-125">Accept</span></span>|<span data-ttu-id="59100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59100-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59100-127">Request body</span></span>
<span data-ttu-id="59100-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59100-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59100-129">响应</span><span class="sxs-lookup"><span data-stu-id="59100-129">Response</span></span>
<span data-ttu-id="59100-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59100-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59100-131">示例</span><span class="sxs-lookup"><span data-stu-id="59100-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="59100-132">请求</span><span class="sxs-lookup"><span data-stu-id="59100-132">Request</span></span>
<span data-ttu-id="59100-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59100-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="59100-134">响应</span><span class="sxs-lookup"><span data-stu-id="59100-134">Response</span></span>
<span data-ttu-id="59100-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59100-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true
  }
}
```



