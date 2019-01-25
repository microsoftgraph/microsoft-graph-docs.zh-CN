---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8d65b7604c2ec17d4225c9cb887cbbfad2223009
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526303"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="d119e-102">以其他格式下载文件</span><span class="sxs-lookup"><span data-stu-id="d119e-102">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d119e-103">使用此 API 检索特定格式的项的内容。</span><span class="sxs-lookup"><span data-stu-id="d119e-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="d119e-104">并非所有文件都可转换成全部格式。</span><span class="sxs-lookup"><span data-stu-id="d119e-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="d119e-105">若要下载其原始格式中的项，请参阅[下载项目的内容](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="d119e-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d119e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d119e-106">Prerequisites</span></span>

<span data-ttu-id="d119e-107">应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d119e-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="d119e-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d119e-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="d119e-109">查询参数</span><span class="sxs-lookup"><span data-stu-id="d119e-109">Query parameters</span></span>

| <span data-ttu-id="d119e-110">参数</span><span class="sxs-lookup"><span data-stu-id="d119e-110">Parameter</span></span>      | <span data-ttu-id="d119e-111">类型</span><span class="sxs-lookup"><span data-stu-id="d119e-111">Type</span></span>  | <span data-ttu-id="d119e-112">描述</span><span class="sxs-lookup"><span data-stu-id="d119e-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="d119e-113">_format_</span><span class="sxs-lookup"><span data-stu-id="d119e-113">_format_</span></span>  | <span data-ttu-id="d119e-114">string</span><span class="sxs-lookup"><span data-stu-id="d119e-114">string</span></span> | <span data-ttu-id="d119e-115">指定应以何种格式下载项内容。</span><span class="sxs-lookup"><span data-stu-id="d119e-115">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="d119e-116">以下是**format**参数的有效值：</span><span class="sxs-lookup"><span data-stu-id="d119e-116">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="d119e-117">值</span><span class="sxs-lookup"><span data-stu-id="d119e-117">Value</span></span> | <span data-ttu-id="d119e-118">说明</span><span class="sxs-lookup"><span data-stu-id="d119e-118">Description</span></span>                        | <span data-ttu-id="d119e-119">支持的源扩展名</span><span class="sxs-lookup"><span data-stu-id="d119e-119">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="d119e-120">glb</span><span class="sxs-lookup"><span data-stu-id="d119e-120">glb</span></span>   | <span data-ttu-id="d119e-121">将项目转换成 GLB 格式</span><span class="sxs-lookup"><span data-stu-id="d119e-121">Converts the item into GLB format</span></span>  | <span data-ttu-id="d119e-122">不错，fbx、 obj、 往返流、 stl 3mf</span><span class="sxs-lookup"><span data-stu-id="d119e-122">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="d119e-123">html</span><span class="sxs-lookup"><span data-stu-id="d119e-123">html</span></span>  | <span data-ttu-id="d119e-124">将项目转换为 HTML 格式</span><span class="sxs-lookup"><span data-stu-id="d119e-124">Converts the item into HTML format</span></span> | <span data-ttu-id="d119e-125">eml md、 msg</span><span class="sxs-lookup"><span data-stu-id="d119e-125">eml, md, msg</span></span>
| <span data-ttu-id="d119e-126">.jpg</span><span class="sxs-lookup"><span data-stu-id="d119e-126">jpg</span></span>   | <span data-ttu-id="d119e-127">将项目转换为 JPG 格式</span><span class="sxs-lookup"><span data-stu-id="d119e-127">Converts the item into JPG format</span></span>  | <span data-ttu-id="d119e-128">3g 2、 3gp、 3gp2、 3gpp、 3mf、 ai、 arw、 asf、 avi、 营业活动报表、 bash、 bat、 bmp、 c、 cbl、 cmd、 不错、 cpp、 cr2、 crw、 cs、 css、 csv、 当前、 dcm、 dcm30、 词典、 dicm、 dicom、 dng、 doc、 docx、 dwg、 eml、 epi、 eps、 epsf、 epsi、 epub、 erf、 fbx、 fppx、 gif、 glb、 h、 hcpheic，heif，htm，html、 ico、 图标、 java、 jfif、 jpeg、 jpg、 js、 json、 密钥、 日志、 m2ts、 m4a、 m4v、 减价、 md、 mef、 mov、 影片、 mp3、 mp4 （英文）、 mp4v、 mrw、 msg、 mts、 nef、 nrw、 数字、 obj、 odp、 odt、 ogg、 orf、 页面、 全景、 pdf、 pef、 php、 pict、 pl、 往返流、 png、 potpotm，potx，pps，ppsx，ppsxm，ppt、 pptm、 pptx、 ps、 ps1、 psb、 psd、 上一年度，原始，rb、 rtf、 rw1、 rw2，sh，素描，sql、 sr2、 stl、 tif、 tiff、 ts、 txt、 vb、 webm、 wma、 wmv (英文)、 xaml、 xbm、 xcf、 xd、 xml、 xpm、 yaml、 yml</span><span class="sxs-lookup"><span data-stu-id="d119e-128">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="d119e-129">PDF</span><span class="sxs-lookup"><span data-stu-id="d119e-129">pdf</span></span>   | <span data-ttu-id="d119e-130">将项转换成 PDF 格式。</span><span class="sxs-lookup"><span data-stu-id="d119e-130">Converts the item into PDF format</span></span>  | <span data-ttu-id="d119e-131">doc、 docx、 epub、 eml、 htm、 html、 md、 msg、 odp、 ods、 odt、 pps、 ppsx、 ppt、 pptx、 rtf、 tif、 tiff、 xls、 xlsm、 xlsx</span><span class="sxs-lookup"><span data-stu-id="d119e-131">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="d119e-132">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d119e-132">Optional request headers</span></span>

| <span data-ttu-id="d119e-133">名称</span><span class="sxs-lookup"><span data-stu-id="d119e-133">Name</span></span>            | <span data-ttu-id="d119e-134">值</span><span class="sxs-lookup"><span data-stu-id="d119e-134">Value</span></span>   | <span data-ttu-id="d119e-135">说明</span><span class="sxs-lookup"><span data-stu-id="d119e-135">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d119e-136">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="d119e-136">_if-none-match_</span></span> | <span data-ttu-id="d119e-137">String</span><span class="sxs-lookup"><span data-stu-id="d119e-137">String</span></span>  | <span data-ttu-id="d119e-138">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="d119e-138">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="d119e-139">示例</span><span class="sxs-lookup"><span data-stu-id="d119e-139">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="d119e-140">响应</span><span class="sxs-lookup"><span data-stu-id="d119e-140">Response</span></span>

<span data-ttu-id="d119e-141">返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d119e-141">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="d119e-142">应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。</span><span class="sxs-lookup"><span data-stu-id="d119e-142">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="d119e-143">已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。</span><span class="sxs-lookup"><span data-stu-id="d119e-143">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="d119e-144">错误响应</span><span class="sxs-lookup"><span data-stu-id="d119e-144">Error responses</span></span>

<span data-ttu-id="d119e-145">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="d119e-145">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
