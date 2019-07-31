---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f515744f5206ea132531373e3df317e02dd6cbb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006400"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="3524d-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="3524d-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3524d-104">用于在 CSV 文件为输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="3524d-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="3524d-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="3524d-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3524d-106">属性</span><span class="sxs-lookup"><span data-stu-id="3524d-106">Properties</span></span>

| <span data-ttu-id="3524d-107">属性</span><span class="sxs-lookup"><span data-stu-id="3524d-107">Property</span></span> | <span data-ttu-id="3524d-108">类型</span><span class="sxs-lookup"><span data-stu-id="3524d-108">Type</span></span> | <span data-ttu-id="3524d-109">说明</span><span class="sxs-lookup"><span data-stu-id="3524d-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3524d-110">**操作**</span><span class="sxs-lookup"><span data-stu-id="3524d-110">**customizations**</span></span> | [<span data-ttu-id="3524d-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="3524d-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="3524d-112">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="3524d-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3524d-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3524d-113">JSON representation</span></span>

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
