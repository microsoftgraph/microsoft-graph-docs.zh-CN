---
title: educationCsvDataProvider 资源类型
description: '用于输入的源 CSV 文件时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529871"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="2c2d9-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c2d9-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c2d9-104">用于输入的源 CSV 文件时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="2c2d9-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="2c2d9-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="2c2d9-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c2d9-106">属性</span><span class="sxs-lookup"><span data-stu-id="2c2d9-106">Properties</span></span>

| <span data-ttu-id="2c2d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c2d9-107">Property</span></span> | <span data-ttu-id="2c2d9-108">类型</span><span class="sxs-lookup"><span data-stu-id="2c2d9-108">Type</span></span> | <span data-ttu-id="2c2d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="2c2d9-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2c2d9-110">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="2c2d9-110">**customizations**</span></span> | [<span data-ttu-id="2c2d9-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="2c2d9-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="2c2d9-112">可选自定义项应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="2c2d9-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c2d9-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c2d9-113">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcsvdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
