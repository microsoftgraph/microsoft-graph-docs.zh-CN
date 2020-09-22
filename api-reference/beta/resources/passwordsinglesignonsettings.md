---
title: passwordSingleSignOnSettings 资源类型
description: 与基于密码的单一登录相关的设置
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1b2739ecbd5d09358e58203ab61d4e65c48716b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998171"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="0f47a-103">passwordSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f47a-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f47a-104">包含基于密码的单一登录设置的集合。</span><span class="sxs-lookup"><span data-stu-id="0f47a-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="0f47a-105">属性</span><span class="sxs-lookup"><span data-stu-id="0f47a-105">Properties</span></span>

| <span data-ttu-id="0f47a-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f47a-106">Property</span></span>     | <span data-ttu-id="0f47a-107">类型</span><span class="sxs-lookup"><span data-stu-id="0f47a-107">Type</span></span>        | <span data-ttu-id="0f47a-108">说明</span><span class="sxs-lookup"><span data-stu-id="0f47a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f47a-109">域</span><span class="sxs-lookup"><span data-stu-id="0f47a-109">fields</span></span>|<span data-ttu-id="0f47a-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f47a-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="0f47a-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f47a-111">JSON representation</span></span>

<span data-ttu-id="0f47a-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f47a-112">The following is a JSON representation of the resource.</span></span>

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

