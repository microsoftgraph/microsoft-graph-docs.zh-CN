---
title: deploymentAudience：updateAudience
description: 更新 deploymentAudience 的成员和排除集合。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 23fe655e076987ffb33591eb8aaa1600ed4a8fa4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351123"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="c3f62-103">deploymentAudience：updateAudience</span><span class="sxs-lookup"><span data-stu-id="c3f62-103">deploymentAudience: updateAudience</span></span>

<span data-ttu-id="c3f62-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c3f62-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3f62-105">更新 [deploymentAudience](../resources/windowsupdates-deploymentaudience.md)的成员和排除集合。</span><span class="sxs-lookup"><span data-stu-id="c3f62-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="c3f62-106">向部署访问群体的成员或排除集合添加 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 会自动创建 Azure AD 设备对象（如果该对象不存在）。</span><span class="sxs-lookup"><span data-stu-id="c3f62-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="c3f62-107">如果 **deploymentAudience** 的排除和 **成员** 集合中包含相同的 [updatableAsset，](../resources/windowsupdates-updatableasset.md)则部署不会应用于该资产。 </span><span class="sxs-lookup"><span data-stu-id="c3f62-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="c3f62-108">如果 **所有 updatableAsset** 对象都是同一类型，则也可使用 [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) 方法更新 **deploymentAudience**。</span><span class="sxs-lookup"><span data-stu-id="c3f62-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

> [!NOTE]
> <span data-ttu-id="c3f62-109">此 API 具有 [与](/Graph/known-issues#accessing-and-updating-deployment-audiences) 通过 Intune 创建的部署相关的已知问题。</span><span class="sxs-lookup"><span data-stu-id="c3f62-109">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f62-110">权限</span><span class="sxs-lookup"><span data-stu-id="c3f62-110">Permissions</span></span>
<span data-ttu-id="c3f62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3f62-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3f62-113">Permission type</span></span>|<span data-ttu-id="c3f62-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3f62-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3f62-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3f62-115">Delegated (work or school account)</span></span>|<span data-ttu-id="c3f62-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f62-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c3f62-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3f62-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3f62-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3f62-118">Not supported.</span></span>|
|<span data-ttu-id="c3f62-119">Application</span><span class="sxs-lookup"><span data-stu-id="c3f62-119">Application</span></span>|<span data-ttu-id="c3f62-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f62-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3f62-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3f62-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="c3f62-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3f62-122">Request headers</span></span>
|<span data-ttu-id="c3f62-123">名称</span><span class="sxs-lookup"><span data-stu-id="c3f62-123">Name</span></span>|<span data-ttu-id="c3f62-124">说明</span><span class="sxs-lookup"><span data-stu-id="c3f62-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3f62-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3f62-125">Authorization</span></span>|<span data-ttu-id="c3f62-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3f62-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3f62-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3f62-128">Content-Type</span></span>|<span data-ttu-id="c3f62-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c3f62-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3f62-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3f62-131">Request body</span></span>
<span data-ttu-id="c3f62-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3f62-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c3f62-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c3f62-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c3f62-134">参数</span><span class="sxs-lookup"><span data-stu-id="c3f62-134">Parameter</span></span>|<span data-ttu-id="c3f62-135">类型</span><span class="sxs-lookup"><span data-stu-id="c3f62-135">Type</span></span>|<span data-ttu-id="c3f62-136">说明</span><span class="sxs-lookup"><span data-stu-id="c3f62-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3f62-137">addMembers</span><span class="sxs-lookup"><span data-stu-id="c3f62-137">addMembers</span></span>|<span data-ttu-id="c3f62-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3f62-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c3f62-139">要添加为部署访问群体成员的 [updatableAsset](../resources/windowsupdates-updatableasset.md) 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="c3f62-139">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="c3f62-140">removeMembers</span><span class="sxs-lookup"><span data-stu-id="c3f62-140">removeMembers</span></span>|<span data-ttu-id="c3f62-141">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3f62-141">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c3f62-142">要作为部署访问群体成员删除的可更新资源的列表。</span><span class="sxs-lookup"><span data-stu-id="c3f62-142">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="c3f62-143">addExclusions</span><span class="sxs-lookup"><span data-stu-id="c3f62-143">addExclusions</span></span>|<span data-ttu-id="c3f62-144">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3f62-144">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c3f62-145">要添加为部署访问群体排除项的可更新资源列表。</span><span class="sxs-lookup"><span data-stu-id="c3f62-145">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="c3f62-146">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="c3f62-146">removeExclusions</span></span>|<span data-ttu-id="c3f62-147">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3f62-147">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c3f62-148">要作为部署访问群体排除项删除的可更新资源的列表。</span><span class="sxs-lookup"><span data-stu-id="c3f62-148">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="c3f62-149">响应</span><span class="sxs-lookup"><span data-stu-id="c3f62-149">Response</span></span>

<span data-ttu-id="c3f62-150">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c3f62-150">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="c3f62-151">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c3f62-151">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3f62-152">示例</span><span class="sxs-lookup"><span data-stu-id="c3f62-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3f62-153">请求</span><span class="sxs-lookup"><span data-stu-id="c3f62-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c3f62-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f62-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudience"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-Type: application/json
Content-length: 599

{
  "addMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "addExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c3f62-155">C#</span><span class="sxs-lookup"><span data-stu-id="c3f62-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudience-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3f62-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3f62-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudience-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3f62-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3f62-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudience-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3f62-158">Java</span><span class="sxs-lookup"><span data-stu-id="c3f62-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudience-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c3f62-159">响应</span><span class="sxs-lookup"><span data-stu-id="c3f62-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

