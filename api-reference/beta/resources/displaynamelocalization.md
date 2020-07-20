---
title: displayNameLocalization 资源类型
description: 使管理员能够自定义在共享 Microsoft 365 体验中使用的字符串。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8ae6c62acfacfccd22cc9985386762a2f61a2bc7
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050854"
---
# <a name="displaynamelocalization-resource-type"></a><span data-ttu-id="2e094-103">displayNameLocalization 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e094-103">displayNameLocalization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e094-104">使管理员能够自定义在共享 Microsoft 365 体验中使用的字符串。</span><span class="sxs-lookup"><span data-stu-id="2e094-104">Provides the ability for an administrator to customize the string used in a shared Microsoft 365 experience.</span></span>

## <a name="properties"></a><span data-ttu-id="2e094-105">属性</span><span class="sxs-lookup"><span data-stu-id="2e094-105">Properties</span></span>

| <span data-ttu-id="2e094-106">属性</span><span class="sxs-lookup"><span data-stu-id="2e094-106">Property</span></span>     | <span data-ttu-id="2e094-107">类型</span><span class="sxs-lookup"><span data-stu-id="2e094-107">Type</span></span>        | <span data-ttu-id="2e094-108">说明</span><span class="sxs-lookup"><span data-stu-id="2e094-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e094-109">displayName</span><span class="sxs-lookup"><span data-stu-id="2e094-109">displayName</span></span>   |<span data-ttu-id="2e094-110">String</span><span class="sxs-lookup"><span data-stu-id="2e094-110">String</span></span>       | <span data-ttu-id="2e094-111">如果存在，则此字段的值包含已为**languageTag**字段中存在的语言设置的**displayName**字符串。</span><span class="sxs-lookup"><span data-stu-id="2e094-111">If present, the value of this field contains the **displayName** string that has been set for the language present in the **languageTag** field.</span></span>|
|<span data-ttu-id="2e094-112">languageTag</span><span class="sxs-lookup"><span data-stu-id="2e094-112">languageTag</span></span>   |<span data-ttu-id="2e094-113">String</span><span class="sxs-lookup"><span data-stu-id="2e094-113">String</span></span>       | <span data-ttu-id="2e094-114">提供在其中提供了**displayName**字段的语言的语言区域性代码和友好名称。</span><span class="sxs-lookup"><span data-stu-id="2e094-114">Provides the language culture-code and friendly name of the language that the **displayName** field has been provided in.</span></span>                  |

## <a name="json-representation"></a><span data-ttu-id="2e094-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e094-115">JSON representation</span></span>

<span data-ttu-id="2e094-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e094-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
