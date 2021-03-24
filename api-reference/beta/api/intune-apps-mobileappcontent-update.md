---
title: 更新 mobileAppContent
description: 更新 mobileAppContent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff40470d0313cc3b3d1f040b605069b1491d5a99
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139823"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="87653-103">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="87653-103">Update mobileAppContent</span></span>

<span data-ttu-id="87653-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87653-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87653-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87653-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87653-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87653-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87653-107">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87653-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87653-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="87653-108">Prerequisites</span></span>
<span data-ttu-id="87653-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87653-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87653-111">Permission type</span></span>|<span data-ttu-id="87653-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87653-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87653-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87653-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87653-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87653-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87653-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87653-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87653-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87653-116">Not supported.</span></span>|
|<span data-ttu-id="87653-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87653-117">Application</span></span>|<span data-ttu-id="87653-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87653-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87653-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87653-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="87653-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="87653-120">Request headers</span></span>
|<span data-ttu-id="87653-121">标头</span><span class="sxs-lookup"><span data-stu-id="87653-121">Header</span></span>|<span data-ttu-id="87653-122">值</span><span class="sxs-lookup"><span data-stu-id="87653-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87653-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87653-123">Authorization</span></span>|<span data-ttu-id="87653-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87653-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87653-125">接受</span><span class="sxs-lookup"><span data-stu-id="87653-125">Accept</span></span>|<span data-ttu-id="87653-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87653-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87653-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87653-127">Request body</span></span>
<span data-ttu-id="87653-128">在请求正文中，提供 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87653-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="87653-129">下表显示创建 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="87653-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="87653-130">属性</span><span class="sxs-lookup"><span data-stu-id="87653-130">Property</span></span>|<span data-ttu-id="87653-131">类型</span><span class="sxs-lookup"><span data-stu-id="87653-131">Type</span></span>|<span data-ttu-id="87653-132">说明</span><span class="sxs-lookup"><span data-stu-id="87653-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87653-133">id</span><span class="sxs-lookup"><span data-stu-id="87653-133">id</span></span>|<span data-ttu-id="87653-134">String</span><span class="sxs-lookup"><span data-stu-id="87653-134">String</span></span>|<span data-ttu-id="87653-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="87653-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="87653-136">响应</span><span class="sxs-lookup"><span data-stu-id="87653-136">Response</span></span>
<span data-ttu-id="87653-137">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87653-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87653-138">示例</span><span class="sxs-lookup"><span data-stu-id="87653-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="87653-139">请求</span><span class="sxs-lookup"><span data-stu-id="87653-139">Request</span></span>
<span data-ttu-id="87653-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87653-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="87653-141">响应</span><span class="sxs-lookup"><span data-stu-id="87653-141">Response</span></span>
<span data-ttu-id="87653-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87653-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




