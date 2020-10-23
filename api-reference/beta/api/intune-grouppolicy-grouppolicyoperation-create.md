---
title: 创建 groupPolicyOperation
description: 创建新的 groupPolicyOperation 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a3ba919a8e3a6c8b8338fcbd3389b3c3b764e52
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729094"
---
# <a name="create-grouppolicyoperation"></a><span data-ttu-id="19f6c-103">创建 groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="19f6c-103">Create groupPolicyOperation</span></span>

<span data-ttu-id="19f6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19f6c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19f6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19f6c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19f6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19f6c-107">创建新的 [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19f6c-107">Create a new [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19f6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="19f6c-108">Prerequisites</span></span>
<span data-ttu-id="19f6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="19f6c-111">Permission type</span></span>|<span data-ttu-id="19f6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="19f6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19f6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19f6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19f6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19f6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19f6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19f6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19f6c-116">Not supported.</span></span>|
|<span data-ttu-id="19f6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="19f6c-117">Application</span></span>|<span data-ttu-id="19f6c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f6c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19f6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19f6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

## <a name="request-headers"></a><span data-ttu-id="19f6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="19f6c-120">Request headers</span></span>
|<span data-ttu-id="19f6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="19f6c-121">Header</span></span>|<span data-ttu-id="19f6c-122">值</span><span class="sxs-lookup"><span data-stu-id="19f6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19f6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19f6c-123">Authorization</span></span>|<span data-ttu-id="19f6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="19f6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19f6c-125">接受</span><span class="sxs-lookup"><span data-stu-id="19f6c-125">Accept</span></span>|<span data-ttu-id="19f6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19f6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19f6c-127">Request body</span></span>
<span data-ttu-id="19f6c-128">在请求正文中，提供 groupPolicyOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19f6c-128">In the request body, supply a JSON representation for the groupPolicyOperation object.</span></span>

<span data-ttu-id="19f6c-129">下表显示创建 groupPolicyOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="19f6c-129">The following table shows the properties that are required when you create the groupPolicyOperation.</span></span>

|<span data-ttu-id="19f6c-130">属性</span><span class="sxs-lookup"><span data-stu-id="19f6c-130">Property</span></span>|<span data-ttu-id="19f6c-131">类型</span><span class="sxs-lookup"><span data-stu-id="19f6c-131">Type</span></span>|<span data-ttu-id="19f6c-132">说明</span><span class="sxs-lookup"><span data-stu-id="19f6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19f6c-133">operationType</span><span class="sxs-lookup"><span data-stu-id="19f6c-133">operationType</span></span>|[<span data-ttu-id="19f6c-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="19f6c-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="19f6c-135">组策略操作的类型。</span><span class="sxs-lookup"><span data-stu-id="19f6c-135">The type of group policy operation.</span></span> <span data-ttu-id="19f6c-136">可取值为：`none`、`upload`、`uploadNewVersion`、`addLanguageFiles`、`removeLanguageFiles`、`updateLanguageFiles` 或 `remove`。</span><span class="sxs-lookup"><span data-stu-id="19f6c-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="19f6c-137">operationStatus</span><span class="sxs-lookup"><span data-stu-id="19f6c-137">operationStatus</span></span>|[<span data-ttu-id="19f6c-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="19f6c-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="19f6c-139">组策略操作状态。</span><span class="sxs-lookup"><span data-stu-id="19f6c-139">The group policy operation status.</span></span> <span data-ttu-id="19f6c-140">可取值为：`unknown`、`inProgress`、`success`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="19f6c-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="19f6c-141">statusDetails</span><span class="sxs-lookup"><span data-stu-id="19f6c-141">statusDetails</span></span>|<span data-ttu-id="19f6c-142">String</span><span class="sxs-lookup"><span data-stu-id="19f6c-142">String</span></span>|<span data-ttu-id="19f6c-143">组策略操作状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="19f6c-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="19f6c-144">id</span><span class="sxs-lookup"><span data-stu-id="19f6c-144">id</span></span>|<span data-ttu-id="19f6c-145">String</span><span class="sxs-lookup"><span data-stu-id="19f6c-145">String</span></span>|<span data-ttu-id="19f6c-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="19f6c-146">Key of the entity.</span></span>|
|<span data-ttu-id="19f6c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19f6c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="19f6c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19f6c-148">DateTimeOffset</span></span>|<span data-ttu-id="19f6c-149">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="19f6c-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="19f6c-150">响应</span><span class="sxs-lookup"><span data-stu-id="19f6c-150">Response</span></span>
<span data-ttu-id="19f6c-151">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19f6c-151">If successful, this method returns a `201 Created` response code and a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f6c-152">示例</span><span class="sxs-lookup"><span data-stu-id="19f6c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="19f6c-153">请求</span><span class="sxs-lookup"><span data-stu-id="19f6c-153">Request</span></span>
<span data-ttu-id="19f6c-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19f6c-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a><span data-ttu-id="19f6c-155">响应</span><span class="sxs-lookup"><span data-stu-id="19f6c-155">Response</span></span>
<span data-ttu-id="19f6c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19f6c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value",
  "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





