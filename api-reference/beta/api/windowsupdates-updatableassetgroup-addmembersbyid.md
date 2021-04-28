---
title: updatableAssetGroup：addMembersById
description: 将相同类型的成员添加到 updatableAssetGroup。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 004b8600644f6fcc8a599b53761f66491f62ebd8
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067332"
---
# <a name="updatableassetgroup-addmembersbyid"></a><span data-ttu-id="54d6e-103">updatableAssetGroup：addMembersById</span><span class="sxs-lookup"><span data-stu-id="54d6e-103">updatableAssetGroup: addMembersById</span></span>
<span data-ttu-id="54d6e-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="54d6e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54d6e-105">将相同类型的成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="54d6e-105">Add members of the same type to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="54d6e-106">您还可以使用 [addMembers 方法](windowsupdates-updatableassetgroup-addmembers.md) 添加成员。</span><span class="sxs-lookup"><span data-stu-id="54d6e-106">You can also use the method [addMembers](windowsupdates-updatableassetgroup-addmembers.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d6e-107">权限</span><span class="sxs-lookup"><span data-stu-id="54d6e-107">Permissions</span></span>
<span data-ttu-id="54d6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54d6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d6e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="54d6e-110">Permission type</span></span>|<span data-ttu-id="54d6e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54d6e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54d6e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54d6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54d6e-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d6e-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="54d6e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54d6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54d6e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54d6e-115">Not supported.</span></span>|
|<span data-ttu-id="54d6e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54d6e-116">Application</span></span>|<span data-ttu-id="54d6e-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d6e-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54d6e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54d6e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
```

## <a name="request-headers"></a><span data-ttu-id="54d6e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54d6e-119">Request headers</span></span>
|<span data-ttu-id="54d6e-120">名称</span><span class="sxs-lookup"><span data-stu-id="54d6e-120">Name</span></span>|<span data-ttu-id="54d6e-121">说明</span><span class="sxs-lookup"><span data-stu-id="54d6e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="54d6e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54d6e-122">Authorization</span></span>|<span data-ttu-id="54d6e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54d6e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="54d6e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54d6e-125">Content-Type</span></span>|<span data-ttu-id="54d6e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="54d6e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54d6e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="54d6e-128">Request body</span></span>
<span data-ttu-id="54d6e-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54d6e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="54d6e-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="54d6e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="54d6e-131">参数</span><span class="sxs-lookup"><span data-stu-id="54d6e-131">Parameter</span></span>|<span data-ttu-id="54d6e-132">类型</span><span class="sxs-lookup"><span data-stu-id="54d6e-132">Type</span></span>|<span data-ttu-id="54d6e-133">说明</span><span class="sxs-lookup"><span data-stu-id="54d6e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54d6e-134">ids</span><span class="sxs-lookup"><span data-stu-id="54d6e-134">ids</span></span>|<span data-ttu-id="54d6e-135">String collection</span><span class="sxs-lookup"><span data-stu-id="54d6e-135">String collection</span></span>|<span data-ttu-id="54d6e-136">与要添加为 [updatableAssetGroup](../resources/windowsupdates-updatableasset.md) 成员的 **updatableAsset** 资源相对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="54d6e-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="54d6e-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="54d6e-137">memberEntityType</span></span>|<span data-ttu-id="54d6e-138">String</span><span class="sxs-lookup"><span data-stu-id="54d6e-138">String</span></span>|<span data-ttu-id="54d6e-139">**updatableAsset 资源的完整** 类型。</span><span class="sxs-lookup"><span data-stu-id="54d6e-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="54d6e-140">可能的值是 `#microsoft.graph.windowsUpdates.azureADDevice` ：。</span><span class="sxs-lookup"><span data-stu-id="54d6e-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="54d6e-141">响应</span><span class="sxs-lookup"><span data-stu-id="54d6e-141">Response</span></span>

<span data-ttu-id="54d6e-142">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54d6e-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="54d6e-143">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="54d6e-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54d6e-144">示例</span><span class="sxs-lookup"><span data-stu-id="54d6e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54d6e-145">请求</span><span class="sxs-lookup"><span data-stu-id="54d6e-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
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

### <a name="response"></a><span data-ttu-id="54d6e-146">响应</span><span class="sxs-lookup"><span data-stu-id="54d6e-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

