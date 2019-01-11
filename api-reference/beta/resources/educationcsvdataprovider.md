---
title: educationCsvDataProvider 资源类型
description: '用于输入的源 CSV 文件时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb4d08a2a6750310a825f66ecfb0017abacd36fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878566"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="ff106-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff106-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="ff106-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff106-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff106-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff106-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff106-106">用于输入的源 CSV 文件时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="ff106-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="ff106-107">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="ff106-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ff106-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff106-108">Properties</span></span>

| <span data-ttu-id="ff106-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff106-109">Property</span></span> | <span data-ttu-id="ff106-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff106-110">Type</span></span> | <span data-ttu-id="ff106-111">Description</span><span class="sxs-lookup"><span data-stu-id="ff106-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ff106-112">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="ff106-112">**customizations**</span></span> | [<span data-ttu-id="ff106-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="ff106-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="ff106-114">可选自定义项应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="ff106-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff106-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff106-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
