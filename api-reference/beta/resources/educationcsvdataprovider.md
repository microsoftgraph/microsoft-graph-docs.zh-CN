---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60377b1761bcb5c672ae42f3067bb20d41325e9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095532"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="df655-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="df655-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="df655-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df655-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df655-105">用于在 CSV 文件为输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="df655-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>

<span data-ttu-id="df655-106">派生自 [educationSynchronizationDataProvider]。</span><span class="sxs-lookup"><span data-stu-id="df655-106">Derived from [educationSynchronizationDataProvider].</span></span>

## <a name="properties"></a><span data-ttu-id="df655-107">属性</span><span class="sxs-lookup"><span data-stu-id="df655-107">Properties</span></span>

| <span data-ttu-id="df655-108">属性</span><span class="sxs-lookup"><span data-stu-id="df655-108">Property</span></span>       | <span data-ttu-id="df655-109">类型</span><span class="sxs-lookup"><span data-stu-id="df655-109">Type</span></span>                                     | <span data-ttu-id="df655-110">说明</span><span class="sxs-lookup"><span data-stu-id="df655-110">Description</span></span>                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="df655-111">操作</span><span class="sxs-lookup"><span data-stu-id="df655-111">customizations</span></span> | <span data-ttu-id="df655-112">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="df655-112">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="df655-113">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="df655-113">Optional customizations to be applied to the synchronization profile.</span></span> |

[educationsynchronizationdataprovider]: educationsynchronizationdataprovider.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="df655-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df655-116">JSON representation</span></span>

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


