---
title: Microsoft Graph 中 OneNote API 的错误代码
description: 每当通过 API 发送的请求失败时，在 Microsoft Graph 中查找有关 OneNote API 返回的错误代码的信息。
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 378dae17b2c0668a33b50a1275f409f9b8e4d015
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668144"
---
# <a name="error-codes-for-the-onenote-api-in-microsoft-graph"></a>Microsoft Graph 中 OneNote API 的错误代码

本文介绍每当通过 API 发送的请求失败时，OneNote API 在 Microsoft Graph 中返回的错误代码。

## <a name="error-response-example"></a>错误响应示例

请求生成错误时，OneNote API 将停止执行此请求并将错误响应作为 JSON 对象返回。 错误响应将包含相关的错误代码、消息和本文相应部分的链接。 以下示例演示了错误响应的外观。

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

有关 Microsoft Graph 错误的详细信息，请参阅 [Microsoft Graph 错误响应和资源类型](errors.md)。

## <a name="codes-from-10001-to-19999"></a>从 10001 到 19999 的代码

服务遇到问题，或向应用程序发送信息。

### <a name="10001"></a>10001
出现意外错误，请求失败。

### <a name="10002"></a>10002
服务当前不可用。

### <a name="10003"></a>10003
当前用户的帐户已超过最大活动请求数。 你的应用将不得不重复请求。

### <a name="10004"></a>10004
服务无法在请求的部分创建页面，因为该部分受密码保护。

### <a name="10005"></a>10005
请求包含超过最大数量的图像标记，其中 **data-render-src** 属性包含 PDF。 请参阅[添加图像和文件](onenote-images-files.md)。

### <a name="10006"></a>10006
OneNote API 程序无法在指定部分创建页面，因为该部分已损坏。

### <a name="10007"></a>10007
服务器太忙，目前无法处理传入的请求。请稍后重试。

### <a name="10008"></a>10008
用户或组的 OneDrive 上的一个或多个文档库包含的 OneNote 项目数（笔记本、分区、分区组）超过 5000 个，无法使用 API 查询。 请确保用户或组的文档库包含的 OneNote 项目数均未超过 5000 个。 请参阅 [OneNote 开发博客](/archive/blogs/onenotedev/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library)获取缓解步骤。

