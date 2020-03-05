---
author: JeremyKelley
description: 使用此 API 检索特定格式的项的内容。
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 03bb884e8dde82c99d0aadfa2a6e925b0d6552a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432654"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="f11c5-103">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="f11c5-103">Download a file in another format</span></span>

<span data-ttu-id="f11c5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f11c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f11c5-105">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="f11c5-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="f11c5-106">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="f11c5-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="f11c5-107">若要下载原始格式的项目，请参阅[下载项内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="f11c5-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f11c5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f11c5-108">Prerequisites</span></span>

<span data-ttu-id="f11c5-109">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f11c5-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="f11c5-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f11c5-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="f11c5-111">查询参数</span><span class="sxs-lookup"><span data-stu-id="f11c5-111">Query parameters</span></span>

| <span data-ttu-id="f11c5-112">参数</span><span class="sxs-lookup"><span data-stu-id="f11c5-112">Parameter</span></span>      | <span data-ttu-id="f11c5-113">类型</span><span class="sxs-lookup"><span data-stu-id="f11c5-113">Type</span></span>  | <span data-ttu-id="f11c5-114">说明</span><span class="sxs-lookup"><span data-stu-id="f11c5-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="f11c5-115">_format_</span><span class="sxs-lookup"><span data-stu-id="f11c5-115">_format_</span></span>  | <span data-ttu-id="f11c5-116">string</span><span class="sxs-lookup"><span data-stu-id="f11c5-116">string</span></span> | <span data-ttu-id="f11c5-117">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="f11c5-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="f11c5-118">以下值对于 **format** 参数有效：</span><span class="sxs-lookup"><span data-stu-id="f11c5-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="f11c5-119">值</span><span class="sxs-lookup"><span data-stu-id="f11c5-119">Value</span></span> | <span data-ttu-id="f11c5-120">说明</span><span class="sxs-lookup"><span data-stu-id="f11c5-120">Description</span></span>                        | <span data-ttu-id="f11c5-121">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="f11c5-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="f11c5-122">glb</span><span class="sxs-lookup"><span data-stu-id="f11c5-122">glb</span></span>   | <span data-ttu-id="f11c5-123">将项转换为 GLB 格式</span><span class="sxs-lookup"><span data-stu-id="f11c5-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="f11c5-124">cool、fbx、obj、ply、stl、3mf</span><span class="sxs-lookup"><span data-stu-id="f11c5-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="f11c5-125">html</span><span class="sxs-lookup"><span data-stu-id="f11c5-125">html</span></span>  | <span data-ttu-id="f11c5-126">将项转换为 HTML 格式</span><span class="sxs-lookup"><span data-stu-id="f11c5-126">Converts the item into HTML format</span></span> | <span data-ttu-id="f11c5-127">eml、md、msg</span><span class="sxs-lookup"><span data-stu-id="f11c5-127">eml, md, msg</span></span>
| <span data-ttu-id="f11c5-128">jpg</span><span class="sxs-lookup"><span data-stu-id="f11c5-128">jpg</span></span>   | <span data-ttu-id="f11c5-129">将项转换为 JPG 格式</span><span class="sxs-lookup"><span data-stu-id="f11c5-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="f11c5-130">3g2、3gp、3gp2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、cool、cpp、cr2、crw、cs、css、csv、cur、dcm、dcm30、dic、dicm、dicom、dng、doc、docx、dwg、eml、epi、eps、epsf、epsi、epub、erf、fbx、fppx、gif、glb、h、hcp、heic、heif、htm、html、ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、movie、mp3、mp4、mp4v、mrw、msg、mts、nef、nrw、numbers、obj、odp、odt、ogg、orf、pages、pano、pdf、pef、php、pict、pl、ply、png、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、ps、ps1、psb、psd、py、raw、rb、rtf、rw1、rw2、sh、sketch、sql、sr2、stl、tif、tiff、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml</span><span class="sxs-lookup"><span data-stu-id="f11c5-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="f11c5-131">pdf</span><span class="sxs-lookup"><span data-stu-id="f11c5-131">pdf</span></span>   | <span data-ttu-id="f11c5-132">将项转换为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="f11c5-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="f11c5-133">doc、docx、epub、eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、pptx、rtf、tif、tiff、xls、xlsm、xlsx</span><span class="sxs-lookup"><span data-stu-id="f11c5-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="f11c5-134">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f11c5-134">Optional request headers</span></span>

| <span data-ttu-id="f11c5-135">名称</span><span class="sxs-lookup"><span data-stu-id="f11c5-135">Name</span></span>            | <span data-ttu-id="f11c5-136">值</span><span class="sxs-lookup"><span data-stu-id="f11c5-136">Value</span></span>   | <span data-ttu-id="f11c5-137">说明</span><span class="sxs-lookup"><span data-stu-id="f11c5-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f11c5-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="f11c5-138">_if-none-match_</span></span> | <span data-ttu-id="f11c5-139">String</span><span class="sxs-lookup"><span data-stu-id="f11c5-139">String</span></span>  | <span data-ttu-id="f11c5-140">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="f11c5-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="f11c5-141">示例</span><span class="sxs-lookup"><span data-stu-id="f11c5-141">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="f11c5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f11c5-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="f11c5-143">C#</span><span class="sxs-lookup"><span data-stu-id="f11c5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f11c5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f11c5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f11c5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f11c5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f11c5-146">响应</span><span class="sxs-lookup"><span data-stu-id="f11c5-146">Response</span></span>

<span data-ttu-id="f11c5-147">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f11c5-147">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="f11c5-148">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="f11c5-148">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="f11c5-149">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="f11c5-149">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="f11c5-150">错误响应</span><span class="sxs-lookup"><span data-stu-id="f11c5-150">Error responses</span></span>

<span data-ttu-id="f11c5-151">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="f11c5-151">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
}
-->
