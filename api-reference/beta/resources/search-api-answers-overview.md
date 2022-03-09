---
title: 使用 Microsoft 搜索 API 管理管理答案
description: 使用 Microsoft Graph 管理 Microsoft 搜索体验中的管理搜索答案。
ms.localizationpriority: high
author: jakeost-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 4e3204594dde96fc5c51b1f27337ad3e84125fb8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338371"
---
# <a name="use-the-microsoft-search-api-to-manage-administrative-answers"></a>使用 Microsoft 搜索 API 管理管理答案

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以使用 Microsoft Graph 以在 [Microsoft 搜索](/microsoftsearch/overview-microsoft-search) 体验中管理管理搜索答案结果。

管理管理搜索答案的请求由全局管理员、搜索管理员、搜索编辑器执行，或者在无已登录用户的情况下代表应用程序执行，使用 [具有应用程序权限的访问令牌](/graph/auth-v2-service) 进行识别。

## <a name="common-use-cases"></a>常见用例

本节中 API 的用例涉及管理管理答案，例如组织的首字母缩略词、书签和 QnA。

| 用例                                        | REST 资源                              |
|:-------------------------------------------------|:--------------------------------------------|
| **搜索回答操作**                        |                                             |
| 创建、更新或删除搜索答案        | [首字母缩写词](search-acronym.md)、[书签](search-bookmark.md)、[qna](search-qna.md) |

## <a name="supported-language-tags"></a>受支持的语言标记
[书签](search-bookmark.md) 或 [qna](search-qna.md) 的语言标记表示可在其中查看搜索答案(**书签** 或 **qna**)的地理上的特定语言。 语言标记遵循 {language}-{REGION} 模式。 有关该模式的详细信息，请参阅 [RFC 4646](https://datatracker.ietf.org/doc/html/rfc4646)。

下表列出了可在 [Microsoft 365 管理中心](https://admin.microsoft.com/) 内设置的语言标记、区域设置以及相应的国家或地区，以便发布搜索答案。 **区域设置** 列描述了在该国家或地区中使用的语言。

| 受支持的语言标记 | Locale | 在 Microsoft 365 管理中心内选择国家或地区  |
| ----------- | ----------  | ----------  |
|`es-AR`| 西班牙语（阿根廷） | 阿根廷 | 
|`en-AU`| 英语（澳大利亚） | 澳大利亚 |
|`de-AT`| 德语（奥地利） |奥地利 | 
|`fr-BE`| 法语（比利时） |比利时 - 法语 | 
|`nl-BE`| 荷兰语（比利时） | 比利时 - 荷兰语 | 
|`en-CA`| 英语（加拿大） | 加拿大 - 英语 | 
|`fr-CA`| 法语（加拿大） | 加拿大 - 法语 | 
|`fr-FR`| 法语（法国） | 法国 | 
|`de-DE`| 德语（德国） | 德国 | 
|`zh-HK`| 中文（香港） | 香港特别行政区 |
|`en-IN`| 英语（印度） | 印度 |
|`it-IT`| 意大利语（意大利） | Italy（意大利） |
|`pt-BR`| 葡萄牙语（巴西） | 巴西 |
|`en-ID`| 英语(印度尼西亚) | 印度尼西亚 |
|`ja-JP`| 日语（日本） | 日本 |
|`ko-KR`| 韩语(韩国) | 韩国 |
|`en-MY`| 英语（马来西亚） | 马来西亚 |
|`es-MX`| 西班牙语（墨西哥） | 墨西哥 |
|`nl-NL`| 荷兰语（荷兰） | 荷兰 |
|`nb-NO`| 书面挪威语(挪威) | 挪威 |
|`zh-CN`| 中文（中国） | 中华人民共和国 |
|`pl-PL`| 波兰语（波兰） | Poland（波兰） |
|`ru-RU`| 俄语（俄罗斯） | 俄罗斯 |
|`ar-SA`| 阿拉伯语（沙特阿拉伯） | 沙特阿拉伯 |
|`sv-SE`| 瑞典语（瑞典） | 瑞典 |
|`es-ES`| 西班牙语（西班牙） | 西班牙 |
|`fr-CH`| 法语（瑞士） | 瑞士 - 法语 |
|`de-CH`| 德语（瑞士） | 瑞士 - 德语 |
|`en-ZA`| 英语（南非） | 南非 |
|`zh-TW`| 中文（台湾） | Taiwan（台湾） |
|`tr-TR`| 土耳其语(土耳其) | 土耳其 |
|`en-GB`| 英语（英国） | 英国 |
|`en-US`| 英语（美国） | 美国 - 英语 |
|`es-US`| 西班牙语（美国） | 美国 - 西班牙语 |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

- 请参阅 [Microsoft 搜索 API 概述](/graph/search-concept-overview)。
- 深入了解答案类型资源的方法、属性和关系: [书签](search-bookmark.md)、[首字母缩略词](search-acronym.md) 和 [QnA](search-qna.md)。

