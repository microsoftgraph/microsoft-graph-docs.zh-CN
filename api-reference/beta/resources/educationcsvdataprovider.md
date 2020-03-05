---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 207fee7f889c4369862918943371e2d629c8fab9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502170"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="33f38-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="33f38-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="33f38-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="33f38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33f38-105">用于在 CSV 文件为输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="33f38-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="33f38-106">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="33f38-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="33f38-107">属性</span><span class="sxs-lookup"><span data-stu-id="33f38-107">Properties</span></span>

| <span data-ttu-id="33f38-108">属性</span><span class="sxs-lookup"><span data-stu-id="33f38-108">Property</span></span> | <span data-ttu-id="33f38-109">类型</span><span class="sxs-lookup"><span data-stu-id="33f38-109">Type</span></span> | <span data-ttu-id="33f38-110">说明</span><span class="sxs-lookup"><span data-stu-id="33f38-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="33f38-111">**操作**</span><span class="sxs-lookup"><span data-stu-id="33f38-111">**customizations**</span></span> | [<span data-ttu-id="33f38-112">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="33f38-112">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="33f38-113">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="33f38-113">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33f38-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33f38-114">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
