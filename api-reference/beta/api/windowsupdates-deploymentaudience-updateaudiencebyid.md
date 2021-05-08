---
title: deploymentAudience：updateAudienceById
description: 使用相同类型的 updatableAsset 资源更新 deploymentAudience 的成员和排除集合。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 81404ad4807f045b75b3b161ec361f06b622f78b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240576"
---
# <a name="deploymentaudience-updateaudiencebyid"></a><span data-ttu-id="44993-103">deploymentAudience：updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="44993-103">deploymentAudience: updateAudienceById</span></span>
<span data-ttu-id="44993-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="44993-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44993-105">使用相同类型的[updatableAsset](../resources/windowsupdates-updatableasset.md)资源更新[deploymentAudience](../resources/windowsupdates-deploymentaudience.md)的成员和排除集合。</span><span class="sxs-lookup"><span data-stu-id="44993-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) with [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type.</span></span>

<span data-ttu-id="44993-106">向部署访问群体的成员或排除集合添加 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 会自动创建 Azure AD 设备对象（如果该对象不存在）。</span><span class="sxs-lookup"><span data-stu-id="44993-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object if it does not already exist.</span></span>

<span data-ttu-id="44993-107">如果 **deploymentAudience** 的排除和 **成员** 集合中包含相同的 [updatableAsset，](../resources/windowsupdates-updatableasset.md)则部署不会应用于该资产。 </span><span class="sxs-lookup"><span data-stu-id="44993-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="44993-108">您还可以使用 [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) 方法来更新 **deploymentAudience**。</span><span class="sxs-lookup"><span data-stu-id="44993-108">You can also use the method [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="44993-109">权限</span><span class="sxs-lookup"><span data-stu-id="44993-109">Permissions</span></span>
<span data-ttu-id="44993-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44993-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="44993-112">Permission type</span></span>|<span data-ttu-id="44993-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44993-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44993-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44993-114">Delegated (work or school account)</span></span>|<span data-ttu-id="44993-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44993-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="44993-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44993-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44993-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="44993-117">Not supported.</span></span>|
|<span data-ttu-id="44993-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="44993-118">Application</span></span>|<span data-ttu-id="44993-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44993-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44993-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44993-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a><span data-ttu-id="44993-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="44993-121">Request headers</span></span>
|<span data-ttu-id="44993-122">名称</span><span class="sxs-lookup"><span data-stu-id="44993-122">Name</span></span>|<span data-ttu-id="44993-123">说明</span><span class="sxs-lookup"><span data-stu-id="44993-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="44993-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="44993-124">Authorization</span></span>|<span data-ttu-id="44993-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44993-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="44993-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44993-127">Content-Type</span></span>|<span data-ttu-id="44993-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="44993-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44993-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="44993-130">Request body</span></span>
<span data-ttu-id="44993-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44993-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="44993-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="44993-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="44993-133">参数</span><span class="sxs-lookup"><span data-stu-id="44993-133">Parameter</span></span>|<span data-ttu-id="44993-134">类型</span><span class="sxs-lookup"><span data-stu-id="44993-134">Type</span></span>|<span data-ttu-id="44993-135">说明</span><span class="sxs-lookup"><span data-stu-id="44993-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44993-136">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="44993-136">memberEntityType</span></span>|<span data-ttu-id="44993-137">字符串</span><span class="sxs-lookup"><span data-stu-id="44993-137">String</span></span>|<span data-ttu-id="44993-138">可更新资源的完整类型。</span><span class="sxs-lookup"><span data-stu-id="44993-138">The full type of the updatable assets.</span></span> <span data-ttu-id="44993-139">可取值为：`#microsoft.graph.windowsUpdates.azureADDevice`、`#microsoft.graph.windowsUpdates.updatableAssetGroup`。</span><span class="sxs-lookup"><span data-stu-id="44993-139">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span></span>|
|<span data-ttu-id="44993-140">addMembers</span><span class="sxs-lookup"><span data-stu-id="44993-140">addMembers</span></span>|<span data-ttu-id="44993-141">String collection</span><span class="sxs-lookup"><span data-stu-id="44993-141">String collection</span></span>|<span data-ttu-id="44993-142">与要添加为部署访问群体成员的可更新资产对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="44993-142">List of identifiers corresponding to the updatable assets to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="44993-143">removeMembers</span><span class="sxs-lookup"><span data-stu-id="44993-143">removeMembers</span></span>|<span data-ttu-id="44993-144">String collection</span><span class="sxs-lookup"><span data-stu-id="44993-144">String collection</span></span>|<span data-ttu-id="44993-145">与要作为部署访问群体成员删除的可更新资源相对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="44993-145">List of identifiers corresponding to the updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="44993-146">addExclusions</span><span class="sxs-lookup"><span data-stu-id="44993-146">addExclusions</span></span>|<span data-ttu-id="44993-147">String collection</span><span class="sxs-lookup"><span data-stu-id="44993-147">String collection</span></span>|<span data-ttu-id="44993-148">与要作为部署访问群体排除项添加的可更新资源相对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="44993-148">List of identifiers corresponding to the updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="44993-149">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="44993-149">removeExclusions</span></span>|<span data-ttu-id="44993-150">String collection</span><span class="sxs-lookup"><span data-stu-id="44993-150">String collection</span></span>|<span data-ttu-id="44993-151">与要作为部署访问群体排除项删除的可更新资源相对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="44993-151">List of identifiers corresponding to the updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="44993-152">响应</span><span class="sxs-lookup"><span data-stu-id="44993-152">Response</span></span>

<span data-ttu-id="44993-153">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="44993-153">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="44993-154">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="44993-154">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44993-155">示例</span><span class="sxs-lookup"><span data-stu-id="44993-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44993-156">请求</span><span class="sxs-lookup"><span data-stu-id="44993-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="44993-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="44993-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudiencebyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
Content-Type: application/json
Content-length: 204

{
  "memberEntityType": "String",
  "addMembers": [
    "String"
  ],
  "removeMembers": [
    "String"
  ],
  "addExclusions": [
    "String"
  ],
  "removeExclusions": [
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="44993-158">C#</span><span class="sxs-lookup"><span data-stu-id="44993-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44993-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44993-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44993-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44993-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44993-161">Java</span><span class="sxs-lookup"><span data-stu-id="44993-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="44993-162">响应</span><span class="sxs-lookup"><span data-stu-id="44993-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

