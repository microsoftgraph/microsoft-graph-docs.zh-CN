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
# <a name="download-a-file-in-another-format"></a>以其他格式下载文件

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

使用此 API 检索特定格式的项的内容。
并非所有文件都可转换成全部格式。

若要下载其原始格式中的项，请参阅[下载项目的内容](driveitem-get-content.md)。

## <a name="prerequisites"></a>先决条件

应用必须拥有用户授予的对应用要转换的文件的读取权限，才能调用此 API。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a>查询参数

| 参数      | 类型  | 说明                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | string | 指定应以何种格式下载项内容。 |


以下是**format**参数的有效值：

| 值 | 说明                        | 支持的源扩展名
|:------|:-----------------------------------|---------------------------------
| glb   | 将项目转换成 GLB 格式  | 不错，fbx、 obj、 往返流、 stl 3mf
| html  | 将项目转换为 HTML 格式 | eml md、 msg
| jpg   | 将项目转换为 JPG 格式  | 3g 2、 3gp、 3gp2、 3gpp、 3mf、 ai、 arw、 asf、 avi、 营业活动报表、 bash、 bat、 bmp、 c、 cbl、 cmd、 不错、 cpp、 cr2、 crw、 cs、 css、 csv、 当前、 dcm、 dcm30、 词典、 dicm、 dicom、 dng、 doc、 docx、 dwg、 eml、 epi、 eps、 epsf、 epsi、 epub、 erf、 fbx、 fppx、 gif、 glb、 h、 hcpheic，heif，htm，html、 ico、 图标、 java、 jfif、 jpeg、 jpg、 js、 json、 密钥、 日志、 m2ts、 m4a、 m4v、 减价、 md、 mef、 mov、 影片、 mp3、 mp4 （英文）、 mp4v、 mrw、 msg、 mts、 nef、 nrw、 数字、 obj、 odp、 odt、 ogg、 orf、 页面、 全景、 pdf、 pef、 php、 pict、 pl、 往返流、 png、 potpotm，potx，pps，ppsx，ppsxm，ppt、 pptm、 pptx、 ps、 ps1、 psb、 psd、 上一年度，原始，rb、 rtf、 rw1、 rw2，sh，素描，sql、 sr2、 stl、 tif、 tiff、 ts、 txt、 vb、 webm、 wma、 wmv (英文)、 xaml、 xbm、 xcf、 xd、 xml、 xpm、 yaml、 yml
| pdf   | 将项目转换为 PDF 格式  | doc、 docx、 epub、 eml、 htm、 html、 md、 msg、 odp、 ods、 odt、 pps、 ppsx、 ppt、 pptx、 rtf、 tif、 tiff、 xls、 xlsm、 xlsx

## <a name="optional-request-headers"></a>可选的请求标头

| 名称            | 值   | 说明                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | 如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。 |

## <a name="example"></a>示例

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a>响应

返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。

应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。

已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
