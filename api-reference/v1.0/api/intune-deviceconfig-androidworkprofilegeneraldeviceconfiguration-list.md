---
title: 列表 androidWorkProfileGeneralDeviceConfigurations
description: 列出属性和 androidWorkProfileGeneralDeviceConfiguration 对象之间的关系。
ms.openlocfilehash: a38db4f5fa714968f9a66ffd244db254d774f0db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011199"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="6c6de-103">列表 androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="6c6de-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="6c6de-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c6de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c6de-105">列出属性和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="6c6de-105">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c6de-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c6de-106">Prerequisites</span></span>
<span data-ttu-id="6c6de-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6c6de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c6de-109">Permission type</span></span>|<span data-ttu-id="6c6de-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c6de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c6de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c6de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c6de-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c6de-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c6de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c6de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c6de-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c6de-114">Not supported.</span></span>|
|<span data-ttu-id="6c6de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c6de-115">Application</span></span>|<span data-ttu-id="6c6de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c6de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c6de-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c6de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c6de-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c6de-118">Request headers</span></span>
|<span data-ttu-id="6c6de-119">标头</span><span class="sxs-lookup"><span data-stu-id="6c6de-119">Header</span></span>|<span data-ttu-id="6c6de-120">值</span><span class="sxs-lookup"><span data-stu-id="6c6de-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c6de-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6de-121">Authorization</span></span>|<span data-ttu-id="6c6de-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c6de-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c6de-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6c6de-123">Accept</span></span>|<span data-ttu-id="6c6de-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c6de-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6de-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c6de-125">Request body</span></span>
<span data-ttu-id="6c6de-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c6de-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c6de-127">响应</span><span class="sxs-lookup"><span data-stu-id="6c6de-127">Response</span></span>
<span data-ttu-id="6c6de-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="6c6de-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c6de-129">示例</span><span class="sxs-lookup"><span data-stu-id="6c6de-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c6de-130">请求</span><span class="sxs-lookup"><span data-stu-id="6c6de-130">Request</span></span>
<span data-ttu-id="6c6de-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c6de-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6c6de-132">响应</span><span class="sxs-lookup"><span data-stu-id="6c6de-132">Response</span></span>
<span data-ttu-id="6c6de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c6de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

{
  "value": [
    {
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
  ]
}
```



