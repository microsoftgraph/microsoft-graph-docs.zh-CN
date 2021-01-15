---
title: 创建 unifiedGroupSource
description: 创建新的 unifiedGroupSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 61e7ff3aef7c4a94b0a0efcbc0f012b7eda0b604
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872546"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="58fd2-103">创建 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="58fd2-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="58fd2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58fd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58fd2-105">创建新的 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58fd2-105">Create a new [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58fd2-106">权限</span><span class="sxs-lookup"><span data-stu-id="58fd2-106">Permissions</span></span>

<span data-ttu-id="58fd2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58fd2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58fd2-109">Permission type</span></span>|<span data-ttu-id="58fd2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58fd2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58fd2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58fd2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58fd2-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="58fd2-112">User.Read</span></span>|
|<span data-ttu-id="58fd2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58fd2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58fd2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58fd2-114">Not supported.</span></span>|
|<span data-ttu-id="58fd2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58fd2-115">Application</span></span>|<span data-ttu-id="58fd2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58fd2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58fd2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58fd2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="58fd2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="58fd2-118">Request headers</span></span>

|<span data-ttu-id="58fd2-119">名称</span><span class="sxs-lookup"><span data-stu-id="58fd2-119">Name</span></span>|<span data-ttu-id="58fd2-120">说明</span><span class="sxs-lookup"><span data-stu-id="58fd2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="58fd2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58fd2-121">Authorization</span></span>|<span data-ttu-id="58fd2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58fd2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="58fd2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58fd2-124">Content-Type</span></span>|<span data-ttu-id="58fd2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="58fd2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58fd2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58fd2-127">Request body</span></span>

<span data-ttu-id="58fd2-128">在请求正文中，提供 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58fd2-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="58fd2-129">下表显示创建 [unifiedGroupSource](../resources/unifiedgroupsource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58fd2-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/unifiedgroupsource.md).</span></span>

|<span data-ttu-id="58fd2-130">属性</span><span class="sxs-lookup"><span data-stu-id="58fd2-130">Property</span></span>|<span data-ttu-id="58fd2-131">类型</span><span class="sxs-lookup"><span data-stu-id="58fd2-131">Type</span></span>|<span data-ttu-id="58fd2-132">Description</span><span class="sxs-lookup"><span data-stu-id="58fd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fd2-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="58fd2-133">includedSources</span></span>|<span data-ttu-id="58fd2-134">sourceType</span><span class="sxs-lookup"><span data-stu-id="58fd2-134">sourceType</span></span>|<span data-ttu-id="58fd2-135">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="58fd2-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="58fd2-136">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="58fd2-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="58fd2-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="58fd2-137">group@odata.bind</span></span>|<span data-ttu-id="58fd2-138">String</span><span class="sxs-lookup"><span data-stu-id="58fd2-138">String</span></span>|<span data-ttu-id="58fd2-139">组的 ID。</span><span class="sxs-lookup"><span data-stu-id="58fd2-139">ID of the group.</span></span> <span data-ttu-id="58fd2-140">若要获取组 ID，请使用 ["列表组"](../api/group-list.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="58fd2-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="58fd2-141">响应</span><span class="sxs-lookup"><span data-stu-id="58fd2-141">Response</span></span>

<span data-ttu-id="58fd2-142">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [unifiedGroupSource](../resources/unifiedgroupsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58fd2-142">If successful, this method returns a `201 Created` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58fd2-143">示例</span><span class="sxs-lookup"><span data-stu-id="58fd2-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58fd2-144">请求</span><span class="sxs-lookup"><span data-stu-id="58fd2-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="58fd2-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="58fd2-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="58fd2-146">C#</span><span class="sxs-lookup"><span data-stu-id="58fd2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58fd2-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58fd2-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58fd2-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58fd2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedgroupsource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58fd2-149">Java</span><span class="sxs-lookup"><span data-stu-id="58fd2-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58fd2-150">响应</span><span class="sxs-lookup"><span data-stu-id="58fd2-150">Response</span></span>

<span data-ttu-id="58fd2-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="58fd2-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
