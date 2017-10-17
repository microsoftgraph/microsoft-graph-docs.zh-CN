---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "转换为其他格式"
ms.openlocfilehash: 3031500beaec2d765075abfd925a6333f50368f9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="a0926-102">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="a0926-102">Download a file in another format</span></span>

<span data-ttu-id="a0926-103">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="a0926-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="a0926-104">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="a0926-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="a0926-105">若要以原始格式下载项，请参阅[下载项内容](driveitem_get_content.md)。</span><span class="sxs-lookup"><span data-stu-id="a0926-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0926-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0926-106">Prerequisites</span></span>

<span data-ttu-id="a0926-107">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a0926-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0926-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0926-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a><span data-ttu-id="a0926-109">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a0926-109">Optional request headers</span></span>

| <span data-ttu-id="a0926-110">名称</span><span class="sxs-lookup"><span data-stu-id="a0926-110">Name</span></span>            | <span data-ttu-id="a0926-111">值</span><span class="sxs-lookup"><span data-stu-id="a0926-111">Value</span></span>   | <span data-ttu-id="a0926-112">说明</span><span class="sxs-lookup"><span data-stu-id="a0926-112">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a0926-113">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="a0926-113">_if-none-match_</span></span> | <span data-ttu-id="a0926-114">String</span><span class="sxs-lookup"><span data-stu-id="a0926-114">String</span></span>  | <span data-ttu-id="a0926-115">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="a0926-115">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


### <a name="query-string-parameters"></a><span data-ttu-id="a0926-116">查询字符串参数</span><span class="sxs-lookup"><span data-stu-id="a0926-116">Query string parameters</span></span>

| <span data-ttu-id="a0926-117">名称</span><span class="sxs-lookup"><span data-stu-id="a0926-117">Name</span></span>      | <span data-ttu-id="a0926-118">值</span><span class="sxs-lookup"><span data-stu-id="a0926-118">Value</span></span>  | <span data-ttu-id="a0926-119">说明</span><span class="sxs-lookup"><span data-stu-id="a0926-119">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="a0926-120">_format_</span><span class="sxs-lookup"><span data-stu-id="a0926-120">_format_</span></span>  | <span data-ttu-id="a0926-121">string</span><span class="sxs-lookup"><span data-stu-id="a0926-121">string</span></span> | <span data-ttu-id="a0926-122">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="a0926-122">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="a0926-123">**convert** 参数的可取值如下：</span><span class="sxs-lookup"><span data-stu-id="a0926-123">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="a0926-124">值</span><span class="sxs-lookup"><span data-stu-id="a0926-124">Value</span></span>   | <span data-ttu-id="a0926-125">说明</span><span class="sxs-lookup"><span data-stu-id="a0926-125">Description</span></span>                        | <span data-ttu-id="a0926-126">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="a0926-126">Supported source extensions</span></span> |
|:--------|:-----------------------------------|-----------------------------|
| <span data-ttu-id="a0926-127">**pdf**</span><span class="sxs-lookup"><span data-stu-id="a0926-127">**pdf**</span></span> | <span data-ttu-id="a0926-128">将项转换成 PDF 格式。</span><span class="sxs-lookup"><span data-stu-id="a0926-128">Converts the item into PDF format.</span></span> | <span data-ttu-id="a0926-129">csv、doc、docx、odp、ods、odt、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、rtf、xls、xlsx</span><span class="sxs-lookup"><span data-stu-id="a0926-129">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span> | 

### <a name="example"></a><span data-ttu-id="a0926-130">示例</span><span class="sxs-lookup"><span data-stu-id="a0926-130">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="a0926-131">响应</span><span class="sxs-lookup"><span data-stu-id="a0926-131">Response</span></span>

<span data-ttu-id="a0926-132">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a0926-132">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="a0926-133">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="a0926-133">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="a0926-134">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="a0926-134">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="a0926-135">错误响应</span><span class="sxs-lookup"><span data-stu-id="a0926-135">Error responses</span></span>

<span data-ttu-id="a0926-136">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="a0926-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
