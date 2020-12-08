---
title: 创建 unifiedGroupSource
description: 创建新的 unifiedGroupSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f92fa2454b7ab20946091784af11b23ef2252acc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597510"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="cb6e0-103">创建 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="cb6e0-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="cb6e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb6e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb6e0-105">创建新的 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-105">Create a new [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb6e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb6e0-106">Permissions</span></span>

<span data-ttu-id="cb6e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb6e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb6e0-109">Permission type</span></span>|<span data-ttu-id="cb6e0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb6e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb6e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb6e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb6e0-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="cb6e0-112">User.Read</span></span>|
|<span data-ttu-id="cb6e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb6e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb6e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-114">Not supported.</span></span>|
|<span data-ttu-id="cb6e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb6e0-115">Application</span></span>|<span data-ttu-id="cb6e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb6e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb6e0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="cb6e0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb6e0-118">Request headers</span></span>

|<span data-ttu-id="cb6e0-119">名称</span><span class="sxs-lookup"><span data-stu-id="cb6e0-119">Name</span></span>|<span data-ttu-id="cb6e0-120">说明</span><span class="sxs-lookup"><span data-stu-id="cb6e0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb6e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb6e0-121">Authorization</span></span>|<span data-ttu-id="cb6e0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cb6e0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb6e0-124">Content-Type</span></span>|<span data-ttu-id="cb6e0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cb6e0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb6e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb6e0-127">Request body</span></span>

<span data-ttu-id="cb6e0-128">在请求正文中，提供 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="cb6e0-129">下表显示创建 [unifiedGroupSource](../resources/unifiedgroupsource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/unifiedgroupsource.md).</span></span>

|<span data-ttu-id="cb6e0-130">属性</span><span class="sxs-lookup"><span data-stu-id="cb6e0-130">Property</span></span>|<span data-ttu-id="cb6e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="cb6e0-131">Type</span></span>|<span data-ttu-id="cb6e0-132">Description</span><span class="sxs-lookup"><span data-stu-id="cb6e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6e0-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="cb6e0-133">includedSources</span></span>|<span data-ttu-id="cb6e0-134">sourceType</span><span class="sxs-lookup"><span data-stu-id="cb6e0-134">sourceType</span></span>|<span data-ttu-id="cb6e0-135">指定要包含在此组中的源。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="cb6e0-136">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="cb6e0-137">group@odata 绑定</span><span class="sxs-lookup"><span data-stu-id="cb6e0-137">group@odata.bind</span></span>|<span data-ttu-id="cb6e0-138">String</span><span class="sxs-lookup"><span data-stu-id="cb6e0-138">String</span></span>|<span data-ttu-id="cb6e0-139">组的 ID。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-139">ID of the group.</span></span> <span data-ttu-id="cb6e0-140">若要获取组 ID，请使用 [列表组](../api/group-list.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="cb6e0-141">响应</span><span class="sxs-lookup"><span data-stu-id="cb6e0-141">Response</span></span>

<span data-ttu-id="cb6e0-142">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-142">If successful, this method returns a `201 Created` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb6e0-143">示例</span><span class="sxs-lookup"><span data-stu-id="cb6e0-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb6e0-144">请求</span><span class="sxs-lookup"><span data-stu-id="cb6e0-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```

### <a name="response"></a><span data-ttu-id="cb6e0-145">响应</span><span class="sxs-lookup"><span data-stu-id="cb6e0-145">Response</span></span>

<span data-ttu-id="cb6e0-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb6e0-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site",
  "id": "14202dd90a1f4ccc84929586326c7104",
  "displayName": "SFA Videos",
  "createdDateTime": "2020-03-13T22:38:00.8985662Z",
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Megan Bowen"
      }
  }
}
```
