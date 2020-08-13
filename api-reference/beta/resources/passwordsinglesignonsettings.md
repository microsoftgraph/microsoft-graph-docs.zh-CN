---
title: passwordSingleSignOnSettings 资源类型
description: 与基于密码的单一登录相关的设置
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4da86cb39a1b16c9312ebe8de35c7fc87a09fdb
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658173"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="67607-103">passwordSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="67607-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67607-104">包含基于密码的单一登录设置的集合。</span><span class="sxs-lookup"><span data-stu-id="67607-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="67607-105">属性</span><span class="sxs-lookup"><span data-stu-id="67607-105">Properties</span></span>

| <span data-ttu-id="67607-106">属性</span><span class="sxs-lookup"><span data-stu-id="67607-106">Property</span></span>     | <span data-ttu-id="67607-107">类型</span><span class="sxs-lookup"><span data-stu-id="67607-107">Type</span></span>        | <span data-ttu-id="67607-108">说明</span><span class="sxs-lookup"><span data-stu-id="67607-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67607-109">域</span><span class="sxs-lookup"><span data-stu-id="67607-109">fields</span></span>|<span data-ttu-id="67607-110">[passwordSingleSignOnField](passwordsinglesignonfield.md)集合</span><span class="sxs-lookup"><span data-stu-id="67607-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="67607-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67607-111">JSON representation</span></span>

<span data-ttu-id="67607-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67607-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnSettings",
  "baseType": null
}-->

```json
{
  "fields": [{"@odata.type": "microsoft.graph.passwordSingleSignOnField"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->