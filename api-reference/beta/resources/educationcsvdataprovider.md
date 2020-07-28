---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33cb0268eeb8c6d6b896dfb8ab02f7bb59b00e98
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434982"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="38853-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="38853-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="38853-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38853-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38853-105">用于在 CSV 文件为输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="38853-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>

<span data-ttu-id="38853-106">派生自[educationSynchronizationDataProvider]。</span><span class="sxs-lookup"><span data-stu-id="38853-106">Derived from [educationSynchronizationDataProvider].</span></span>

## <a name="properties"></a><span data-ttu-id="38853-107">属性</span><span class="sxs-lookup"><span data-stu-id="38853-107">Properties</span></span>

| <span data-ttu-id="38853-108">属性</span><span class="sxs-lookup"><span data-stu-id="38853-108">Property</span></span>       | <span data-ttu-id="38853-109">类型</span><span class="sxs-lookup"><span data-stu-id="38853-109">Type</span></span>                                     | <span data-ttu-id="38853-110">说明</span><span class="sxs-lookup"><span data-stu-id="38853-110">Description</span></span>                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="38853-111">操作</span><span class="sxs-lookup"><span data-stu-id="38853-111">customizations</span></span> | <span data-ttu-id="38853-112">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="38853-112">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="38853-113">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="38853-113">Optional customizations to be applied to the synchronization profile.</span></span> |

[educationsynchronizationdataprovider]: educationsynchronizationdataprovider.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="38853-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38853-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationCsvDataProvider",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```
