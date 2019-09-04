---
author: JeremyKelley
description: 使用此 API 检索特定格式的项的内容。
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 914f6b5d847c6b8af5439c4b5e83f3d9f281aa65
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719379"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="ce6e5-103">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="ce6e5-103">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce6e5-104">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-104">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="ce6e5-105">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-105">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="ce6e5-106">若要下载原始格式的项目，请参阅[下载项内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-106">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce6e5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce6e5-107">Prerequisites</span></span>

<span data-ttu-id="ce6e5-108">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-108">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="ce6e5-109">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce6e5-109">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="ce6e5-110">查询参数</span><span class="sxs-lookup"><span data-stu-id="ce6e5-110">Query parameters</span></span>

| <span data-ttu-id="ce6e5-111">参数</span><span class="sxs-lookup"><span data-stu-id="ce6e5-111">Parameter</span></span>      | <span data-ttu-id="ce6e5-112">类型</span><span class="sxs-lookup"><span data-stu-id="ce6e5-112">Type</span></span>  | <span data-ttu-id="ce6e5-113">说明</span><span class="sxs-lookup"><span data-stu-id="ce6e5-113">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="ce6e5-114">_format_</span><span class="sxs-lookup"><span data-stu-id="ce6e5-114">_format_</span></span>  | <span data-ttu-id="ce6e5-115">string</span><span class="sxs-lookup"><span data-stu-id="ce6e5-115">string</span></span> | <span data-ttu-id="ce6e5-116">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-116">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="ce6e5-117">以下值对于 **format** 参数有效：</span><span class="sxs-lookup"><span data-stu-id="ce6e5-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="ce6e5-118">值</span><span class="sxs-lookup"><span data-stu-id="ce6e5-118">Value</span></span> | <span data-ttu-id="ce6e5-119">说明</span><span class="sxs-lookup"><span data-stu-id="ce6e5-119">Description</span></span>                        | <span data-ttu-id="ce6e5-120">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="ce6e5-120">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="ce6e5-121">glb</span><span class="sxs-lookup"><span data-stu-id="ce6e5-121">glb</span></span>   | <span data-ttu-id="ce6e5-122">将项目转换为 GLB 格式</span><span class="sxs-lookup"><span data-stu-id="ce6e5-122">Converts the item into GLB format</span></span>  | <span data-ttu-id="ce6e5-123">酷、fbx、obj、往返和 stl、3mf</span><span class="sxs-lookup"><span data-stu-id="ce6e5-123">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="ce6e5-124">Html</span><span class="sxs-lookup"><span data-stu-id="ce6e5-124">html</span></span>  | <span data-ttu-id="ce6e5-125">将项目转换为 HTML 格式</span><span class="sxs-lookup"><span data-stu-id="ce6e5-125">Converts the item into HTML format</span></span> | <span data-ttu-id="ce6e5-126">.eml、md、msg</span><span class="sxs-lookup"><span data-stu-id="ce6e5-126">eml, md, msg</span></span>
| <span data-ttu-id="ce6e5-127">.jpg</span><span class="sxs-lookup"><span data-stu-id="ce6e5-127">jpg</span></span>   | <span data-ttu-id="ce6e5-128">将项目转换为 JPG 格式</span><span class="sxs-lookup"><span data-stu-id="ce6e5-128">Converts the item into JPG format</span></span>  | <span data-ttu-id="ce6e5-129">3g2、3gp、3gp2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat 和 cbl、bmp、c、、cmd、cr2、、crw、cs、css、csv、当前、dcm、dcm30、home.dic、dicm、dicom、dng、、、、、epi、epsf、epsi、epub、erf、fbx、fppx、glb、gif、、、、heic、heif、htm、html、.ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、电影、mp3、、mp4v、mrw、msg、mts、nef、nrw、、、、、ogg、orf、pages、全景、pdf、pef、php、pict、pl、、.png、、potm、.potx、pps、ppsx、ppsxm、ppt、.pptm、.pptx、ps、ps1、psb、psd、py、raw、rb、rtf、rw1、rw2、sh、素描、sql、、、、xml、sr2、webm、xbm、xcf、、xml、</span><span class="sxs-lookup"><span data-stu-id="ce6e5-129">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="ce6e5-130">pdf</span><span class="sxs-lookup"><span data-stu-id="ce6e5-130">pdf</span></span>   | <span data-ttu-id="ce6e5-131">将项目转换为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="ce6e5-131">Converts the item into PDF format</span></span>  | <span data-ttu-id="ce6e5-132">doc、.docx、epub、.eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、.pptx、rtf、tif、tiff、xls、xlsm、.xlsx</span><span class="sxs-lookup"><span data-stu-id="ce6e5-132">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="ce6e5-133">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ce6e5-133">Optional request headers</span></span>

| <span data-ttu-id="ce6e5-134">名称</span><span class="sxs-lookup"><span data-stu-id="ce6e5-134">Name</span></span>            | <span data-ttu-id="ce6e5-135">值</span><span class="sxs-lookup"><span data-stu-id="ce6e5-135">Value</span></span>   | <span data-ttu-id="ce6e5-136">说明</span><span class="sxs-lookup"><span data-stu-id="ce6e5-136">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ce6e5-137">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="ce6e5-137">_if-none-match_</span></span> | <span data-ttu-id="ce6e5-138">String</span><span class="sxs-lookup"><span data-stu-id="ce6e5-138">String</span></span>  | <span data-ttu-id="ce6e5-139">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="ce6e5-140">示例</span><span class="sxs-lookup"><span data-stu-id="ce6e5-140">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ce6e5-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ce6e5-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce6e5-142">C#</span><span class="sxs-lookup"><span data-stu-id="ce6e5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce6e5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce6e5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce6e5-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="ce6e5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ce6e5-145">响应</span><span class="sxs-lookup"><span data-stu-id="ce6e5-145">Response</span></span>

<span data-ttu-id="ce6e5-146">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-146">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="ce6e5-147">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-147">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="ce6e5-148">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-148">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="ce6e5-149">错误响应</span><span class="sxs-lookup"><span data-stu-id="ce6e5-149">Error responses</span></span>

<span data-ttu-id="ce6e5-150">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="ce6e5-150">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
