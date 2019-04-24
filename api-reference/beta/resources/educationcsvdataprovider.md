---
title: educationCsvDataProvider 资源类型
description: '用于在 CSV 文件为输入源时设置学校数据同步配置文件。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507173"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="08419-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="08419-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08419-104">用于在 CSV 文件为输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="08419-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="08419-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="08419-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="08419-106">属性</span><span class="sxs-lookup"><span data-stu-id="08419-106">Properties</span></span>

| <span data-ttu-id="08419-107">属性</span><span class="sxs-lookup"><span data-stu-id="08419-107">Property</span></span> | <span data-ttu-id="08419-108">类型</span><span class="sxs-lookup"><span data-stu-id="08419-108">Type</span></span> | <span data-ttu-id="08419-109">说明</span><span class="sxs-lookup"><span data-stu-id="08419-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="08419-110">**操作**</span><span class="sxs-lookup"><span data-stu-id="08419-110">**customizations**</span></span> | [<span data-ttu-id="08419-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="08419-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="08419-112">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="08419-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08419-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08419-113">JSON representation</span></span>

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
