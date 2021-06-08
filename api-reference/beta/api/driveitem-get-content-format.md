---
author: JeremyKelley
description: 使用此 API 检索特定格式的项的内容。
ms.date: 09/10/2017
title: 转换为其他格式
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f6343e3b0ce7ba9eb114e6eeadc6040341fb5c47
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786816"
---
# <a name="download-a-file-in-another-format"></a>以其他格式下载文件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 检索特定格式的项的内容。 并非所有文件都可转换成全部格式。

若要下载原始格式的项目，请参阅[下载项内容](driveitem-get-content.md)。

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


以下值对于 **format** 参数有效：

| 值 | 说明                        | 支持的源扩展名
|:------|:-----------------------------------|---------------------------------
| glb   | 将项转换为 GLB 格式  | cool、fbx、obj、ply、stl、3mf
| html  | 将项转换为 HTML 格式 | eml、md、msg
| jpg   | 将项转换为 JPG 格式  | 3g2、3gp、3gp2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、cool、cpp、cr2、crw、cs、css、csv、cur、dcm、dcm30、dic、dicm、dicom、dng、doc、docx、dwg、eml、epi、eps、epsf、epsi、epub、erf、fbx、fppx、gif、glb、h、hcp、heic、heif、htm、html、ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、movie、mp3、mp4、mp4v、mrw、msg、mts、nef、nrw、numbers、obj、odp、odt、ogg、orf、pages、pano、pdf、pef、php、pict、pl、ply、png、pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、ps、ps1、psb、psd、py、raw、rb、rtf、rw1、rw2、sh、sketch、sql、sr2、stl、tif、tiff、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml
| pdf   | 将项转换为 PDF 格式  | doc、docx、epub、eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、pptx、rtf、tif、tiff、xls、xlsm、xlsx

## <a name="optional-request-headers"></a>可选的请求标头

| 名称            | 值   | 说明                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | 如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。 |

## <a name="example"></a>示例


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>响应

返回 `302 Found` 响应，重定向到已转换文件的已预先验证的下载 URL。

应用必须遵循响应中的 `Location` 头，才能下载已转换的文件。

已预先验证的 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可访问。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

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


