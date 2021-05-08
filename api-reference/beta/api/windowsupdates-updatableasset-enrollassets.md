---
title: updatableAsset： enrollAssets
description: 在部署服务的更新管理中注册 updatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: e83dd02ded297cde0e80b535a9d4fcb01ed45ae6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241238"
---
# <a name="updatableasset-enrollassets"></a><span data-ttu-id="ef818-103">updatableAsset： enrollAssets</span><span class="sxs-lookup"><span data-stu-id="ef818-103">updatableAsset: enrollAssets</span></span>
<span data-ttu-id="ef818-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ef818-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef818-105">在 [部署服务的更新管理中注册 updatableAsset](../resources/windowsupdates-updatableasset.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="ef818-105">Enroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources in update management by the deployment service.</span></span>

<span data-ttu-id="ef818-106">可以在更新管理中注册[azureADDevice](../resources/windowsupdates-azureaddevice.md)资源，但不能在更新管理中注册[updatableAssetGroup。](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ef818-106">You can enroll an [azureADDevice](../resources/windowsupdates-azureaddevice.md) resource in update management, but may not enroll an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) in update management.</span></span>

<span data-ttu-id="ef818-107">在更新管理中注册 Azure AD 设备会自动创建 **azureADDevice** 对象（如果该对象不存在）。</span><span class="sxs-lookup"><span data-stu-id="ef818-107">Enrolling an Azure AD device in update management automatically creates an **azureADDevice** object if it does not already exist.</span></span>

<span data-ttu-id="ef818-108">您还可以使用 [enrollAssetsById 方法](windowsupdates-updatableasset-enrollassetsbyid.md) 注册资产。</span><span class="sxs-lookup"><span data-stu-id="ef818-108">You can also use the method [enrollAssetsById](windowsupdates-updatableasset-enrollassetsbyid.md) to enroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef818-109">权限</span><span class="sxs-lookup"><span data-stu-id="ef818-109">Permissions</span></span>
<span data-ttu-id="ef818-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef818-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef818-112">Permission type</span></span>|<span data-ttu-id="ef818-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef818-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef818-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef818-114">Delegated (work or school account)</span></span>|<span data-ttu-id="ef818-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef818-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="ef818-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef818-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef818-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef818-117">Not supported.</span></span>|
|<span data-ttu-id="ef818-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef818-118">Application</span></span>|<span data-ttu-id="ef818-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef818-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef818-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef818-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/enrollAssets
```

## <a name="request-headers"></a><span data-ttu-id="ef818-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef818-121">Request headers</span></span>
|<span data-ttu-id="ef818-122">名称</span><span class="sxs-lookup"><span data-stu-id="ef818-122">Name</span></span>|<span data-ttu-id="ef818-123">说明</span><span class="sxs-lookup"><span data-stu-id="ef818-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef818-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef818-124">Authorization</span></span>|<span data-ttu-id="ef818-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef818-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ef818-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef818-127">Content-Type</span></span>|<span data-ttu-id="ef818-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ef818-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef818-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef818-130">Request body</span></span>
<span data-ttu-id="ef818-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef818-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ef818-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ef818-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ef818-133">参数</span><span class="sxs-lookup"><span data-stu-id="ef818-133">Parameter</span></span>|<span data-ttu-id="ef818-134">类型</span><span class="sxs-lookup"><span data-stu-id="ef818-134">Type</span></span>|<span data-ttu-id="ef818-135">说明</span><span class="sxs-lookup"><span data-stu-id="ef818-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef818-136">updateCategory</span><span class="sxs-lookup"><span data-stu-id="ef818-136">updateCategory</span></span>|<span data-ttu-id="ef818-137">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="ef818-137">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="ef818-138">要管理的服务的更新类别。</span><span class="sxs-lookup"><span data-stu-id="ef818-138">The category of updates for the service to manage.</span></span> <span data-ttu-id="ef818-139">支持 **updateCategory** 值的子集。</span><span class="sxs-lookup"><span data-stu-id="ef818-139">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="ef818-140">可能的值是 `feature` ：。</span><span class="sxs-lookup"><span data-stu-id="ef818-140">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="ef818-141">assets</span><span class="sxs-lookup"><span data-stu-id="ef818-141">assets</span></span>|<span data-ttu-id="ef818-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef818-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ef818-143">要通过服务注册更新管理的 **updatableAsset** 资源列表，用于给定 **updateCategory**。</span><span class="sxs-lookup"><span data-stu-id="ef818-143">List of **updatableAsset** resources to enroll in update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="ef818-144">响应</span><span class="sxs-lookup"><span data-stu-id="ef818-144">Response</span></span>

<span data-ttu-id="ef818-145">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ef818-145">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="ef818-146">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ef818-146">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef818-147">示例</span><span class="sxs-lookup"><span data-stu-id="ef818-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef818-148">请求</span><span class="sxs-lookup"><span data-stu-id="ef818-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef818-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef818-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
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
# <a name="c"></a>[<span data-ttu-id="ef818-150">C#</span><span class="sxs-lookup"><span data-stu-id="ef818-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-enrollassets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef818-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef818-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-enrollassets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef818-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef818-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-enrollassets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef818-153">Java</span><span class="sxs-lookup"><span data-stu-id="ef818-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-enrollassets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ef818-154">响应</span><span class="sxs-lookup"><span data-stu-id="ef818-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

