---
title: 更新部署
description: 更新部署对象的属性。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 68654adf5bba14c98b19acab47880008c4d18b08
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241306"
---
# <a name="update-deployment"></a><span data-ttu-id="f6559-103">更新部署</span><span class="sxs-lookup"><span data-stu-id="f6559-103">Update deployment</span></span>
<span data-ttu-id="f6559-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f6559-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6559-105">更新 [部署对象的属性](../resources/windowsupdates-deployment.md) 。</span><span class="sxs-lookup"><span data-stu-id="f6559-105">Update the properties of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6559-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6559-106">Permissions</span></span>
<span data-ttu-id="f6559-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6559-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6559-109">Permission type</span></span>|<span data-ttu-id="f6559-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6559-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6559-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6559-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6559-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6559-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f6559-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6559-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6559-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6559-114">Not supported.</span></span>|
|<span data-ttu-id="f6559-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6559-115">Application</span></span>|<span data-ttu-id="f6559-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6559-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6559-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6559-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="f6559-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6559-118">Request headers</span></span>
|<span data-ttu-id="f6559-119">名称</span><span class="sxs-lookup"><span data-stu-id="f6559-119">Name</span></span>|<span data-ttu-id="f6559-120">说明</span><span class="sxs-lookup"><span data-stu-id="f6559-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6559-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6559-121">Authorization</span></span>|<span data-ttu-id="f6559-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6559-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f6559-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6559-124">Content-Type</span></span>|<span data-ttu-id="f6559-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f6559-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6559-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6559-127">Request body</span></span>
<span data-ttu-id="f6559-128">在请求正文中，提供部署对象的 JSON [表示](../resources/windowsupdates-deployment.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="f6559-128">In the request body, supply a JSON representation of the [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

<span data-ttu-id="f6559-129">下表显示更新部署时可以设置 [的属性](../resources/windowsupdates-deployment.md)。</span><span class="sxs-lookup"><span data-stu-id="f6559-129">The following table shows the properties that can be set when you update the [deployment](../resources/windowsupdates-deployment.md).</span></span>

|<span data-ttu-id="f6559-130">属性</span><span class="sxs-lookup"><span data-stu-id="f6559-130">Property</span></span>|<span data-ttu-id="f6559-131">类型</span><span class="sxs-lookup"><span data-stu-id="f6559-131">Type</span></span>|<span data-ttu-id="f6559-132">说明</span><span class="sxs-lookup"><span data-stu-id="f6559-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6559-133">state</span><span class="sxs-lookup"><span data-stu-id="f6559-133">state</span></span>|[<span data-ttu-id="f6559-134">microsoft.graph.windowsUpdates.deploymentState</span><span class="sxs-lookup"><span data-stu-id="f6559-134">microsoft.graph.windowsUpdates.deploymentState</span></span>](../resources/windowsupdates-deploymentstate.md)|<span data-ttu-id="f6559-135">部署的执行状态。</span><span class="sxs-lookup"><span data-stu-id="f6559-135">Execution status of the deployment.</span></span>|
|<span data-ttu-id="f6559-136">设置</span><span class="sxs-lookup"><span data-stu-id="f6559-136">settings</span></span>|[<span data-ttu-id="f6559-137">microsoft.graph.windowsUpdates.deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="f6559-137">microsoft.graph.windowsUpdates.deploymentSettings</span></span>](../resources/windowsupdates-deploymentsettings.md)|<span data-ttu-id="f6559-138">设置管理如何部署部署的特定部署中指定的策略 `content` 。</span><span class="sxs-lookup"><span data-stu-id="f6559-138">Settings specified on the specific deployment governing how to deploy deployment `content`.</span></span>|


## <a name="response"></a><span data-ttu-id="f6559-139">响应</span><span class="sxs-lookup"><span data-stu-id="f6559-139">Response</span></span>

<span data-ttu-id="f6559-140">如果成功，此方法在响应 `202 Accepted` 正文中返回 响应代码[](../resources/windowsupdates-deployment.md)和更新的部署对象。</span><span class="sxs-lookup"><span data-stu-id="f6559-140">If successful, this method returns a `202 Accepted` response code and an updated [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6559-141">示例</span><span class="sxs-lookup"><span data-stu-id="f6559-141">Examples</span></span>

### <a name="example-pause-a-deployment"></a><span data-ttu-id="f6559-142">示例：暂停部署</span><span class="sxs-lookup"><span data-stu-id="f6559-142">Example: Pause a deployment</span></span>

<span data-ttu-id="f6559-143">在此例中，部署通过更新 部署 `requestedValue` 暂停 `state` 。</span><span class="sxs-lookup"><span data-stu-id="f6559-143">In this example, the deployment is paused by updating the `requestedValue` of the deployment `state`.</span></span>

#### <a name="request"></a><span data-ttu-id="f6559-144">请求</span><span class="sxs-lookup"><span data-stu-id="f6559-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6559-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6559-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_deployment",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "requestedValue": "paused"
  },
}
```
# <a name="c"></a>[<span data-ttu-id="f6559-146">C#</span><span class="sxs-lookup"><span data-stu-id="f6559-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6559-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6559-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6559-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6559-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6559-149">Java</span><span class="sxs-lookup"><span data-stu-id="f6559-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="f6559-150">响应</span><span class="sxs-lookup"><span data-stu-id="f6559-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "pausedByRequest"
      }
    ],
    "requestedValue": "paused",
    "value": "paused"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": null,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-update-deployment-settings-to-add-a-monitoring-rule"></a><span data-ttu-id="f6559-151">示例：更新部署设置以添加监视规则</span><span class="sxs-lookup"><span data-stu-id="f6559-151">Example: Update deployment settings to add a monitoring rule</span></span>

<span data-ttu-id="f6559-152">此示例更新 `settings` 了部署的 属性以添加监视规则。</span><span class="sxs-lookup"><span data-stu-id="f6559-152">In this example, the `settings` property of the deployment is updated to add a monitoring rule.</span></span>

#### <a name="request"></a><span data-ttu-id="f6559-153">请求</span><span class="sxs-lookup"><span data-stu-id="f6559-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_deployment",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "monitoring": {
      "monitoringRules": [
        {
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  }
}
```


#### <a name="response"></a><span data-ttu-id="f6559-154">响应</span><span class="sxs-lookup"><span data-stu-id="f6559-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "offeringByRequest"
      }
    ],
    "requestedValue": "none",
    "value": "offering"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "monitoring": {
      "monitoringRules": [
        {
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

