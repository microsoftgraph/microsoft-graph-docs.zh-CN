---
title: updatableAsset：unenrollAssets
description: 从部署服务的更新管理中注销 updatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 8f32ca029e94da476eb1b6c491057a3d4343b523
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317187"
---
# <a name="updatableasset-unenrollassets"></a><span data-ttu-id="fe646-103">updatableAsset：unenrollAssets</span><span class="sxs-lookup"><span data-stu-id="fe646-103">updatableAsset: unenrollAssets</span></span>
<span data-ttu-id="fe646-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="fe646-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe646-105">从部署服务的更新管理中注销 [updatableAsset](../resources/windowsupdates-updatableasset.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="fe646-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from update management by the deployment service.</span></span>

<span data-ttu-id="fe646-106">您还可以使用 [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) 方法注销资产。</span><span class="sxs-lookup"><span data-stu-id="fe646-106">You can also use the method [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) to unenroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe646-107">权限</span><span class="sxs-lookup"><span data-stu-id="fe646-107">Permissions</span></span>
<span data-ttu-id="fe646-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe646-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe646-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe646-110">Permission type</span></span>|<span data-ttu-id="fe646-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe646-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe646-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe646-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe646-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe646-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="fe646-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe646-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe646-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe646-115">Not supported.</span></span>|
|<span data-ttu-id="fe646-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe646-116">Application</span></span>|<span data-ttu-id="fe646-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe646-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe646-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe646-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/unenrollAssets
```

## <a name="request-headers"></a><span data-ttu-id="fe646-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe646-119">Request headers</span></span>
|<span data-ttu-id="fe646-120">名称</span><span class="sxs-lookup"><span data-stu-id="fe646-120">Name</span></span>|<span data-ttu-id="fe646-121">说明</span><span class="sxs-lookup"><span data-stu-id="fe646-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fe646-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe646-122">Authorization</span></span>|<span data-ttu-id="fe646-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe646-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe646-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe646-125">Content-Type</span></span>|<span data-ttu-id="fe646-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fe646-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe646-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe646-128">Request body</span></span>
<span data-ttu-id="fe646-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe646-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fe646-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="fe646-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fe646-131">参数</span><span class="sxs-lookup"><span data-stu-id="fe646-131">Parameter</span></span>|<span data-ttu-id="fe646-132">类型</span><span class="sxs-lookup"><span data-stu-id="fe646-132">Type</span></span>|<span data-ttu-id="fe646-133">说明</span><span class="sxs-lookup"><span data-stu-id="fe646-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe646-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="fe646-134">updateCategory</span></span>|<span data-ttu-id="fe646-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="fe646-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="fe646-136">要停止管理的服务的更新类别。</span><span class="sxs-lookup"><span data-stu-id="fe646-136">The category of updates for the service to stop managing.</span></span> <span data-ttu-id="fe646-137">支持 **updateCategory** 值的子集。</span><span class="sxs-lookup"><span data-stu-id="fe646-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="fe646-138">可能的值是 `feature` ：。</span><span class="sxs-lookup"><span data-stu-id="fe646-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="fe646-139">assets</span><span class="sxs-lookup"><span data-stu-id="fe646-139">assets</span></span>|<span data-ttu-id="fe646-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe646-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="fe646-141">要从服务的更新管理中注销的 **updatableAsset** 资源列表，用于给定 **updateCategory**。</span><span class="sxs-lookup"><span data-stu-id="fe646-141">List of **updatableAsset** resources to unenroll from update management by the service for the given **updateCategory**.</span></span>|



## <a name="response"></a><span data-ttu-id="fe646-142">响应</span><span class="sxs-lookup"><span data-stu-id="fe646-142">Response</span></span>

<span data-ttu-id="fe646-143">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fe646-143">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="fe646-144">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fe646-144">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe646-145">示例</span><span class="sxs-lookup"><span data-stu-id="fe646-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe646-146">请求</span><span class="sxs-lookup"><span data-stu-id="fe646-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="fe646-147">响应</span><span class="sxs-lookup"><span data-stu-id="fe646-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

