---
title: 创建 termsAndConditionsAcceptanceStatus
description: 创建新的 termsAndConditionsAcceptanceStatus 对象。
author: tfitzmac
ms.openlocfilehash: 4a371d2ac03ef47ad0af4ae70aa248dcd96e4bf0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348298"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="fbff2-103">创建 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fbff2-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="fbff2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbff2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbff2-105">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbff2-105">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbff2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbff2-106">Prerequisites</span></span>
<span data-ttu-id="fbff2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fbff2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbff2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbff2-109">Permission type</span></span>|<span data-ttu-id="fbff2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbff2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbff2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbff2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbff2-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbff2-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbff2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbff2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbff2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbff2-114">Not supported.</span></span>|
|<span data-ttu-id="fbff2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbff2-115">Application</span></span>|<span data-ttu-id="fbff2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbff2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbff2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbff2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fbff2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbff2-118">Request headers</span></span>
|<span data-ttu-id="fbff2-119">标头</span><span class="sxs-lookup"><span data-stu-id="fbff2-119">Header</span></span>|<span data-ttu-id="fbff2-120">值</span><span class="sxs-lookup"><span data-stu-id="fbff2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbff2-121">授权</span><span class="sxs-lookup"><span data-stu-id="fbff2-121">Authorization</span></span>|<span data-ttu-id="fbff2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbff2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbff2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fbff2-123">Accept</span></span>|<span data-ttu-id="fbff2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fbff2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbff2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbff2-125">Request body</span></span>
<span data-ttu-id="fbff2-126">在请求正文中，提供 termsAndConditionsAcceptanceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbff2-126">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="fbff2-127">下表显示创建 termsAndConditionsAcceptanceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fbff2-127">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="fbff2-128">属性</span><span class="sxs-lookup"><span data-stu-id="fbff2-128">Property</span></span>|<span data-ttu-id="fbff2-129">类型</span><span class="sxs-lookup"><span data-stu-id="fbff2-129">Type</span></span>|<span data-ttu-id="fbff2-130">说明</span><span class="sxs-lookup"><span data-stu-id="fbff2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbff2-131">id</span><span class="sxs-lookup"><span data-stu-id="fbff2-131">id</span></span>|<span data-ttu-id="fbff2-132">String</span><span class="sxs-lookup"><span data-stu-id="fbff2-132">String</span></span>|<span data-ttu-id="fbff2-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fbff2-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fbff2-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fbff2-134">userDisplayName</span></span>|<span data-ttu-id="fbff2-135">String</span><span class="sxs-lookup"><span data-stu-id="fbff2-135">String</span></span>|<span data-ttu-id="fbff2-136">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fbff2-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="fbff2-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="fbff2-137">acceptedVersion</span></span>|<span data-ttu-id="fbff2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fbff2-138">Int32</span></span>|<span data-ttu-id="fbff2-139">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="fbff2-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="fbff2-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbff2-140">acceptedDateTime</span></span>|<span data-ttu-id="fbff2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbff2-141">DateTimeOffset</span></span>|<span data-ttu-id="fbff2-142">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fbff2-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="fbff2-143">响应</span><span class="sxs-lookup"><span data-stu-id="fbff2-143">Response</span></span>
<span data-ttu-id="fbff2-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbff2-144">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbff2-145">示例</span><span class="sxs-lookup"><span data-stu-id="fbff2-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbff2-146">请求</span><span class="sxs-lookup"><span data-stu-id="fbff2-146">Request</span></span>
<span data-ttu-id="fbff2-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbff2-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fbff2-148">响应</span><span class="sxs-lookup"><span data-stu-id="fbff2-148">Response</span></span>
<span data-ttu-id="fbff2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fbff2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



