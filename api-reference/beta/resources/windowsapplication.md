---
title: windowsApplication 资源类型
description: 表示运行 Microsoft Windows并在 Microsoft Store 或 Xbox 游戏商店中发布的应用的设置。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: aricrowe57
ms.openlocfilehash: 9472a8c39a9ddeb7ed7a3857c5bba11c8435d44c
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848677"
---
# <a name="windowsapplication-resource-type"></a>windowsApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示运行 Microsoft Windows并在 Microsoft Store 或 Xbox 游戏商店中发布的应用的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| packageSid | 字符串 | Microsoft 已分配应用程序的包安全标识符。 可选。 只读。 |
| redirectUris | String collection | 指定为登录发送用户令牌的 URL，或在其中发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。 仅适用于支持 **signInAudience 的**`PersonalMicrosoftAccount`应用程序。 |

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
