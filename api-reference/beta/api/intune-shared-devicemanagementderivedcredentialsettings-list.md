---
title: 列出 deviceManagementDerivedCredentialSettingses
description: 列出 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 806cb2a4eb3844f9d9f279b45d00cf23114bbbc6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867859"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="c71e4-103">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="c71e4-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="c71e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c71e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c71e4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c71e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c71e4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c71e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c71e4-107">列出 [deviceManagementDerivedCredentialSettings 对象的属性和](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c71e4-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c71e4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c71e4-108">Prerequisites</span></span>
<span data-ttu-id="c71e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c71e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c71e4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c71e4-111">Permission type</span></span>|<span data-ttu-id="c71e4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c71e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c71e4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c71e4-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c71e4-114">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="c71e4-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="c71e4-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c71e4-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c71e4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c71e4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c71e4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c71e4-117">Not supported.</span></span>|
|<span data-ttu-id="c71e4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c71e4-118">Application</span></span>||
|<span data-ttu-id="c71e4-119">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="c71e4-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="c71e4-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c71e4-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c71e4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c71e4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="c71e4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c71e4-122">Request headers</span></span>
|<span data-ttu-id="c71e4-123">标头</span><span class="sxs-lookup"><span data-stu-id="c71e4-123">Header</span></span>|<span data-ttu-id="c71e4-124">值</span><span class="sxs-lookup"><span data-stu-id="c71e4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c71e4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c71e4-125">Authorization</span></span>|<span data-ttu-id="c71e4-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c71e4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c71e4-127">接受</span><span class="sxs-lookup"><span data-stu-id="c71e4-127">Accept</span></span>|<span data-ttu-id="c71e4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c71e4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c71e4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c71e4-129">Request body</span></span>
<span data-ttu-id="c71e4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c71e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c71e4-131">响应</span><span class="sxs-lookup"><span data-stu-id="c71e4-131">Response</span></span>
<span data-ttu-id="c71e4-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c71e4-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c71e4-133">示例</span><span class="sxs-lookup"><span data-stu-id="c71e4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c71e4-134">请求</span><span class="sxs-lookup"><span data-stu-id="c71e4-134">Request</span></span>
<span data-ttu-id="c71e4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c71e4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="c71e4-136">响应</span><span class="sxs-lookup"><span data-stu-id="c71e4-136">Response</span></span>
<span data-ttu-id="c71e4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c71e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
      "id": "bc650741-0741-bc65-4107-65bc410765bc",
      "helpUrl": "https://example.com/helpUrl/",
      "displayName": "Display Name value",
      "issuer": "entrustDatacard",
      "notificationType": "companyPortal"
    }
  ]
}
```








