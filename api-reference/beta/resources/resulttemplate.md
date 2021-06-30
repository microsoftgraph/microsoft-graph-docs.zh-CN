---
title: resultTemplate 资源类型
description: resultTemplateIds 和关联值的字典，其中包括结果模板的名称和 JSON 架构。
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 402b60efc278e72102d9bba4eb89be2dda38916b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211232"
---
# <a name="resulttemplate-resource-type"></a><span data-ttu-id="cf662-103">resultTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf662-103">resultTemplate resource type</span></span>

<span data-ttu-id="cf662-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf662-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf662-105">**resultTemplateIds** 和相关值的字典，其中包括结果模板的名称和 JSON 架构。</span><span class="sxs-lookup"><span data-stu-id="cf662-105">A dictionary of **resultTemplateIds** and associated values, which includes the name and JSON schema of the result templates.</span></span>

## <a name="properties"></a><span data-ttu-id="cf662-106">属性</span><span class="sxs-lookup"><span data-stu-id="cf662-106">Properties</span></span>

| <span data-ttu-id="cf662-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf662-107">Property</span></span>     | <span data-ttu-id="cf662-108">类型</span><span class="sxs-lookup"><span data-stu-id="cf662-108">Type</span></span>        | <span data-ttu-id="cf662-109">说明</span><span class="sxs-lookup"><span data-stu-id="cf662-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf662-110">Key</span><span class="sxs-lookup"><span data-stu-id="cf662-110">key</span></span>|<span data-ttu-id="cf662-111">String</span><span class="sxs-lookup"><span data-stu-id="cf662-111">String</span></span>|<span data-ttu-id="cf662-112">结果模板的 ID。</span><span class="sxs-lookup"><span data-stu-id="cf662-112">ID of a result template.</span></span> <span data-ttu-id="cf662-113">它必须映射到 [searchHit](searchhit.md)中的 **resultTemplateId。**</span><span class="sxs-lookup"><span data-stu-id="cf662-113">It must map to a **resultTemplateId** in the [searchHit](searchhit.md).</span></span>|
|<span data-ttu-id="cf662-114">displayName</span><span class="sxs-lookup"><span data-stu-id="cf662-114">displayName</span></span>|<span data-ttu-id="cf662-115">String</span><span class="sxs-lookup"><span data-stu-id="cf662-115">String</span></span>|<span data-ttu-id="cf662-116">结果模板的名称。</span><span class="sxs-lookup"><span data-stu-id="cf662-116">Name of the result template.</span></span>|
|<span data-ttu-id="cf662-117">body</span><span class="sxs-lookup"><span data-stu-id="cf662-117">body</span></span>|<span data-ttu-id="cf662-118">Json</span><span class="sxs-lookup"><span data-stu-id="cf662-118">Json</span></span>|<span data-ttu-id="cf662-119">结果模板的 JSON 架构。</span><span class="sxs-lookup"><span data-stu-id="cf662-119">JSON schema of the result template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf662-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf662-120">JSON representation</span></span>

<span data-ttu-id="cf662-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf662-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
  "resultTemplateId": {
                    "displayName": "String",
                    "body": "Json schema"
                }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


