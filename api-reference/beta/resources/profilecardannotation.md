---
title: profileCardAnnotation 资源类型
description: 允许管理员自定义 Microsoft 365 配置文件卡片中所选字段的外观。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 973732dc92527dcf3795b8796e1c817ba880836c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051004"
---
# <a name="profilecardannotation-resource-type"></a><span data-ttu-id="fdac7-103">profileCardAnnotation 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdac7-103">profileCardAnnotation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdac7-104">用于为共享的 Microsoft 365 人员 experieence 中显示的字段设置自定义显示名称。</span><span class="sxs-lookup"><span data-stu-id="fdac7-104">Used to set a custom display name for fields that surface in a shared Microsoft 365 people experieence.</span></span> <span data-ttu-id="fdac7-105">管理员可以为其组织中支持的语言定义默认的显示名称字符串和一组替代转换。</span><span class="sxs-lookup"><span data-stu-id="fdac7-105">An administrator can define a default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

## <a name="properties"></a><span data-ttu-id="fdac7-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdac7-106">Properties</span></span>

| <span data-ttu-id="fdac7-107">属性</span><span class="sxs-lookup"><span data-stu-id="fdac7-107">Property</span></span>     | <span data-ttu-id="fdac7-108">类型</span><span class="sxs-lookup"><span data-stu-id="fdac7-108">Type</span></span>                                                            | <span data-ttu-id="fdac7-109">说明</span><span class="sxs-lookup"><span data-stu-id="fdac7-109">Description</span></span>                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fdac7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="fdac7-110">displayName</span></span>   |<span data-ttu-id="fdac7-111">String</span><span class="sxs-lookup"><span data-stu-id="fdac7-111">String</span></span>                                                           | <span data-ttu-id="fdac7-112">如果存在，则配置文件卡片将使用此字段的值作为体验中的默认属性标签（例如，"成本中心"）。</span><span class="sxs-lookup"><span data-stu-id="fdac7-112">If present, the value of this field is used by the profile card as the default property label in the experience (for example, "Cost Center").</span></span> |
|<span data-ttu-id="fdac7-113">localizations</span><span class="sxs-lookup"><span data-stu-id="fdac7-113">localizations</span></span> |<span data-ttu-id="fdac7-114">[displayNameLocalization](displaynamelocalization.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdac7-114">[displayNameLocalization](displaynamelocalization.md) collection</span></span> | <span data-ttu-id="fdac7-115">此集合中的每个资源都代表给定语言的属性名称的本地化值，用作该区域设置的默认标签。</span><span class="sxs-lookup"><span data-stu-id="fdac7-115">Each resource in this collection represents the localized value of the attribute name for a given language, used as the default label for that locale.</span></span> <span data-ttu-id="fdac7-116">例如，拥有客户端的用户将 `no-NB` "Kostnads Senter" 作为属性标签，而不是 "成本中心"。</span><span class="sxs-lookup"><span data-stu-id="fdac7-116">For example, a user with a `no-NB` client gets "Kostnads Senter" as the attribute label, rather than "Cost Center."</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdac7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdac7-117">JSON representation</span></span>

<span data-ttu-id="fdac7-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdac7-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [
    {
      "displayName": "String",
      "languageTag": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardAnnotation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
