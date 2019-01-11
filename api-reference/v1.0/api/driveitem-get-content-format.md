---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Priority
ms.openlocfilehash: 86210d4364f771d2bf6f8d0ebbdd70634521cd67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812409"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="b345d-102">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="b345d-102">Download a file in another format</span></span>

<span data-ttu-id="b345d-103">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="b345d-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="b345d-104">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="b345d-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="b345d-105">若要下载其原始格式中的项，请参阅[下载项目的内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="b345d-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b345d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b345d-106">Prerequisites</span></span>

<span data-ttu-id="b345d-107">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b345d-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="b345d-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b345d-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="b345d-109">查询参数</span><span class="sxs-lookup"><span data-stu-id="b345d-109">Query parameters</span></span>

| <span data-ttu-id="b345d-110">参数</span><span class="sxs-lookup"><span data-stu-id="b345d-110">Parameter</span></span>      | <span data-ttu-id="b345d-111">类型</span><span class="sxs-lookup"><span data-stu-id="b345d-111">Type</span></span>  | <span data-ttu-id="b345d-112">说明</span><span class="sxs-lookup"><span data-stu-id="b345d-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="b345d-113">_format_</span><span class="sxs-lookup"><span data-stu-id="b345d-113">_format_</span></span>  | <span data-ttu-id="b345d-114">string</span><span class="sxs-lookup"><span data-stu-id="b345d-114">string</span></span> | <span data-ttu-id="b345d-115">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="b345d-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="b345d-116">格式选项</span><span class="sxs-lookup"><span data-stu-id="b345d-116">Format options</span></span>

<span data-ttu-id="b345d-117">以下是**format**参数的有效值：</span><span class="sxs-lookup"><span data-stu-id="b345d-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="b345d-118">格式值</span><span class="sxs-lookup"><span data-stu-id="b345d-118">Format value</span></span> | <span data-ttu-id="b345d-119">说明</span><span class="sxs-lookup"><span data-stu-id="b345d-119">Description</span></span>                        | <span data-ttu-id="b345d-120">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="b345d-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="b345d-121">pdf</span><span class="sxs-lookup"><span data-stu-id="b345d-121">pdf</span></span>          | <span data-ttu-id="b345d-122">将项转换成 PDF 格式。</span><span class="sxs-lookup"><span data-stu-id="b345d-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="b345d-123">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="b345d-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="b345d-124">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b345d-124">Optional request headers</span></span>

| <span data-ttu-id="b345d-125">名称</span><span class="sxs-lookup"><span data-stu-id="b345d-125">Name</span></span>            | <span data-ttu-id="b345d-126">值</span><span class="sxs-lookup"><span data-stu-id="b345d-126">Value</span></span>   | <span data-ttu-id="b345d-127">说明</span><span class="sxs-lookup"><span data-stu-id="b345d-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b345d-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="b345d-128">_if-none-match_</span></span> | <span data-ttu-id="b345d-129">String</span><span class="sxs-lookup"><span data-stu-id="b345d-129">String</span></span>  | <span data-ttu-id="b345d-130">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="b345d-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="b345d-131">示例</span><span class="sxs-lookup"><span data-stu-id="b345d-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="b345d-132">响应</span><span class="sxs-lookup"><span data-stu-id="b345d-132">Response</span></span>

<span data-ttu-id="b345d-133">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b345d-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="b345d-134">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="b345d-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="b345d-135">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="b345d-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="b345d-136">错误响应</span><span class="sxs-lookup"><span data-stu-id="b345d-136">Error responses</span></span>

<span data-ttu-id="b345d-137">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="b345d-137">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
