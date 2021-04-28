---
title: deploymentAudience：updateAudience
description: 更新 deploymentAudience 的成员和排除集合。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a0567070f4042896835b735fa69b5cd1dddeb1a3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067337"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="89fda-103">deploymentAudience：updateAudience</span><span class="sxs-lookup"><span data-stu-id="89fda-103">deploymentAudience: updateAudience</span></span>
<span data-ttu-id="89fda-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="89fda-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89fda-105">更新 [deploymentAudience](../resources/windowsupdates-deploymentaudience.md)的成员和排除集合。</span><span class="sxs-lookup"><span data-stu-id="89fda-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="89fda-106">向部署访问群体的成员或排除集合添加 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 会自动创建 Azure AD 设备对象（如果该对象不存在）。</span><span class="sxs-lookup"><span data-stu-id="89fda-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="89fda-107">如果 **deploymentAudience** 的排除和 **成员** 集合中包含相同的 [updatableAsset，](../resources/windowsupdates-updatableasset.md)则部署不会应用于该资产。 </span><span class="sxs-lookup"><span data-stu-id="89fda-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="89fda-108">如果 **所有 updatableAsset** 对象都是同一类型，则也可使用 [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) 方法更新 **deploymentAudience**。</span><span class="sxs-lookup"><span data-stu-id="89fda-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="89fda-109">权限</span><span class="sxs-lookup"><span data-stu-id="89fda-109">Permissions</span></span>
<span data-ttu-id="89fda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89fda-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="89fda-112">Permission type</span></span>|<span data-ttu-id="89fda-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89fda-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89fda-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89fda-114">Delegated (work or school account)</span></span>|<span data-ttu-id="89fda-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89fda-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="89fda-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89fda-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89fda-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="89fda-117">Not supported.</span></span>|
|<span data-ttu-id="89fda-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="89fda-118">Application</span></span>|<span data-ttu-id="89fda-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89fda-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89fda-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89fda-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="89fda-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="89fda-121">Request headers</span></span>
|<span data-ttu-id="89fda-122">名称</span><span class="sxs-lookup"><span data-stu-id="89fda-122">Name</span></span>|<span data-ttu-id="89fda-123">说明</span><span class="sxs-lookup"><span data-stu-id="89fda-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89fda-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89fda-124">Authorization</span></span>|<span data-ttu-id="89fda-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89fda-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="89fda-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89fda-127">Content-Type</span></span>|<span data-ttu-id="89fda-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="89fda-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89fda-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="89fda-130">Request body</span></span>
<span data-ttu-id="89fda-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89fda-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="89fda-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="89fda-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="89fda-133">参数</span><span class="sxs-lookup"><span data-stu-id="89fda-133">Parameter</span></span>|<span data-ttu-id="89fda-134">类型</span><span class="sxs-lookup"><span data-stu-id="89fda-134">Type</span></span>|<span data-ttu-id="89fda-135">说明</span><span class="sxs-lookup"><span data-stu-id="89fda-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89fda-136">addMembers</span><span class="sxs-lookup"><span data-stu-id="89fda-136">addMembers</span></span>|<span data-ttu-id="89fda-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89fda-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="89fda-138">要添加为部署访问群体成员的 [updatableAsset](../resources/windowsupdates-updatableasset.md) 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="89fda-138">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="89fda-139">removeMembers</span><span class="sxs-lookup"><span data-stu-id="89fda-139">removeMembers</span></span>|<span data-ttu-id="89fda-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89fda-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="89fda-141">要作为部署访问群体成员删除的可更新资源的列表。</span><span class="sxs-lookup"><span data-stu-id="89fda-141">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="89fda-142">addExclusions</span><span class="sxs-lookup"><span data-stu-id="89fda-142">addExclusions</span></span>|<span data-ttu-id="89fda-143">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89fda-143">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="89fda-144">要添加为部署访问群体排除项的可更新资源列表。</span><span class="sxs-lookup"><span data-stu-id="89fda-144">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="89fda-145">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="89fda-145">removeExclusions</span></span>|<span data-ttu-id="89fda-146">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89fda-146">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="89fda-147">要作为部署访问群体排除项删除的可更新资源的列表。</span><span class="sxs-lookup"><span data-stu-id="89fda-147">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="89fda-148">响应</span><span class="sxs-lookup"><span data-stu-id="89fda-148">Response</span></span>

<span data-ttu-id="89fda-149">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="89fda-149">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="89fda-150">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="89fda-150">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89fda-151">示例</span><span class="sxs-lookup"><span data-stu-id="89fda-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89fda-152">请求</span><span class="sxs-lookup"><span data-stu-id="89fda-152">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="89fda-153">响应</span><span class="sxs-lookup"><span data-stu-id="89fda-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

