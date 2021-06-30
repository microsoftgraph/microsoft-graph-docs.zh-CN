---
title: resultTemplateOption 资源类型
description: 提供呈现连接器搜索结果的搜索显示布局选项。
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 404051f4eeee68ca3d5f5eb3ac6b84a23a331515
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211231"
---
# <a name="resulttemplateoption-resource-type"></a><span data-ttu-id="c38e9-103">resultTemplateOption 资源类型</span><span class="sxs-lookup"><span data-stu-id="c38e9-103">resultTemplateOption resource type</span></span>

<span data-ttu-id="c38e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c38e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c38e9-105">提供用于呈现连接器搜索结果的搜索结果模板选项。</span><span class="sxs-lookup"><span data-stu-id="c38e9-105">Provides the search result templates options for render connectors search results.</span></span>

## <a name="properties"></a><span data-ttu-id="c38e9-106">属性</span><span class="sxs-lookup"><span data-stu-id="c38e9-106">Properties</span></span>

| <span data-ttu-id="c38e9-107">属性</span><span class="sxs-lookup"><span data-stu-id="c38e9-107">Property</span></span>     | <span data-ttu-id="c38e9-108">类型</span><span class="sxs-lookup"><span data-stu-id="c38e9-108">Type</span></span>        | <span data-ttu-id="c38e9-109">说明</span><span class="sxs-lookup"><span data-stu-id="c38e9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c38e9-110">enableResultTemplate</span><span class="sxs-lookup"><span data-stu-id="c38e9-110">enableResultTemplate</span></span>|<span data-ttu-id="c38e9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="c38e9-111">Boolean</span></span>|<span data-ttu-id="c38e9-112">指示是否启用搜索显示布局。</span><span class="sxs-lookup"><span data-stu-id="c38e9-112">Indicates whether search display layouts are enabled.</span></span> <span data-ttu-id="c38e9-113">如果启用，用户将获取结果模板，以在响应 的 **resultTemplates** 属性中呈现 [搜索结果内容](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="c38e9-113">If enabled, the user will get the result template to render the search results content in the **resultTemplates** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="c38e9-114">结果模板基于自适应 [卡片](https://adaptivecards.io/)。</span><span class="sxs-lookup"><span data-stu-id="c38e9-114">The result template is based on [Adaptive Cards](https://adaptivecards.io/).</span></span> <span data-ttu-id="c38e9-115">此属性可选。</span><span class="sxs-lookup"><span data-stu-id="c38e9-115">This property is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c38e9-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c38e9-116">JSON representation</span></span>

<span data-ttu-id="c38e9-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c38e9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplateOption",
  "baseType": null
}-->

```json
 {
    "enableResultTemplate": true
 }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplateOption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
