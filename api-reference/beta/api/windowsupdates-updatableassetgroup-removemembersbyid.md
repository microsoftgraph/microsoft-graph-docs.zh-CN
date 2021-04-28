---
title: updatableAssetGroup：removeMembersById
description: 从 updatableAssetGroup 中删除相同类型的成员。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1ea11298a7aa19d60b69b98b07c003887aae30b3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068005"
---
# <a name="updatableassetgroup-removemembersbyid"></a><span data-ttu-id="cc90b-103">updatableAssetGroup：removeMembersById</span><span class="sxs-lookup"><span data-stu-id="cc90b-103">updatableAssetGroup: removeMembersById</span></span>
<span data-ttu-id="cc90b-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="cc90b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc90b-105">从 [updatableAssetGroup 中删除相同类型的成员](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="cc90b-105">Remove members of the same type from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="cc90b-106">您还可以使用 [removeMembers 方法](windowsupdates-updatableassetgroup-removemembers.md) 删除成员。</span><span class="sxs-lookup"><span data-stu-id="cc90b-106">You can also use the method [removeMembers](windowsupdates-updatableassetgroup-removemembers.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc90b-107">权限</span><span class="sxs-lookup"><span data-stu-id="cc90b-107">Permissions</span></span>
<span data-ttu-id="cc90b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc90b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc90b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc90b-110">Permission type</span></span>|<span data-ttu-id="cc90b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc90b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc90b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc90b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc90b-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc90b-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="cc90b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc90b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc90b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc90b-115">Not supported.</span></span>|
|<span data-ttu-id="cc90b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc90b-116">Application</span></span>|<span data-ttu-id="cc90b-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc90b-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc90b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc90b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
```

## <a name="request-headers"></a><span data-ttu-id="cc90b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc90b-119">Request headers</span></span>
|<span data-ttu-id="cc90b-120">名称</span><span class="sxs-lookup"><span data-stu-id="cc90b-120">Name</span></span>|<span data-ttu-id="cc90b-121">说明</span><span class="sxs-lookup"><span data-stu-id="cc90b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cc90b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc90b-122">Authorization</span></span>|<span data-ttu-id="cc90b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc90b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cc90b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc90b-125">Content-Type</span></span>|<span data-ttu-id="cc90b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cc90b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc90b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc90b-128">Request body</span></span>
<span data-ttu-id="cc90b-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc90b-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cc90b-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="cc90b-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cc90b-131">参数</span><span class="sxs-lookup"><span data-stu-id="cc90b-131">Parameter</span></span>|<span data-ttu-id="cc90b-132">类型</span><span class="sxs-lookup"><span data-stu-id="cc90b-132">Type</span></span>|<span data-ttu-id="cc90b-133">说明</span><span class="sxs-lookup"><span data-stu-id="cc90b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc90b-134">ids</span><span class="sxs-lookup"><span data-stu-id="cc90b-134">ids</span></span>|<span data-ttu-id="cc90b-135">String collection</span><span class="sxs-lookup"><span data-stu-id="cc90b-135">String collection</span></span>|<span data-ttu-id="cc90b-136">与要作为 [updatableAssetGroup](../resources/windowsupdates-updatableasset.md) 成员删除的 **updatableAsset** 资源对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="cc90b-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to remove as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="cc90b-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="cc90b-137">memberEntityType</span></span>|<span data-ttu-id="cc90b-138">String</span><span class="sxs-lookup"><span data-stu-id="cc90b-138">String</span></span>|<span data-ttu-id="cc90b-139">**updatableAsset 资源的完整** 类型。</span><span class="sxs-lookup"><span data-stu-id="cc90b-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="cc90b-140">可能的值是 `#microsoft.graph.windowsUpdates.azureADDevice` ：。</span><span class="sxs-lookup"><span data-stu-id="cc90b-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="cc90b-141">响应</span><span class="sxs-lookup"><span data-stu-id="cc90b-141">Response</span></span>

<span data-ttu-id="cc90b-142">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cc90b-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="cc90b-143">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cc90b-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc90b-144">示例</span><span class="sxs-lookup"><span data-stu-id="cc90b-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc90b-145">请求</span><span class="sxs-lookup"><span data-stu-id="cc90b-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
Content-Type: application/json

{
  "ids": [
    "String",
    "String",
    "String"
  ],
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice"
}
```

### <a name="response"></a><span data-ttu-id="cc90b-146">响应</span><span class="sxs-lookup"><span data-stu-id="cc90b-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

