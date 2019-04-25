---
title: 列出 groupPolicyPresentationDropdownLists
description: 列出 groupPolicyPresentationDropdownList 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7708e0dd8a3dd2e01c5cc09e50c4fee9d47d78fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32531087"
---
# <a name="list-grouppolicypresentationdropdownlists"></a><span data-ttu-id="65bbe-103">列出 groupPolicyPresentationDropdownLists</span><span class="sxs-lookup"><span data-stu-id="65bbe-103">List groupPolicyPresentationDropdownLists</span></span>

> <span data-ttu-id="65bbe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65bbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65bbe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65bbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65bbe-106">列出[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65bbe-106">List properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65bbe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="65bbe-107">Prerequisites</span></span>
<span data-ttu-id="65bbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65bbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65bbe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="65bbe-110">Permission type</span></span>|<span data-ttu-id="65bbe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65bbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65bbe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65bbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65bbe-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="65bbe-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="65bbe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65bbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65bbe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65bbe-115">Not supported.</span></span>|
|<span data-ttu-id="65bbe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65bbe-116">Application</span></span>|<span data-ttu-id="65bbe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="65bbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65bbe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65bbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="65bbe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65bbe-119">Request headers</span></span>
|<span data-ttu-id="65bbe-120">标头</span><span class="sxs-lookup"><span data-stu-id="65bbe-120">Header</span></span>|<span data-ttu-id="65bbe-121">值</span><span class="sxs-lookup"><span data-stu-id="65bbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65bbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65bbe-122">Authorization</span></span>|<span data-ttu-id="65bbe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65bbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65bbe-124">接受</span><span class="sxs-lookup"><span data-stu-id="65bbe-124">Accept</span></span>|<span data-ttu-id="65bbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65bbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65bbe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65bbe-126">Request body</span></span>
<span data-ttu-id="65bbe-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65bbe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65bbe-128">响应</span><span class="sxs-lookup"><span data-stu-id="65bbe-128">Response</span></span>
<span data-ttu-id="65bbe-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="65bbe-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65bbe-130">示例</span><span class="sxs-lookup"><span data-stu-id="65bbe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="65bbe-131">请求</span><span class="sxs-lookup"><span data-stu-id="65bbe-131">Request</span></span>
<span data-ttu-id="65bbe-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65bbe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="65bbe-133">响应</span><span class="sxs-lookup"><span data-stu-id="65bbe-133">Response</span></span>
<span data-ttu-id="65bbe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65bbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 703

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
      "label": "Label value",
      "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultItem": {
        "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
        "displayName": "Display Name value",
        "value": "Value value"
      },
      "items": [
        {
          "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
          "displayName": "Display Name value",
          "value": "Value value"
        }
      ],
      "required": true
    }
  ]
}
```





