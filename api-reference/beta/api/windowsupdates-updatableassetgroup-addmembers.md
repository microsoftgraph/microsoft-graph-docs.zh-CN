---
title: updatableAssetGroup：addMembers
description: 将成员添加到 updatableAssetGroup。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 99d56de596cb28f21bffdd915911fd6ca6c9417f
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316475"
---
# <a name="updatableassetgroup-addmembers"></a><span data-ttu-id="ee2f5-103">updatableAssetGroup：addMembers</span><span class="sxs-lookup"><span data-stu-id="ee2f5-103">updatableAssetGroup: addMembers</span></span>
<span data-ttu-id="ee2f5-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ee2f5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee2f5-105">将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-105">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="ee2f5-106">可以将 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源添加为成员，但不能将 **updatableAssetGroup** 资源添加为成员。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-106">You can add [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources as members, but may not add **updatableAssetGroup** resources as members.</span></span>

<span data-ttu-id="ee2f5-107">将 Azure AD 设备添加为可更新资源组的成员会自动创建 **azureADDevice** 对象（如果该对象不存在）。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-107">Adding an Azure AD device as a member of an updatable asset group automatically creates an **azureADDevice** object, if it does not already exist.</span></span>

<span data-ttu-id="ee2f5-108">您还可以使用 [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) 方法添加成员。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-108">You can also use the method [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee2f5-109">权限</span><span class="sxs-lookup"><span data-stu-id="ee2f5-109">Permissions</span></span>
<span data-ttu-id="ee2f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee2f5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee2f5-112">Permission type</span></span>|<span data-ttu-id="ee2f5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee2f5-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee2f5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee2f5-114">Delegated (work or school account)</span></span>|<span data-ttu-id="ee2f5-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee2f5-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="ee2f5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee2f5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee2f5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-117">Not supported.</span></span>|
|<span data-ttu-id="ee2f5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee2f5-118">Application</span></span>|<span data-ttu-id="ee2f5-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee2f5-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee2f5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee2f5-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers
```

## <a name="request-headers"></a><span data-ttu-id="ee2f5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee2f5-121">Request headers</span></span>
|<span data-ttu-id="ee2f5-122">名称</span><span class="sxs-lookup"><span data-stu-id="ee2f5-122">Name</span></span>|<span data-ttu-id="ee2f5-123">说明</span><span class="sxs-lookup"><span data-stu-id="ee2f5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee2f5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee2f5-124">Authorization</span></span>|<span data-ttu-id="ee2f5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee2f5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee2f5-127">Content-Type</span></span>|<span data-ttu-id="ee2f5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ee2f5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee2f5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee2f5-130">Request body</span></span>
<span data-ttu-id="ee2f5-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ee2f5-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ee2f5-133">参数</span><span class="sxs-lookup"><span data-stu-id="ee2f5-133">Parameter</span></span>|<span data-ttu-id="ee2f5-134">类型</span><span class="sxs-lookup"><span data-stu-id="ee2f5-134">Type</span></span>|<span data-ttu-id="ee2f5-135">说明</span><span class="sxs-lookup"><span data-stu-id="ee2f5-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee2f5-136">assets</span><span class="sxs-lookup"><span data-stu-id="ee2f5-136">assets</span></span>|<span data-ttu-id="ee2f5-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee2f5-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ee2f5-138">要 **添加为 updatableAssetGroup** 成员的 **updatableAsset 资源列表**。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-138">List of **updatableAsset** resources to add as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="ee2f5-139">响应</span><span class="sxs-lookup"><span data-stu-id="ee2f5-139">Response</span></span>

<span data-ttu-id="ee2f5-140">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-140">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="ee2f5-141">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ee2f5-141">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee2f5-142">示例</span><span class="sxs-lookup"><span data-stu-id="ee2f5-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee2f5-143">请求</span><span class="sxs-lookup"><span data-stu-id="ee2f5-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers
Content-Type: application/json

{
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ee2f5-144">响应</span><span class="sxs-lookup"><span data-stu-id="ee2f5-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
