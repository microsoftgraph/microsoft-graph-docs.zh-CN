---
title: 创建 unifiedGroupSource
description: 创建新的 unifiedGroupSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1c2ffe7ca2739b728cd15561266ee583e98b320e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446056"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="be4a3-103">创建 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="be4a3-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="be4a3-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="be4a3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be4a3-105">创建新的 [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be4a3-105">Create a new [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be4a3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="be4a3-106">Permissions</span></span>

<span data-ttu-id="be4a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be4a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be4a3-109">Permission type</span></span>|<span data-ttu-id="be4a3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be4a3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be4a3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be4a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be4a3-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4a3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="be4a3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be4a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be4a3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be4a3-114">Not supported.</span></span>|
|<span data-ttu-id="be4a3-115">Application</span><span class="sxs-lookup"><span data-stu-id="be4a3-115">Application</span></span>|<span data-ttu-id="be4a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be4a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be4a3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be4a3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="be4a3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="be4a3-118">Request headers</span></span>

|<span data-ttu-id="be4a3-119">名称</span><span class="sxs-lookup"><span data-stu-id="be4a3-119">Name</span></span>|<span data-ttu-id="be4a3-120">说明</span><span class="sxs-lookup"><span data-stu-id="be4a3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="be4a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be4a3-121">Authorization</span></span>|<span data-ttu-id="be4a3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be4a3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="be4a3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be4a3-124">Content-Type</span></span>|<span data-ttu-id="be4a3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="be4a3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="be4a3-127">Request body</span></span>

<span data-ttu-id="be4a3-128">在请求正文中，提供 [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be4a3-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="be4a3-129">下表显示创建 [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be4a3-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span></span>

|<span data-ttu-id="be4a3-130">属性</span><span class="sxs-lookup"><span data-stu-id="be4a3-130">Property</span></span>|<span data-ttu-id="be4a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="be4a3-131">Type</span></span>|<span data-ttu-id="be4a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="be4a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4a3-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="be4a3-133">includedSources</span></span>|<span data-ttu-id="be4a3-134">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="be4a3-134">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="be4a3-135">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="be4a3-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="be4a3-136">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="be4a3-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="be4a3-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="be4a3-137">group@odata.bind</span></span>|<span data-ttu-id="be4a3-138">String</span><span class="sxs-lookup"><span data-stu-id="be4a3-138">String</span></span>|<span data-ttu-id="be4a3-139">组的 ID。</span><span class="sxs-lookup"><span data-stu-id="be4a3-139">ID of the group.</span></span> <span data-ttu-id="be4a3-140">若要获取组 ID，请使用 ["列表组"](../api/group-list.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="be4a3-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="be4a3-141">响应</span><span class="sxs-lookup"><span data-stu-id="be4a3-141">Response</span></span>

<span data-ttu-id="be4a3-142">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be4a3-142">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be4a3-143">示例</span><span class="sxs-lookup"><span data-stu-id="be4a3-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be4a3-144">请求</span><span class="sxs-lookup"><span data-stu-id="be4a3-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```

### <a name="response"></a><span data-ttu-id="be4a3-145">响应</span><span class="sxs-lookup"><span data-stu-id="be4a3-145">Response</span></span>

<span data-ttu-id="be4a3-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be4a3-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource"
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
