---
author: swapnil1993
title: contentType：copyToDefaultContentLocation
description: 将文件复制到内容类型中的默认内容位置。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: afe4a5aebe4e19dd3957e0be0cca334a33035981
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201986"
---
# <a name="contenttype-copytodefaultcontentlocation"></a><span data-ttu-id="6e08a-103">contentType：copyToDefaultContentLocation</span><span class="sxs-lookup"><span data-stu-id="6e08a-103">contentType: copyToDefaultContentLocation</span></span>
<span data-ttu-id="6e08a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e08a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6e08a-105">将文件复制到内容类型 中的默认 [内容位置][contentType]。</span><span class="sxs-lookup"><span data-stu-id="6e08a-105">Copy a file to a default content location in a [content type][contentType].</span></span> <span data-ttu-id="6e08a-106">然后，可以通过 POST 操作将该文件添加为默认文件或模板。</span><span class="sxs-lookup"><span data-stu-id="6e08a-106">The file can then be added as a default file or template via a POST operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e08a-107">权限</span><span class="sxs-lookup"><span data-stu-id="6e08a-107">Permissions</span></span>  

<span data-ttu-id="6e08a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6e08a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="6e08a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e08a-110">Permission type</span></span> | <span data-ttu-id="6e08a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e08a-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e08a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e08a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e08a-113">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6e08a-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="6e08a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e08a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e08a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e08a-115">Not supported.</span></span> |
|<span data-ttu-id="6e08a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e08a-116">Application</span></span> | <span data-ttu-id="6e08a-117">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6e08a-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="6e08a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e08a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /sites/id/contentTypes/id/copyToDefaultContentLocation 
```

## <a name="request-headers"></a><span data-ttu-id="6e08a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e08a-119">Request headers</span></span>
|<span data-ttu-id="6e08a-120">名称</span><span class="sxs-lookup"><span data-stu-id="6e08a-120">Name</span></span>|<span data-ttu-id="6e08a-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e08a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e08a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e08a-122">Authorization</span></span>|<span data-ttu-id="6e08a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e08a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6e08a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e08a-125">Content-Type</span></span>|<span data-ttu-id="6e08a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6e08a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e08a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e08a-128">Request body</span></span>
<span data-ttu-id="6e08a-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e08a-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="6e08a-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6e08a-130">The following table shows the parameters that can be used with this action.</span></span>


|<span data-ttu-id="6e08a-131">参数</span><span class="sxs-lookup"><span data-stu-id="6e08a-131">Parameter</span></span>|<span data-ttu-id="6e08a-132">类型</span><span class="sxs-lookup"><span data-stu-id="6e08a-132">Type</span></span>|<span data-ttu-id="6e08a-133">说明</span><span class="sxs-lookup"><span data-stu-id="6e08a-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="6e08a-134">sourceFile</span><span class="sxs-lookup"><span data-stu-id="6e08a-134">sourceFile</span></span>| [<span data-ttu-id="6e08a-135">itemReference</span><span class="sxs-lookup"><span data-stu-id="6e08a-135">itemReference</span></span>](../resources/itemreference.md) |<span data-ttu-id="6e08a-136">有关需要复制到默认内容位置的源文件的元数据。</span><span class="sxs-lookup"><span data-stu-id="6e08a-136">Metadata about the source file that needs to be copied to the default content location.</span></span> <span data-ttu-id="6e08a-137">必需。</span><span class="sxs-lookup"><span data-stu-id="6e08a-137">Required.</span></span>|
|<span data-ttu-id="6e08a-138">destinationFileName</span><span class="sxs-lookup"><span data-stu-id="6e08a-138">destinationFileName</span></span>| <span data-ttu-id="6e08a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="6e08a-139">string</span></span> |<span data-ttu-id="6e08a-140">目标文件名。</span><span class="sxs-lookup"><span data-stu-id="6e08a-140">Destination filename.</span></span> 

## <a name="response"></a><span data-ttu-id="6e08a-141">响应</span><span class="sxs-lookup"><span data-stu-id="6e08a-141">Response</span></span>


<span data-ttu-id="6e08a-142">如果成功，此调用将返回 `204 No Content` 响应。</span><span class="sxs-lookup"><span data-stu-id="6e08a-142">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="6e08a-143">示例</span><span class="sxs-lookup"><span data-stu-id="6e08a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e08a-144">请求</span><span class="sxs-lookup"><span data-stu-id="6e08a-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6e08a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e08a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
   "sourceFile":{
      "sharepointIds":{
         "listId":"e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
         "listItemId":"2"
      }
   },
   "destinationFileName":"newname.txt"
}
```
# <a name="c"></a>[<span data-ttu-id="6e08a-146">C#</span><span class="sxs-lookup"><span data-stu-id="6e08a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-copytodefaultcontentlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e08a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e08a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-copytodefaultcontentlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e08a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e08a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-copytodefaultcontentlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e08a-149">Java</span><span class="sxs-lookup"><span data-stu-id="6e08a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-copytodefaultcontentlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="6e08a-150">响应</span><span class="sxs-lookup"><span data-stu-id="6e08a-150">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
