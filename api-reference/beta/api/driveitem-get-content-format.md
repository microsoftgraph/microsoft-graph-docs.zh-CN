---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Normal
ms.openlocfilehash: d27420153a295eac9d3f880910d63bd701525427
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887435"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="d4a4e-102">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="d4a4e-102">Download a file in another format</span></span>

> <span data-ttu-id="d4a4e-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4a4e-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4a4e-105">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="d4a4e-106">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="d4a4e-107">若要下载其原始格式中的项，请参阅[下载项目的内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4a4e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4a4e-108">Prerequisites</span></span>

<span data-ttu-id="d4a4e-109">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4a4e-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4a4e-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="d4a4e-111">查询参数</span><span class="sxs-lookup"><span data-stu-id="d4a4e-111">Query parameters</span></span>

| <span data-ttu-id="d4a4e-112">参数</span><span class="sxs-lookup"><span data-stu-id="d4a4e-112">Parameter</span></span>      | <span data-ttu-id="d4a4e-113">类型</span><span class="sxs-lookup"><span data-stu-id="d4a4e-113">Type</span></span>  | <span data-ttu-id="d4a4e-114">说明</span><span class="sxs-lookup"><span data-stu-id="d4a4e-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="d4a4e-115">_format_</span><span class="sxs-lookup"><span data-stu-id="d4a4e-115">_format_</span></span>  | <span data-ttu-id="d4a4e-116">string</span><span class="sxs-lookup"><span data-stu-id="d4a4e-116">string</span></span> | <span data-ttu-id="d4a4e-117">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="d4a4e-118">以下是**format**参数的有效值：</span><span class="sxs-lookup"><span data-stu-id="d4a4e-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="d4a4e-119">值</span><span class="sxs-lookup"><span data-stu-id="d4a4e-119">Value</span></span> | <span data-ttu-id="d4a4e-120">说明</span><span class="sxs-lookup"><span data-stu-id="d4a4e-120">Description</span></span>                        | <span data-ttu-id="d4a4e-121">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="d4a4e-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="d4a4e-122">glb</span><span class="sxs-lookup"><span data-stu-id="d4a4e-122">glb</span></span>   | <span data-ttu-id="d4a4e-123">将项目转换成 GLB 格式</span><span class="sxs-lookup"><span data-stu-id="d4a4e-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="d4a4e-124">不错，fbx、 obj、 往返流、 stl 3mf</span><span class="sxs-lookup"><span data-stu-id="d4a4e-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="d4a4e-125">html</span><span class="sxs-lookup"><span data-stu-id="d4a4e-125">html</span></span>  | <span data-ttu-id="d4a4e-126">将项目转换为 HTML 格式</span><span class="sxs-lookup"><span data-stu-id="d4a4e-126">Converts the item into HTML format</span></span> | <span data-ttu-id="d4a4e-127">eml md、 msg</span><span class="sxs-lookup"><span data-stu-id="d4a4e-127">eml, md, msg</span></span>
| <span data-ttu-id="d4a4e-128">jpg</span><span class="sxs-lookup"><span data-stu-id="d4a4e-128">jpg</span></span>   | <span data-ttu-id="d4a4e-129">将项目转换为 JPG 格式</span><span class="sxs-lookup"><span data-stu-id="d4a4e-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="d4a4e-130">3g 2、 3gp、 3gp2、 3gpp、 3mf、 ai、 arw、 asf、 avi、 营业活动报表、 bash、 bat、 bmp、 c、 cbl、 cmd、 不错、 cpp、 cr2、 crw、 cs、 css、 csv、 当前、 dcm、 dcm30、 词典、 dicm、 dicom、 dng、 doc、 docx、 dwg、 eml、 epi、 eps、 epsf、 epsi、 epub、 erf、 fbx、 fppx、 gif、 glb、 h、 hcpheic，heif，htm，html、 ico、 图标、 java、 jfif、 jpeg、 jpg、 js、 json、 密钥、 日志、 m2ts、 m4a、 m4v、 减价、 md、 mef、 mov、 影片、 mp3、 mp4 （英文）、 mp4v、 mrw、 msg、 mts、 nef、 nrw、 数字、 obj、 odp、 odt、 ogg、 orf、 页面、 全景、 pdf、 pef、 php、 pict、 pl、 往返流、 png、 potpotm，potx，pps，ppsx，ppsxm，ppt、 pptm、 pptx、 ps、 ps1、 psb、 psd、 上一年度，原始，rb、 rtf、 rw1、 rw2，sh，素描，sql、 sr2、 stl、 tif、 tiff、 ts、 txt、 vb、 webm、 wma、 wmv (英文)、 xaml、 xbm、 xcf、 xd、 xml、 xpm、 yaml、 yml</span><span class="sxs-lookup"><span data-stu-id="d4a4e-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="d4a4e-131">pdf</span><span class="sxs-lookup"><span data-stu-id="d4a4e-131">pdf</span></span>   | <span data-ttu-id="d4a4e-132">将项目转换为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="d4a4e-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="d4a4e-133">doc、 docx、 epub、 eml、 htm、 html、 md、 msg、 odp、 ods、 odt、 pps、 ppsx、 ppt、 pptx、 rtf、 tif、 tiff、 xls、 xlsm、 xlsx</span><span class="sxs-lookup"><span data-stu-id="d4a4e-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="d4a4e-134">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d4a4e-134">Optional request headers</span></span>

| <span data-ttu-id="d4a4e-135">名称</span><span class="sxs-lookup"><span data-stu-id="d4a4e-135">Name</span></span>            | <span data-ttu-id="d4a4e-136">值</span><span class="sxs-lookup"><span data-stu-id="d4a4e-136">Value</span></span>   | <span data-ttu-id="d4a4e-137">说明</span><span class="sxs-lookup"><span data-stu-id="d4a4e-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d4a4e-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="d4a4e-138">_if-none-match_</span></span> | <span data-ttu-id="d4a4e-139">String</span><span class="sxs-lookup"><span data-stu-id="d4a4e-139">String</span></span>  | <span data-ttu-id="d4a4e-140">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="d4a4e-141">示例</span><span class="sxs-lookup"><span data-stu-id="d4a4e-141">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="d4a4e-142">响应</span><span class="sxs-lookup"><span data-stu-id="d4a4e-142">Response</span></span>

<span data-ttu-id="d4a4e-143">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-143">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="d4a4e-144">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-144">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="d4a4e-145">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-145">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="d4a4e-146">错误响应</span><span class="sxs-lookup"><span data-stu-id="d4a4e-146">Error responses</span></span>

<span data-ttu-id="d4a4e-147">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="d4a4e-147">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
