---
title: 创建 mobileAppCategory
description: 创建新的 mobileAppCategory 对象。
author: tfitzmac
ms.openlocfilehash: 17084b8c02421b94b733a9ecb1011d647dab02d4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326332"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="bfaab-103">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="bfaab-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="bfaab-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bfaab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfaab-105">创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfaab-105">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfaab-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bfaab-106">Prerequisites</span></span>
<span data-ttu-id="bfaab-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bfaab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfaab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfaab-109">Permission type</span></span>|<span data-ttu-id="bfaab-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bfaab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfaab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfaab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfaab-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfaab-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfaab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfaab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfaab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfaab-114">Not supported.</span></span>|
|<span data-ttu-id="bfaab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfaab-115">Application</span></span>|<span data-ttu-id="bfaab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfaab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfaab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfaab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="bfaab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfaab-118">Request headers</span></span>
|<span data-ttu-id="bfaab-119">标头</span><span class="sxs-lookup"><span data-stu-id="bfaab-119">Header</span></span>|<span data-ttu-id="bfaab-120">值</span><span class="sxs-lookup"><span data-stu-id="bfaab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfaab-121">授权</span><span class="sxs-lookup"><span data-stu-id="bfaab-121">Authorization</span></span>|<span data-ttu-id="bfaab-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bfaab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfaab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bfaab-123">Accept</span></span>|<span data-ttu-id="bfaab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bfaab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfaab-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfaab-125">Request body</span></span>
<span data-ttu-id="bfaab-126">在请求正文中，提供 mobileAppCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfaab-126">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="bfaab-127">下表显示创建 mobileAppCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bfaab-127">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="bfaab-128">属性</span><span class="sxs-lookup"><span data-stu-id="bfaab-128">Property</span></span>|<span data-ttu-id="bfaab-129">类型</span><span class="sxs-lookup"><span data-stu-id="bfaab-129">Type</span></span>|<span data-ttu-id="bfaab-130">说明</span><span class="sxs-lookup"><span data-stu-id="bfaab-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfaab-131">id</span><span class="sxs-lookup"><span data-stu-id="bfaab-131">id</span></span>|<span data-ttu-id="bfaab-132">String</span><span class="sxs-lookup"><span data-stu-id="bfaab-132">String</span></span>|<span data-ttu-id="bfaab-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bfaab-133">The key of the entity.</span></span>|
|<span data-ttu-id="bfaab-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bfaab-134">displayName</span></span>|<span data-ttu-id="bfaab-135">String</span><span class="sxs-lookup"><span data-stu-id="bfaab-135">String</span></span>|<span data-ttu-id="bfaab-136">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="bfaab-136">The name of the app category.</span></span>|
|<span data-ttu-id="bfaab-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfaab-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bfaab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfaab-138">DateTimeOffset</span></span>|<span data-ttu-id="bfaab-139">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bfaab-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bfaab-140">响应</span><span class="sxs-lookup"><span data-stu-id="bfaab-140">Response</span></span>
<span data-ttu-id="bfaab-141">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfaab-141">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfaab-142">示例</span><span class="sxs-lookup"><span data-stu-id="bfaab-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfaab-143">请求</span><span class="sxs-lookup"><span data-stu-id="bfaab-143">Request</span></span>
<span data-ttu-id="bfaab-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfaab-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="bfaab-145">响应</span><span class="sxs-lookup"><span data-stu-id="bfaab-145">Response</span></span>
<span data-ttu-id="bfaab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfaab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



