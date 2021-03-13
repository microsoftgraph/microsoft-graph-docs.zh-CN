---
title: passwordSingleSignOnSettings 资源类型
description: 与基于密码的单一登录相关的设置
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e7e4402e6416166dd7c288cdd9aa9ec5ecbba06
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761540"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="d23c0-103">passwordSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d23c0-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d23c0-104">包含基于密码的单一登录设置的集合。</span><span class="sxs-lookup"><span data-stu-id="d23c0-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="d23c0-105">属性</span><span class="sxs-lookup"><span data-stu-id="d23c0-105">Properties</span></span>

| <span data-ttu-id="d23c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="d23c0-106">Property</span></span>     | <span data-ttu-id="d23c0-107">类型</span><span class="sxs-lookup"><span data-stu-id="d23c0-107">Type</span></span>        | <span data-ttu-id="d23c0-108">说明</span><span class="sxs-lookup"><span data-stu-id="d23c0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d23c0-109">域</span><span class="sxs-lookup"><span data-stu-id="d23c0-109">fields</span></span>|<span data-ttu-id="d23c0-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d23c0-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="d23c0-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d23c0-111">JSON representation</span></span>

<span data-ttu-id="d23c0-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d23c0-112">The following is a JSON representation of the resource.</span></span>

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

