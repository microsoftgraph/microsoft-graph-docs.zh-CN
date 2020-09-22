---
title: metadataAction 资源类型
description: 表示要写入或从文件中移除的元数据。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55ddd644428662f6a646fd9c003761ab6f7c1e9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021383"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="71d77-103">metadataAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="71d77-103">metadataAction resource type</span></span>

<span data-ttu-id="71d77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71d77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71d77-105">表示要写入或从文件中移除的元数据。</span><span class="sxs-lookup"><span data-stu-id="71d77-105">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="71d77-106">**metadataAction** 可能由 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) api 返回。</span><span class="sxs-lookup"><span data-stu-id="71d77-106">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="71d77-107">该操作通知使用应用程序应添加到文件中的特定键/值对，或应从文件中删除的特定元数据密钥。</span><span class="sxs-lookup"><span data-stu-id="71d77-107">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="71d77-108">此元数据是描述要 *标记*的文件或信息的内容。</span><span class="sxs-lookup"><span data-stu-id="71d77-108">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="71d77-109">属性</span><span class="sxs-lookup"><span data-stu-id="71d77-109">Properties</span></span>

| <span data-ttu-id="71d77-110">属性</span><span class="sxs-lookup"><span data-stu-id="71d77-110">Property</span></span>         | <span data-ttu-id="71d77-111">类型</span><span class="sxs-lookup"><span data-stu-id="71d77-111">Type</span></span>                                       | <span data-ttu-id="71d77-112">说明</span><span class="sxs-lookup"><span data-stu-id="71d77-112">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="71d77-113">metadataToAdd</span><span class="sxs-lookup"><span data-stu-id="71d77-113">metadataToAdd</span></span>    | <span data-ttu-id="71d77-114">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71d77-114">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="71d77-115">应添加到文件中的键值对的集合。</span><span class="sxs-lookup"><span data-stu-id="71d77-115">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="71d77-116">metadataToRemove</span><span class="sxs-lookup"><span data-stu-id="71d77-116">metadataToRemove</span></span> | <span data-ttu-id="71d77-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="71d77-117">String collection</span></span>                          | <span data-ttu-id="71d77-118">字符串的集合，用于指示要从文件元数据中删除的键。</span><span class="sxs-lookup"><span data-stu-id="71d77-118">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71d77-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71d77-119">JSON representation</span></span>

<span data-ttu-id="71d77-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71d77-120">The following is a JSON representation of the resource.</span></span>

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

