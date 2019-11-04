---
title: metadataAction 资源类型
description: 表示要写入或从文件中移除的元数据。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8652a33de04d0a28a34c3738dd1706d6aff5e5b9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938903"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="c3edd-103">metadataAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3edd-103">metadataAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3edd-104">表示要写入或从文件中移除的元数据。</span><span class="sxs-lookup"><span data-stu-id="c3edd-104">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="c3edd-105">**metadataAction**可能由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) api 返回。</span><span class="sxs-lookup"><span data-stu-id="c3edd-105">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="c3edd-106">该操作通知使用应用程序应添加到文件中的特定键/值对，或应从文件中删除的特定元数据密钥。</span><span class="sxs-lookup"><span data-stu-id="c3edd-106">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="c3edd-107">此元数据是描述要*标记*的文件或信息的内容。</span><span class="sxs-lookup"><span data-stu-id="c3edd-107">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="c3edd-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3edd-108">Properties</span></span>

| <span data-ttu-id="c3edd-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3edd-109">Property</span></span>         | <span data-ttu-id="c3edd-110">类型</span><span class="sxs-lookup"><span data-stu-id="c3edd-110">Type</span></span>                                       | <span data-ttu-id="c3edd-111">描述</span><span class="sxs-lookup"><span data-stu-id="c3edd-111">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="c3edd-112">metadataToAdd</span><span class="sxs-lookup"><span data-stu-id="c3edd-112">metadataToAdd</span></span>    | <span data-ttu-id="c3edd-113">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3edd-113">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="c3edd-114">应添加到文件中的键值对的集合。</span><span class="sxs-lookup"><span data-stu-id="c3edd-114">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="c3edd-115">metadataToRemove</span><span class="sxs-lookup"><span data-stu-id="c3edd-115">metadataToRemove</span></span> | <span data-ttu-id="c3edd-116">String collection</span><span class="sxs-lookup"><span data-stu-id="c3edd-116">String collection</span></span>                          | <span data-ttu-id="c3edd-117">字符串的集合，用于指示要从文件元数据中删除的键。</span><span class="sxs-lookup"><span data-stu-id="c3edd-117">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3edd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3edd-118">JSON representation</span></span>

<span data-ttu-id="c3edd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3edd-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "metadataToAdd": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "metadataToRemove": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->