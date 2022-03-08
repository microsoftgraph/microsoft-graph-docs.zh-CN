---
title: windowsApplication 资源类型
description: 表示运行 Microsoft Windows且在 Microsoft Store Xbox 游戏商店中发布的设置。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: aricrowe57
ms.openlocfilehash: 7caedf0d8f8cda38129cfc108a2e4dc7ce609279
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338277"
---
# <a name="webapplication-resource-type"></a>webApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示运行 Microsoft Windows且在 Microsoft Store Xbox 游戏商店中发布的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| packageSid | String | Microsoft 已分配应用程序的程序包安全标识符。 可选。 只读。 |
| redirectUris | 字符串集合 | 指定用于登录的用户令牌的 URL 或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。 仅适用于支持 `PersonalMicrosoftAccount` **signInAudience 的应用程序**。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.windowsApplication"
}-->

```json
{
  "packageSid": "String",
  "redirectUris": ["String"]
}

```