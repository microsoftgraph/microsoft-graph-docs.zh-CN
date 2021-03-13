---
title: 创建 unifiedGroupSource
description: 创建新的 unifiedGroupSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 96e97475c41c983c38f3d8be5c2ec95315427c7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773240"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="eb6bb-103">创建 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="eb6bb-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="eb6bb-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="eb6bb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb6bb-105">创建新的 [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-105">Create a new [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb6bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="eb6bb-106">Permissions</span></span>

<span data-ttu-id="eb6bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb6bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb6bb-109">Permission type</span></span>|<span data-ttu-id="eb6bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb6bb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb6bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb6bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb6bb-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb6bb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="eb6bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb6bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb6bb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-114">Not supported.</span></span>|
|<span data-ttu-id="eb6bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb6bb-115">Application</span></span>|<span data-ttu-id="eb6bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb6bb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb6bb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="eb6bb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb6bb-118">Request headers</span></span>

|<span data-ttu-id="eb6bb-119">名称</span><span class="sxs-lookup"><span data-stu-id="eb6bb-119">Name</span></span>|<span data-ttu-id="eb6bb-120">说明</span><span class="sxs-lookup"><span data-stu-id="eb6bb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eb6bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb6bb-121">Authorization</span></span>|<span data-ttu-id="eb6bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eb6bb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb6bb-124">Content-Type</span></span>|<span data-ttu-id="eb6bb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eb6bb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb6bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb6bb-127">Request body</span></span>

<span data-ttu-id="eb6bb-128">在请求正文中，提供 [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="eb6bb-129">下表显示创建 [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span></span>

|<span data-ttu-id="eb6bb-130">属性</span><span class="sxs-lookup"><span data-stu-id="eb6bb-130">Property</span></span>|<span data-ttu-id="eb6bb-131">类型</span><span class="sxs-lookup"><span data-stu-id="eb6bb-131">Type</span></span>|<span data-ttu-id="eb6bb-132">说明</span><span class="sxs-lookup"><span data-stu-id="eb6bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb6bb-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="eb6bb-133">includedSources</span></span>|<span data-ttu-id="eb6bb-134">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="eb6bb-134">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="eb6bb-135">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="eb6bb-136">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="eb6bb-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="eb6bb-137">group@odata.bind</span></span>|<span data-ttu-id="eb6bb-138">字符串</span><span class="sxs-lookup"><span data-stu-id="eb6bb-138">String</span></span>|<span data-ttu-id="eb6bb-139">组的 ID。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-139">ID of the group.</span></span> <span data-ttu-id="eb6bb-140">若要获取组 ID，请使用 ["列表组"](../api/group-list.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="eb6bb-141">响应</span><span class="sxs-lookup"><span data-stu-id="eb6bb-141">Response</span></span>

<span data-ttu-id="eb6bb-142">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-142">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb6bb-143">示例</span><span class="sxs-lookup"><span data-stu-id="eb6bb-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb6bb-144">请求</span><span class="sxs-lookup"><span data-stu-id="eb6bb-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eb6bb-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6bb-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eb6bb-146">C#</span><span class="sxs-lookup"><span data-stu-id="eb6bb-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb6bb-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb6bb-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb6bb-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb6bb-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedgroupsource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb6bb-149">Java</span><span class="sxs-lookup"><span data-stu-id="eb6bb-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb6bb-150">响应</span><span class="sxs-lookup"><span data-stu-id="eb6bb-150">Response</span></span>

<span data-ttu-id="eb6bb-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb6bb-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
