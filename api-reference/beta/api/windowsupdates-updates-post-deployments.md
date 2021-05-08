---
title: 创建部署
description: 创建新的部署对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: b6ab12d7687d63a46684496c071fb4f9045a8786
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239183"
---
# <a name="create-deployment"></a><span data-ttu-id="c472a-103">创建部署</span><span class="sxs-lookup"><span data-stu-id="c472a-103">Create deployment</span></span>
<span data-ttu-id="c472a-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c472a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!NOTE]
> <span data-ttu-id="c472a-105">如果在创建 [部署时未指定](/graph/api/resources/windowsupdates-monitoringrule) 监视规则，则创建默认监视规则。</span><span class="sxs-lookup"><span data-stu-id="c472a-105">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a deployment, a default monitoring rule is created.</span></span> <span data-ttu-id="c472a-106">此默认监视规则具有 **信号**、阈值 和 `rollback`  `20` **操作** `alertError` 。</span><span class="sxs-lookup"><span data-stu-id="c472a-106">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="c472a-107">在 API 的未来更新中，此行为将更改，并且不会创建默认监视规则。</span><span class="sxs-lookup"><span data-stu-id="c472a-107">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

<span data-ttu-id="c472a-108">创建新的 [部署](../resources/windowsupdates-deployment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c472a-108">Create a new [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c472a-109">权限</span><span class="sxs-lookup"><span data-stu-id="c472a-109">Permissions</span></span>
<span data-ttu-id="c472a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c472a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c472a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c472a-112">Permission type</span></span>|<span data-ttu-id="c472a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c472a-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c472a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c472a-114">Delegated (work or school account)</span></span>|<span data-ttu-id="c472a-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c472a-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c472a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c472a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c472a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c472a-117">Not supported.</span></span>|
|<span data-ttu-id="c472a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c472a-118">Application</span></span>|<span data-ttu-id="c472a-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c472a-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c472a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c472a-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments
```

## <a name="request-headers"></a><span data-ttu-id="c472a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c472a-121">Request headers</span></span>
|<span data-ttu-id="c472a-122">名称</span><span class="sxs-lookup"><span data-stu-id="c472a-122">Name</span></span>|<span data-ttu-id="c472a-123">说明</span><span class="sxs-lookup"><span data-stu-id="c472a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c472a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c472a-124">Authorization</span></span>|<span data-ttu-id="c472a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c472a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c472a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c472a-127">Content-Type</span></span>|<span data-ttu-id="c472a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c472a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c472a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c472a-130">Request body</span></span>
<span data-ttu-id="c472a-131">在请求正文中，提供部署对象的 JSON [表示](../resources/windowsupdates-deployment.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="c472a-131">In the request body, supply a JSON representation of the [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

<span data-ttu-id="c472a-132">下表显示创建部署时所需的 [属性](../resources/windowsupdates-deployment.md)。</span><span class="sxs-lookup"><span data-stu-id="c472a-132">The following table shows the properties that are required when you create the [deployment](../resources/windowsupdates-deployment.md).</span></span>

|<span data-ttu-id="c472a-133">属性</span><span class="sxs-lookup"><span data-stu-id="c472a-133">Property</span></span>|<span data-ttu-id="c472a-134">类型</span><span class="sxs-lookup"><span data-stu-id="c472a-134">Type</span></span>|<span data-ttu-id="c472a-135">说明</span><span class="sxs-lookup"><span data-stu-id="c472a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c472a-136">内容</span><span class="sxs-lookup"><span data-stu-id="c472a-136">content</span></span>|[<span data-ttu-id="c472a-137">microsoft.graph.windowsUpdates.deployableContent</span><span class="sxs-lookup"><span data-stu-id="c472a-137">microsoft.graph.windowsUpdates.deployableContent</span></span>](../resources/windowsupdates-deployablecontent.md)|<span data-ttu-id="c472a-138">指定要部署的内容。</span><span class="sxs-lookup"><span data-stu-id="c472a-138">Specifies what content to deploy.</span></span> <span data-ttu-id="c472a-139">应作为以下派生类型之一提供可部署内容[：expeditedQualityUpdateReference、featureUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) [](../resources/windowsupdates-featureupdatereference.md)</span><span class="sxs-lookup"><span data-stu-id="c472a-139">Deployable content should be provided as one of the following derived types: [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md) , [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c472a-140">响应</span><span class="sxs-lookup"><span data-stu-id="c472a-140">Response</span></span>

<span data-ttu-id="c472a-141">如果成功，此方法在响应 `201 Created` 正文中返回 响应[](../resources/windowsupdates-deployment.md)代码和部署对象。</span><span class="sxs-lookup"><span data-stu-id="c472a-141">If successful, this method returns a `201 Created` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c472a-142">示例</span><span class="sxs-lookup"><span data-stu-id="c472a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c472a-143">请求</span><span class="sxs-lookup"><span data-stu-id="c472a-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c472a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c472a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_deployment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-Type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100
    },
    "monitoring": {
      "monitoringRules": [
        {
          "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c472a-145">C#</span><span class="sxs-lookup"><span data-stu-id="c472a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-deployment-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c472a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c472a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-deployment-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c472a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c472a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-deployment-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c472a-148">Java</span><span class="sxs-lookup"><span data-stu-id="c472a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-deployment-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c472a-149">响应</span><span class="sxs-lookup"><span data-stu-id="c472a-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "value": "offering",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "offeringByRequest"
      }
    ],
    "requestedValue": "none",
    "effectiveSinceDate": "String (timestamp)"
    },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "rollout": {
      "devicesPerOffer": 100,
      "durationBetweenOffers": "P7D",
      "startDateTime": null,
      "endDateTime": null
    },
    "monitoring": {
      "monitoringRules": [
        {
          "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    },
    "userExperience": null
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

