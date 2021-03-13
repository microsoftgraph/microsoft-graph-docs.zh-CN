---
title: 创建标记
description: 创建新的标记对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 412a0cd1ae4f8c38466a6526a5c84eea670897bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773758"
---
# <a name="create-tag"></a><span data-ttu-id="3ffdb-103">创建标记</span><span class="sxs-lookup"><span data-stu-id="3ffdb-103">Create tag</span></span>

<span data-ttu-id="3ffdb-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3ffdb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ffdb-105">为指定案例创建新标记。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-105">Create a new tag for the specified case.</span></span>  <span data-ttu-id="3ffdb-106">标记在审阅内容时用于审阅集。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-106">The tags are used in review sets while reviewing content.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ffdb-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ffdb-107">Permissions</span></span>

<span data-ttu-id="3ffdb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ffdb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ffdb-110">Permission type</span></span>|<span data-ttu-id="3ffdb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ffdb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ffdb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ffdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ffdb-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffdb-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3ffdb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ffdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ffdb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-115">Not supported.</span></span>|
|<span data-ttu-id="3ffdb-116">Application</span><span class="sxs-lookup"><span data-stu-id="3ffdb-116">Application</span></span>|<span data-ttu-id="3ffdb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ffdb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ffdb-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="request-headers"></a><span data-ttu-id="3ffdb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ffdb-119">Request headers</span></span>

|<span data-ttu-id="3ffdb-120">名称</span><span class="sxs-lookup"><span data-stu-id="3ffdb-120">Name</span></span>|<span data-ttu-id="3ffdb-121">说明</span><span class="sxs-lookup"><span data-stu-id="3ffdb-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3ffdb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ffdb-122">Authorization</span></span>|<span data-ttu-id="3ffdb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3ffdb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ffdb-125">Content-Type</span></span>|<span data-ttu-id="3ffdb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3ffdb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ffdb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ffdb-128">Request body</span></span>

<span data-ttu-id="3ffdb-129">在请求正文中，提供 tag 对象的 JSON [表示](../resources/ediscovery-tag.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-129">In the request body, supply a JSON representation of the [tag](../resources/ediscovery-tag.md) object.</span></span>

<span data-ttu-id="3ffdb-130">下表显示创建 标记时所需的 [属性](../resources/ediscovery-tag.md)。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-130">The following table shows the properties that are required when you create the [tag](../resources/ediscovery-tag.md).</span></span>

|<span data-ttu-id="3ffdb-131">属性</span><span class="sxs-lookup"><span data-stu-id="3ffdb-131">Property</span></span>|<span data-ttu-id="3ffdb-132">类型</span><span class="sxs-lookup"><span data-stu-id="3ffdb-132">Type</span></span>|<span data-ttu-id="3ffdb-133">说明</span><span class="sxs-lookup"><span data-stu-id="3ffdb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ffdb-134">childSelectability</span><span class="sxs-lookup"><span data-stu-id="3ffdb-134">childSelectability</span></span>|[<span data-ttu-id="3ffdb-135">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="3ffdb-135">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="3ffdb-136">指示是否可以将单个或多个子标记与文档关联。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-136">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="3ffdb-137">可取值为：`One`、`Many`。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-137">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="3ffdb-138">此值控制 UX 是作为复选框还是单选按钮组显示标记。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-138">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span> <span data-ttu-id="3ffdb-139">必需。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-139">Required.</span></span>|
|<span data-ttu-id="3ffdb-140">displayName</span><span class="sxs-lookup"><span data-stu-id="3ffdb-140">displayName</span></span>|<span data-ttu-id="3ffdb-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3ffdb-141">String</span></span>|<span data-ttu-id="3ffdb-142">标记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-142">Display name of the tag.</span></span> <span data-ttu-id="3ffdb-143">必需。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-143">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="3ffdb-144">响应</span><span class="sxs-lookup"><span data-stu-id="3ffdb-144">Response</span></span>

<span data-ttu-id="3ffdb-145">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-145">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ffdb-146">示例</span><span class="sxs-lookup"><span data-stu-id="3ffdb-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ffdb-147">请求</span><span class="sxs-lookup"><span data-stu-id="3ffdb-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3ffdb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ffdb-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tag_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
Content-Type: application/json
Content-length: 235

{
  "displayName":"Privileged",
  "description":"The document is privileged",
  "parent@odata.bind":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}
```
# <a name="c"></a>[<span data-ttu-id="3ffdb-149">C#</span><span class="sxs-lookup"><span data-stu-id="3ffdb-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tag-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ffdb-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ffdb-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tag-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ffdb-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ffdb-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tag-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ffdb-152">Java</span><span class="sxs-lookup"><span data-stu-id="3ffdb-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tag-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ffdb-153">响应</span><span class="sxs-lookup"><span data-stu-id="3ffdb-153">Response</span></span>

<span data-ttu-id="3ffdb-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ffdb-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/$entity",
    "displayName": "Privileged",
    "description": "The document is privileged",
    "lastModifiedDateTime": "2021-01-12T01:01:09.0419153Z",
    "childSelectability": "One",
    "id": "0825ef81ade74095a3b3154a3c434c3e",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
