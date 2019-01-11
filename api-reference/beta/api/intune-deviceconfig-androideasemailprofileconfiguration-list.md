---
title: 列表 androidEasEmailProfileConfigurations
description: 列出属性和 androidEasEmailProfileConfiguration 对象之间的关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3306c052f05eb05f84d0c250495a8af0e71a79bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863621"
---
# <a name="list-androideasemailprofileconfigurations"></a><span data-ttu-id="e6b10-103">列表 androidEasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="e6b10-103">List androidEasEmailProfileConfigurations</span></span>

> <span data-ttu-id="e6b10-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e6b10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6b10-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e6b10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6b10-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6b10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6b10-107">列出属性和[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e6b10-107">List properties and relationships of the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6b10-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6b10-108">Prerequisites</span></span>
<span data-ttu-id="e6b10-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e6b10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6b10-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6b10-111">Permission type</span></span>|<span data-ttu-id="e6b10-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6b10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6b10-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6b10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6b10-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6b10-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e6b10-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6b10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6b10-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6b10-116">Not supported.</span></span>|
|<span data-ttu-id="e6b10-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6b10-117">Application</span></span>|<span data-ttu-id="e6b10-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6b10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6b10-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6b10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e6b10-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6b10-120">Request headers</span></span>
|<span data-ttu-id="e6b10-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6b10-121">Header</span></span>|<span data-ttu-id="e6b10-122">值</span><span class="sxs-lookup"><span data-stu-id="e6b10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6b10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6b10-123">Authorization</span></span>|<span data-ttu-id="e6b10-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6b10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6b10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6b10-125">Accept</span></span>|<span data-ttu-id="e6b10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6b10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6b10-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6b10-127">Request body</span></span>
<span data-ttu-id="e6b10-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6b10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6b10-129">响应</span><span class="sxs-lookup"><span data-stu-id="e6b10-129">Response</span></span>
<span data-ttu-id="e6b10-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e6b10-130">If successful, this method returns a `200 OK` response code and a collection of [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6b10-131">示例</span><span class="sxs-lookup"><span data-stu-id="e6b10-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6b10-132">请求</span><span class="sxs-lookup"><span data-stu-id="e6b10-132">Request</span></span>
<span data-ttu-id="e6b10-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6b10-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e6b10-134">响应</span><span class="sxs-lookup"><span data-stu-id="e6b10-134">Response</span></span>
<span data-ttu-id="e6b10-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6b10-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1102

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
      "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountName": "Account Name value",
      "authenticationMethod": "certificate",
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "syncNotes": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSmime": true,
      "requireSsl": true,
      "usernameSource": "userPrincipalName",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value"
    }
  ]
}
```