### <a name="10012"></a>10012
无法创建或更新实体，因为包含笔记本的库要求先将项目签出然后才能编辑这些项。 有关详细信息，请参阅[设置库以请求签出文件](https://support.office.com/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7)。

可从库中删除签出要求，也可以移动笔记本。

### <a name="10013"></a>10013
用户或组 OneDrive 上的一个或多个文档库包含 20,000 多个项目，无法使用 API 通过索引进行查询。请确保没有任何一个用户或组的文档库包含超过 20,000 个项目。有关缓解步骤，请参阅 [OneNote 开发人员博客](/archive/blogs/onenotedev/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library)。

### <a name="10014"></a>10014
Azure Key Vault 太忙，目前无法处理传入的请求。 请稍后重试。

### <a name="10015"></a>10015
SharePoint 当前不可用。 请稍后重试。

### <a name="10016"></a>10016
用户或组的 OneDrive 上的文档库超出了唯一的安全作用域阈值限制。 为库设置的唯一安全作用域的最大数量不能超过 50,000 个。

### <a name="10017"></a>10017
错误的请求。

### <a name="19999"></a>19999
请求失败，因为发生无法确定的错误。

## <a name="codes-from-20001-to-29999"></a>从 20001 到 29999 的代码

应用程序代码已经出现问题。

### <a name="20001"></a>20001

请求缺少必需的“演示”部分。 只需要一个。 

### <a name="20002"></a>20002
请求包含两个或更多个“演示”部分。 只需要一个。

### <a name="20003"></a>20003
“演示”部分的内容类型只能是文本/HTML 或应用程序/XHTML+XML。 

### <a name="20004"></a>20004
“演示”部分 HTML 包含一个图像标记，其中包含 **src** 和 **data-render-src** 属性集。API 将忽略 **src** 属性并使用 **data-render-src** 属性。 

### <a name="20005"></a>20005
请求 URI 太长。 URI 的最大大小（包括所有参数和数据）为 16 KB 或 16,384 个字符。

### <a name="20006"></a>20006
“演示”部分 HTML 包含未设置 src 和 **data-render-src** 属性的图像标记。 API 将忽略该 **图像** 标记。 

### <a name="20007"></a>20007
“演示文稿”部分 HTML 包含与任何允许的格式均不匹配的创建日期/时间字符串。 

### <a name="20008"></a>20008
请求大小太大。 

### <a name="20009"></a>20009
请求包含使用重复名称的部分。 部分名称必须是唯一的。 

### <a name="20010"></a>20010
未提供指定内容类型的内容处置标头。 

### <a name="20011"></a>20011
请求包含格式错误的多部分有效负载。 问题可能包括缺少空行、缺少末行、部分分隔符格式不正确等。 如果正在手动生成多部分消息，请仔细检查逻辑，或者考虑使用第三方库。 

### <a name="20012"></a>20012
请求未提供指定部分的内容类型。 

### <a name="20013"></a>20013
请求未提供指定部分的内容类型和内容处置标头。 

### <a name="20014"></a>20014
多部分消息中的某个部分的长度超过最大大小 25 MB。 

### <a name="20015"></a>20015
多部分消息中的部分计数超过 500 个的限制。 

### <a name="20016"></a>20016
多部分消息的长度超过 75 MB 的限制。 

### <a name="20017"></a>20017
电子邮件 MIME 格式不正确。 

### <a name="20018"></a>20018
会议 MIME 或 ICal 格式不正确。 

### <a name="20019"></a>20019
找不到 ICal。 

### <a name="20020"></a>20020
在请求正文中遇到格式不正确的 Json。 

### <a name="20100"></a>20100
请求的语法有问题。 

### <a name="20101"></a>20101
所请求的属性不存在。

### <a name="20102"></a>20102
所请求的资源不存在。

### <a name="20103"></a>20103
此请求不支持 **expand** 查询。 请参阅[受支持的 OData 查询字符串选项](onenote-get-content.md#supported-odata-query-string-options)。

### <a name="20104"></a>20104
仅当查询某个部分中的网页集或查询特定页时，才支持 **pagelevel** 查询选项。例如：  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a>20106
你的请求包含不受支持的查询运算符。 

### <a name="20108"></a>20108
您的请求包含不受支持的 OData 查询参数。

### <a name="20109"></a>20109
PATCH 请求中的有效负载构建不正确。

### <a name="20110"></a>20110
包含数据部分的页面创建请求要求内容为多部分，并包含“演示”部分。 

### <a name="20111"></a>20111
你的请求使用不受支持的 OData 功能。

### <a name="20112"></a>20112
您的请求包含无效的目标笔记本、节组、节或页面实体 ID。

### <a name="20113"></a>20113
请求中指定的资源已被删除。

### <a name="20115"></a>20115
名称包含无效字符。 笔记本名称中不能包含下列任意字符：`? * \ / : < > | ' "`

### <a name="20117"></a>20117
在您指定的位置中已存在指定名称的项。

### <a name="20119"></a>20119
“演示”部分的 HTML 包含一个 **data-attachment** 属性，该属性不为有效格式，或者包含一个或多个对文件名无效的字符：`\ / : * ? < > | "`。 请求替代了错误消息中指示的值。

### <a name="20120"></a>20120
找不到你的请求指定的 PATCH 目标。

### <a name="20121"></a>20121
请求包含无效的 PATCH 参数。请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20122"></a>20122
请求指定的 PATCH 操作不受支持。请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20123"></a>20123
PATCH 请求无法修改指定页面。

### <a name="20124"></a>20124
你的多部分 PATCH 请求不包含使用 PATCH 操作 JSON 结构的“命令”部分。 请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20125"></a>20125
PATCH 请求不包含任何操作。请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20126"></a>20126
邮件正文包含格式错误的 JSON 或此操作不支持的字段。

### <a name="20127"></a>20127
您的请求指定了未知属性的名称。

### <a name="20128"></a>20128
您的请求在消息中指示的位置包含 OData 语法错误。

### <a name="20129"></a>20129
你的请求包含值过高的 **top** 查询字符串选项。 对于页面查询，最大值为 100，默认值为 20。

### <a name="20130"></a>20130
你的请求包含指向找不到的 HTTP 资源的 URI。

### <a name="20131"></a>20131
你的请求包含无效的内容类型值。 请使用消息中指示的值。 

### <a name="20132"></a>20132
你的请求包含无效的内容。 此问题的常见原因是缺少内容类型请求标头和/或请求正文中没有内容。 

### <a name="20133"></a>20133
你的请求指定的 PATCH 目标不受支持。 请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20134"></a>20134
您的请求将无效元素指定为 PATCH 操作的目标。如果目标使用 **data-id** 标识符，请确保其前缀为 # 符号。请参阅 [更新页面内容](onenote-update-page.md)。

### <a name="20135"></a>20135
你的请求指定的实体类型不受 PATCH 操作支持。 请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20136"></a>20136
你的请求包含无效的 **data-render-src** 或 **data-render-method** 属性或缺失这些属性。 请参阅[从捕获内容中提取数据](onenote-extract-data.md)。

### <a name="20137"></a>20137
目标页面不支持 PATCH 请求。

### <a name="20138"></a>20138
PATCH 请求中的目标元素类型不支持 **append** 操作。请参阅 [更新页面内容](onenote-update-page.md)。

### <a name="20139"></a>20139
请求包含无效的 **data-tag** 属性值。请参阅 [使用笔记标记](onenote-note-tags.md)。

### <a name="20140"></a>20140
你的请求包含无效的 **data-tag** 状态值。 复选框笔记标记可以包含 **已完成** 状态。 

示例：

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
请参阅[使用笔记标记](onenote-note-tags.md)。

### <a name="20141"></a>20141
PATCH 请求中的目标不支持指定操作。 请参阅[更新页面内容](onenote-update-page.md)。

### <a name="20142"></a>20142
你的请求包含子实体的父项或父实体的子项的 **expand** 表达式，但它并不受支持。 请参阅[受支持的 OData 查询字符串选项](onenote-get-content.md#supported-odata-query-string-options)。

### <a name="20143"></a>20143
OData 查询无效。

### <a name="20144"></a>20144
你的请求包含非导航属性的 **expand** 表达式。 只能扩展导航属性。

### <a name="20145"></a>20145
你的请求中的 **select** 或 **expand** 表达式包含无效条件。

### <a name="20146"></a>20146
元素上指定了 `style="position:absolute"` 属性，但是 **body** 元素未指定支持定位所需的 `data-absolute-enabled="true"`。 将忽略所有的定位设置。 请参阅[创建绝对定位的元素](onenote-abs-pos.md)。

### <a name="20147"></a>20147
在非 **body** 元素直接子级的元素上指定了不受支持的 `style="position:absolute"` 属性。 如果元素是 **div**、**img** 或 **object**，请使其成为正文的直接子级；否则，将忽略定位设置，并在绝对定位的 div 中呈现它的内容。 请参阅[创建绝对定位的元素](onenote-abs-pos.md)。

### <a name="20148"></a>20148
在不支持 `style="position:absolute"` 属性的元素类型上指定了此属性。 仅属于页面正文直接子级的 **div**、**img**、和 **object** 元素支持定位。 请参阅[创建绝对定位的元素](onenote-abs-pos.md)。

### <a name="20149"></a>20149
您的请求指定的目标元素找不到。

### <a name="20150"></a>20150
请求对此身份验证类型无效。 请改用 `../me/onenote/` 路径。

### <a name="20151"></a>20151
请求对此身份验证类型无效。 请使用 `../me/onenote/section/{id}/pages` 终结点在特定分区中创建页面。

### <a name="20152"></a>20152
没有为实体指定任何 name 值。必须定义名称，并且其中不能仅包含空格。

### <a name="20153"></a>20153
实体名称包含无效字符。 名称中不能包含下列字符：`? * \ / : < > | & # " % ~`

### <a name="20154"></a>20154
实体名称不能以空格开头。

### <a name="20155"></a>20155
实体名称太长。 笔记本名称的字符数限制为 128 个。 其他实体名称的字符数限制为 50 个。

### <a name="20156"></a>20156
目标资源的指定 ID 不存在。

### <a name="20157"></a>20157
目标实体的指定 ID 无效。

### <a name="20158"></a>20158
无法获取请求中指定的网站 URL 的元数据。 请检查所提供的 URL 的格式。 支持的格式包括 `https://domain.sharepoint.com/site-a` 和 `https://domain.com/sites/site-a`。

### <a name="20160"></a>20160
找不到具有指定 ID 的 Office 365 统一组。

### <a name="20161"></a>20161
此上下文没有指定有效的用户 ID。 一个常见错误是 PUID/CID 作为 long 而不是作为 hex 传入。

### <a name="20166"></a>20166
应用程序在短时间内以用户身份发出的请求过多。 当 API 检测到应用程序使用的资源过多时，它会返回 429 状态代码和此错误，以帮助确保 OneNote API 保持稳定和可响应状态。 

有关详细信息，请参阅 [Microsoft Graph 服务特定的限制指南](./throttling-limits.md)。

### <a name="20168"></a>20168
请求中指定的视频源不受支持。 请参阅[支持的视频网站](onenote-images-files.md#adding-videos)获取最新列表。


## <a name="codes-from-30001-to-39999"></a>从 30001 到 39999 的代码
用户的帐户有问题。

### <a name="30101"></a>30101
用户帐户超出了它的 OneDrive 配额。 请参阅 [OneDrive](https://onedrive.live.com/about/)。

### <a name="30102"></a>30102
不能再向请求的节添加任何内容，因为它已经达到其最大大小。

### <a name="30103"></a>30103
此请求的资源消耗过高。 目标用户帐户的数据集过大或服务将过多数量的并发请求接收到同一个网站（例如，用户的个人网站或团队网站）。

### <a name="30104"></a>30104
用户帐户已被挂起。

### <a name="30105"></a>30105
未设置用户的个人 OneDrive for Business 网站，需要设置该网站才能访问笔记本。 OneNote 服务将立即设置此网站。 此进程可能需要几分钟。

### <a name="30106"></a>30106
正在为用户设置 OneDrive for Business。

### <a name="30108"></a>30108
无法检索用户的个人 OneDrive for Business。 下表列出了部分可能的原因。

| 原因 | 解决方案 |
|:------|:------|
| 尚未设置用户的个人网站。 | 用户应打开 OneDrive for Business，并按照任意说明设置此网站。 如果失败，应联系其 Microsoft 365 租户管理员。 |
| 当前正在设置用户的个人网站。 | 稍后再尝试请求。 |
| 用户没有有效的 OneDrive for Business 许可证。 | 用户应联系其 Microsoft 365 租户管理员。 |
| 网络问题使请求无法成功发送。 | 稍后再尝试请求。 |

### <a name="30109"></a>30109
请求中的某些用户不存在。

### <a name="30110"></a>30110
此租户尚未注册学生信息服务。

### <a name="30111"></a>30111
学生信息服务出现一般性错误。

### <a name="30112"></a>30112
受请求影响的多个用户具有相同的用户名。

### <a name="30113"></a>30113
笔记本未配置为允许邀请。

### <a name="30114"></a>30114
缺少必需的参数。

## <a name="codes-from-40001-to-49999"></a>从 40001 到 49999 的代码
用户或应用程序没有正确的权限。

### <a name="40001"></a>40001
请求不包含有效的 OAuth 标记。 请参阅[注释权限](permissions-reference.md#notes-permissions)。

### <a name="40002"></a>40002
用户在所请求的位置没有写入权限。

### <a name="40003"></a>40003
用户没有权限访问所请求的资源。

### <a name="40004"></a>40004
OAuth 令牌没有所需的作用域来执行所请求的操作。 请参阅[注释权限](permissions-reference.md#notes-permissions)。

### <a name="40006"></a>40006 
OAuth 令牌没有所需的作用域来执行所请求的操作。 尤其是编辑权限。 请参阅[注释权限](permissions-reference.md#notes-permissions)。

### <a name="40007"></a>40007
用户没有权限访问此资源。

### <a name="40008"></a>40008
禁止访问此资源。

### <a name="40009"></a>40009
容器已被其他资源使用。

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 错误响应和资源类型](errors.md)
- [OneNote API 参考](/graph/api/resources/onenote)
