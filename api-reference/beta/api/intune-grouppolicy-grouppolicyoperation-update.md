---
title: 更新 groupPolicyOperation
description: 更新 groupPolicyOperation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a2aac24a6cc4d5a121b364b25c3ee5d18c76faf0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145738"
---
# <a name="update-grouppolicyoperation"></a><span data-ttu-id="1aee5-103">更新 groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1aee5-103">Update groupPolicyOperation</span></span>

<span data-ttu-id="1aee5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aee5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1aee5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1aee5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aee5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1aee5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aee5-107">更新 [groupPolicyOperation 对象](../resources/intune-grouppolicy-grouppolicyoperation.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1aee5-107">Update the properties of a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aee5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1aee5-108">Prerequisites</span></span>
<span data-ttu-id="1aee5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1aee5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aee5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1aee5-111">Permission type</span></span>|<span data-ttu-id="1aee5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1aee5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aee5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1aee5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1aee5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aee5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1aee5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1aee5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aee5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1aee5-116">Not supported.</span></span>|
|<span data-ttu-id="1aee5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1aee5-117">Application</span></span>|<span data-ttu-id="1aee5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aee5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aee5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1aee5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="1aee5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1aee5-120">Request headers</span></span>
|<span data-ttu-id="1aee5-121">标头</span><span class="sxs-lookup"><span data-stu-id="1aee5-121">Header</span></span>|<span data-ttu-id="1aee5-122">值</span><span class="sxs-lookup"><span data-stu-id="1aee5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aee5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aee5-123">Authorization</span></span>|<span data-ttu-id="1aee5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1aee5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aee5-125">接受</span><span class="sxs-lookup"><span data-stu-id="1aee5-125">Accept</span></span>|<span data-ttu-id="1aee5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1aee5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aee5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1aee5-127">Request body</span></span>
<span data-ttu-id="1aee5-128">在请求正文中，提供 [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aee5-128">In the request body, supply a JSON representation for the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

<span data-ttu-id="1aee5-129">下表显示创建 [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1aee5-129">The following table shows the properties that are required when you create the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span></span>

|<span data-ttu-id="1aee5-130">属性</span><span class="sxs-lookup"><span data-stu-id="1aee5-130">Property</span></span>|<span data-ttu-id="1aee5-131">类型</span><span class="sxs-lookup"><span data-stu-id="1aee5-131">Type</span></span>|<span data-ttu-id="1aee5-132">说明</span><span class="sxs-lookup"><span data-stu-id="1aee5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aee5-133">operationType</span><span class="sxs-lookup"><span data-stu-id="1aee5-133">operationType</span></span>|[<span data-ttu-id="1aee5-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="1aee5-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="1aee5-135">组策略操作的类型。</span><span class="sxs-lookup"><span data-stu-id="1aee5-135">The type of group policy operation.</span></span> <span data-ttu-id="1aee5-136">可取值为：`none`、`upload`、`uploadNewVersion`、`addLanguageFiles`、`removeLanguageFiles`、`updateLanguageFiles` 或 `remove`。</span><span class="sxs-lookup"><span data-stu-id="1aee5-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="1aee5-137">operationStatus</span><span class="sxs-lookup"><span data-stu-id="1aee5-137">operationStatus</span></span>|[<span data-ttu-id="1aee5-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="1aee5-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="1aee5-139">组策略操作状态。</span><span class="sxs-lookup"><span data-stu-id="1aee5-139">The group policy operation status.</span></span> <span data-ttu-id="1aee5-140">可取值为：`unknown`、`inProgress`、`success`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="1aee5-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="1aee5-141">statusDetails</span><span class="sxs-lookup"><span data-stu-id="1aee5-141">statusDetails</span></span>|<span data-ttu-id="1aee5-142">String</span><span class="sxs-lookup"><span data-stu-id="1aee5-142">String</span></span>|<span data-ttu-id="1aee5-143">组策略操作状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="1aee5-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="1aee5-144">id</span><span class="sxs-lookup"><span data-stu-id="1aee5-144">id</span></span>|<span data-ttu-id="1aee5-145">String</span><span class="sxs-lookup"><span data-stu-id="1aee5-145">String</span></span>|<span data-ttu-id="1aee5-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1aee5-146">Key of the entity.</span></span>|
|<span data-ttu-id="1aee5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1aee5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1aee5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aee5-148">DateTimeOffset</span></span>|<span data-ttu-id="1aee5-149">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1aee5-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="1aee5-150">响应</span><span class="sxs-lookup"><span data-stu-id="1aee5-150">Response</span></span>
<span data-ttu-id="1aee5-151">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1aee5-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aee5-152">示例</span><span class="sxs-lookup"><span data-stu-id="1aee5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aee5-153">请求</span><span class="sxs-lookup"><span data-stu-id="1aee5-153">Request</span></span>
<span data-ttu-id="1aee5-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1aee5-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a><span data-ttu-id="1aee5-155">响应</span><span class="sxs-lookup"><span data-stu-id="1aee5-155">Response</span></span>
<span data-ttu-id="1aee5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1aee5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




