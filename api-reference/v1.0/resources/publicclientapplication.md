---
title: publicClientApplication 资源类型
description: '指定非 Web 应用或 Web Api 的设置。  (，例如移动或其他公共客户端，如在桌面设备上运行的已安装) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a15f0ea159ab12403186465783200a9e374562bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137513"
---
# <a name="publicclientapplication-resource-type"></a>publicClientApplication 资源类型

命名空间：microsoft.graph

指定非 Web 应用或非 Web API (例如移动或其他公共客户端（如桌面设备上运行的已安装应用程序）的设置) 。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|redirectUris|String collection| 指定用于登录的用户令牌的发送 URL，或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

