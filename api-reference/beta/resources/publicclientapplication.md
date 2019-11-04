---
title: publicClientApplication 资源类型
description: 指定非 Web 应用程序或 Web Api 的设置。 （例如，移动或其他公共客户端，如在桌面设备上运行的已安装应用程序）
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a9d54ed7f15f6bbcabd85ee50e8137b131399b22
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939381"
---
# <a name="publicclientapplication-resource-type"></a>publicClientApplication 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定非 web 应用或非 web API 的设置（例如，移动或其他公共客户端，如在桌面设备上运行的已安装应用程序）。

## <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
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
