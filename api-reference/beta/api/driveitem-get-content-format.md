---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 66a81e5b97d31bc3308409fdfc7bb72bb95eb854
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260177"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="c6fd3-102">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="c6fd3-102">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6fd3-103">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="c6fd3-104">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="c6fd3-105">若要下载原始格式的项目，请参阅[下载项内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6fd3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6fd3-106">Prerequisites</span></span>

<span data-ttu-id="c6fd3-107">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="c6fd3-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6fd3-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="c6fd3-109">查询参数</span><span class="sxs-lookup"><span data-stu-id="c6fd3-109">Query parameters</span></span>

| <span data-ttu-id="c6fd3-110">参数</span><span class="sxs-lookup"><span data-stu-id="c6fd3-110">Parameter</span></span>      | <span data-ttu-id="c6fd3-111">类型</span><span class="sxs-lookup"><span data-stu-id="c6fd3-111">Type</span></span>  | <span data-ttu-id="c6fd3-112">说明</span><span class="sxs-lookup"><span data-stu-id="c6fd3-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c6fd3-113">_format_</span><span class="sxs-lookup"><span data-stu-id="c6fd3-113">_format_</span></span>  | <span data-ttu-id="c6fd3-114">string</span><span class="sxs-lookup"><span data-stu-id="c6fd3-114">string</span></span> | <span data-ttu-id="c6fd3-115">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-115">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="c6fd3-116">以下值对于 **format** 参数有效：</span><span class="sxs-lookup"><span data-stu-id="c6fd3-116">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="c6fd3-117">值</span><span class="sxs-lookup"><span data-stu-id="c6fd3-117">Value</span></span> | <span data-ttu-id="c6fd3-118">说明</span><span class="sxs-lookup"><span data-stu-id="c6fd3-118">Description</span></span>                        | <span data-ttu-id="c6fd3-119">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="c6fd3-119">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="c6fd3-120">glb</span><span class="sxs-lookup"><span data-stu-id="c6fd3-120">glb</span></span>   | <span data-ttu-id="c6fd3-121">将项目转换为 GLB 格式</span><span class="sxs-lookup"><span data-stu-id="c6fd3-121">Converts the item into GLB format</span></span>  | <span data-ttu-id="c6fd3-122">酷、fbx、obj、往返和 stl、3mf</span><span class="sxs-lookup"><span data-stu-id="c6fd3-122">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="c6fd3-123">Html</span><span class="sxs-lookup"><span data-stu-id="c6fd3-123">html</span></span>  | <span data-ttu-id="c6fd3-124">将项目转换为 HTML 格式</span><span class="sxs-lookup"><span data-stu-id="c6fd3-124">Converts the item into HTML format</span></span> | <span data-ttu-id="c6fd3-125">.eml、md、msg</span><span class="sxs-lookup"><span data-stu-id="c6fd3-125">eml, md, msg</span></span>
| <span data-ttu-id="c6fd3-126">.jpg</span><span class="sxs-lookup"><span data-stu-id="c6fd3-126">jpg</span></span>   | <span data-ttu-id="c6fd3-127">将项目转换为 JPG 格式</span><span class="sxs-lookup"><span data-stu-id="c6fd3-127">Converts the item into JPG format</span></span>  | <span data-ttu-id="c6fd3-128">3g2、3gp、3gp2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat 和 cbl、bmp、c、、cmd、cr2、、crw、cs、css、csv、当前、dcm、dcm30、home.dic、dicm、dicom、dng、、、、、epi、epsf、epsi、epub、erf、fbx、fppx、glb、gif、、、、heic、heif、htm、html、.ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、电影、mp3、、mp4v、mrw、msg、mts、nef、nrw、、、、、ogg、orf、pages、全景、pdf、pef、php、pict、pl、、.png、、potm、.potx、pps、ppsx、ppsxm、ppt、.pptm、.pptx、ps、ps1、psb、psd、py、raw、rb、rtf、rw1、rw2、sh、素描、sql、、、、xml、sr2、webm、xbm、xcf、、xml、</span><span class="sxs-lookup"><span data-stu-id="c6fd3-128">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="c6fd3-129">pdf</span><span class="sxs-lookup"><span data-stu-id="c6fd3-129">pdf</span></span>   | <span data-ttu-id="c6fd3-130">将项目转换为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="c6fd3-130">Converts the item into PDF format</span></span>  | <span data-ttu-id="c6fd3-131">doc、.docx、epub、.eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、.pptx、rtf、tif、tiff、xls、xlsm、.xlsx</span><span class="sxs-lookup"><span data-stu-id="c6fd3-131">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="c6fd3-132">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c6fd3-132">Optional request headers</span></span>

| <span data-ttu-id="c6fd3-133">名称</span><span class="sxs-lookup"><span data-stu-id="c6fd3-133">Name</span></span>            | <span data-ttu-id="c6fd3-134">值</span><span class="sxs-lookup"><span data-stu-id="c6fd3-134">Value</span></span>   | <span data-ttu-id="c6fd3-135">说明</span><span class="sxs-lookup"><span data-stu-id="c6fd3-135">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c6fd3-136">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="c6fd3-136">_if-none-match_</span></span> | <span data-ttu-id="c6fd3-137">String</span><span class="sxs-lookup"><span data-stu-id="c6fd3-137">String</span></span>  | <span data-ttu-id="c6fd3-138">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-138">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="c6fd3-139">示例</span><span class="sxs-lookup"><span data-stu-id="c6fd3-139">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="c6fd3-140">响应</span><span class="sxs-lookup"><span data-stu-id="c6fd3-140">Response</span></span>

<span data-ttu-id="c6fd3-141">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-141">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="c6fd3-142">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-142">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="c6fd3-143">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-143">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6fd3-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c6fd3-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6fd3-145">C#</span><span class="sxs-lookup"><span data-stu-id="c6fd3-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/convert-item-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6fd3-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6fd3-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/convert-item-content-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6fd3-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="c6fd3-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/convert-item-content-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a><span data-ttu-id="c6fd3-148">错误响应</span><span class="sxs-lookup"><span data-stu-id="c6fd3-148">Error responses</span></span>

<span data-ttu-id="c6fd3-149">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="c6fd3-149">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
