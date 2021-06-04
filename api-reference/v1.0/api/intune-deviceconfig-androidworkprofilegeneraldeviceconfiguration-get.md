---
title: 获取 androidWorkProfileGeneralDeviceConfiguration
description: 读取 androidWorkProfileGeneralDeviceConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b6f0c1591640cd9b36f64f0ccf8846b02af1741
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753977"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="8be7f-103">获取 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8be7f-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="8be7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8be7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8be7f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8be7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8be7f-106">读取 [androidWorkProfileGeneralDeviceConfiguration 对象的属性和](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="8be7f-106">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8be7f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8be7f-107">Prerequisites</span></span>
<span data-ttu-id="8be7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8be7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8be7f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8be7f-110">Permission type</span></span>|<span data-ttu-id="8be7f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8be7f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8be7f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8be7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8be7f-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8be7f-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8be7f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8be7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8be7f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8be7f-115">Not supported.</span></span>|
|<span data-ttu-id="8be7f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8be7f-116">Application</span></span>|<span data-ttu-id="8be7f-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8be7f-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8be7f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8be7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8be7f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8be7f-119">Optional query parameters</span></span>
<span data-ttu-id="8be7f-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8be7f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8be7f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8be7f-121">Request headers</span></span>
|<span data-ttu-id="8be7f-122">标头</span><span class="sxs-lookup"><span data-stu-id="8be7f-122">Header</span></span>|<span data-ttu-id="8be7f-123">值</span><span class="sxs-lookup"><span data-stu-id="8be7f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8be7f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8be7f-124">Authorization</span></span>|<span data-ttu-id="8be7f-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8be7f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8be7f-126">接受</span><span class="sxs-lookup"><span data-stu-id="8be7f-126">Accept</span></span>|<span data-ttu-id="8be7f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8be7f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8be7f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8be7f-128">Request body</span></span>
<span data-ttu-id="8be7f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8be7f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8be7f-130">响应</span><span class="sxs-lookup"><span data-stu-id="8be7f-130">Response</span></span>
<span data-ttu-id="8be7f-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8be7f-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8be7f-132">示例</span><span class="sxs-lookup"><span data-stu-id="8be7f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8be7f-133">请求</span><span class="sxs-lookup"><span data-stu-id="8be7f-133">Request</span></span>
<span data-ttu-id="8be7f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8be7f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8be7f-135">响应</span><span class="sxs-lookup"><span data-stu-id="8be7f-135">Response</span></span>
<span data-ttu-id="8be7f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8be7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




