---
title: publicClientApplication 资源类型
description: '指定非 Web 应用程序或 Web Api 的设置。  (例如，移动或其他公共客户端（如在桌面设备上运行的已安装应用程序）) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: e963e5b0ae6bd05dbf33ed5f8f3968c601ec1f62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037092"
---
# <a name="publicclientapplication-resource-type"></a>publicClientApplication 资源类型

命名空间：microsoft.graph

指定非 web 应用程序或非 web API (的设置，例如，移动或其他公用客户端（如在桌面设备上运行的已安装应用程序) ）。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|redirectUris|String collection| 指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。 |

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

