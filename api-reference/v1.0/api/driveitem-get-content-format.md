---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Priority
ms.prod: sharepoint
description: 使用此 API 检索特定格式的项的内容。
doc_type: apiPageType
ms.openlocfilehash: ca39ea1bb0707093b782a7068f965cb7716eb381
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009798"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="59a4e-103">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="59a4e-103">Download a file in another format</span></span>

<span data-ttu-id="59a4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59a4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59a4e-105">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="59a4e-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="59a4e-106">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="59a4e-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="59a4e-107">若要下载原始格式的项目，请参阅[下载项内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="59a4e-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59a4e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="59a4e-108">Prerequisites</span></span>

<span data-ttu-id="59a4e-109">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="59a4e-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="59a4e-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59a4e-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="59a4e-111">查询参数</span><span class="sxs-lookup"><span data-stu-id="59a4e-111">Query parameters</span></span>

| <span data-ttu-id="59a4e-112">参数</span><span class="sxs-lookup"><span data-stu-id="59a4e-112">Parameter</span></span>      | <span data-ttu-id="59a4e-113">类型</span><span class="sxs-lookup"><span data-stu-id="59a4e-113">Type</span></span>  | <span data-ttu-id="59a4e-114">说明</span><span class="sxs-lookup"><span data-stu-id="59a4e-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="59a4e-115">_format_</span><span class="sxs-lookup"><span data-stu-id="59a4e-115">_format_</span></span>  | <span data-ttu-id="59a4e-116">string</span><span class="sxs-lookup"><span data-stu-id="59a4e-116">string</span></span> | <span data-ttu-id="59a4e-117">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="59a4e-117">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="59a4e-118">格式选项</span><span class="sxs-lookup"><span data-stu-id="59a4e-118">Format options</span></span>

<span data-ttu-id="59a4e-119">以下值对于 **format** 参数有效：</span><span class="sxs-lookup"><span data-stu-id="59a4e-119">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="59a4e-120">格式值</span><span class="sxs-lookup"><span data-stu-id="59a4e-120">Format value</span></span> | <span data-ttu-id="59a4e-121">说明</span><span class="sxs-lookup"><span data-stu-id="59a4e-121">Description</span></span>                        | <span data-ttu-id="59a4e-122">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="59a4e-122">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="59a4e-123">pdf</span><span class="sxs-lookup"><span data-stu-id="59a4e-123">pdf</span></span>          | <span data-ttu-id="59a4e-124">将项转换成 PDF 格式。</span><span class="sxs-lookup"><span data-stu-id="59a4e-124">Converts the item into PDF format.</span></span> | <span data-ttu-id="59a4e-125">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="59a4e-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="59a4e-126">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="59a4e-126">Optional request headers</span></span>

| <span data-ttu-id="59a4e-127">名称</span><span class="sxs-lookup"><span data-stu-id="59a4e-127">Name</span></span>            | <span data-ttu-id="59a4e-128">值</span><span class="sxs-lookup"><span data-stu-id="59a4e-128">Value</span></span>   | <span data-ttu-id="59a4e-129">说明</span><span class="sxs-lookup"><span data-stu-id="59a4e-129">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="59a4e-130">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="59a4e-130">_if-none-match_</span></span> | <span data-ttu-id="59a4e-131">String</span><span class="sxs-lookup"><span data-stu-id="59a4e-131">String</span></span>  | <span data-ttu-id="59a4e-132">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="59a4e-132">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="59a4e-133">示例</span><span class="sxs-lookup"><span data-stu-id="59a4e-133">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="59a4e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="59a4e-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="59a4e-135">C#</span><span class="sxs-lookup"><span data-stu-id="59a4e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59a4e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59a4e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59a4e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59a4e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59a4e-138">Java</span><span class="sxs-lookup"><span data-stu-id="59a4e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="59a4e-139">响应</span><span class="sxs-lookup"><span data-stu-id="59a4e-139">Response</span></span>

<span data-ttu-id="59a4e-140">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="59a4e-140">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="59a4e-141">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="59a4e-141">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="59a4e-142">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="59a4e-142">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="59a4e-143">错误响应</span><span class="sxs-lookup"><span data-stu-id="59a4e-143">Error responses</span></span>

<span data-ttu-id="59a4e-144">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="59a4e-144">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
} -->

