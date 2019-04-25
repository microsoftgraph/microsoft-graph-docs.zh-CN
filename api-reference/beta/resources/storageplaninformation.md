---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 05140b3256e434449d663c4992e74298bbdedd30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582090"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="a9c21-102">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9c21-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9c21-103">**storagePlanInformation**资源提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="a9c21-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="a9c21-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9c21-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a><span data-ttu-id="a9c21-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9c21-105">Properties</span></span>

| <span data-ttu-id="a9c21-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="a9c21-106">Property name</span></span>     | <span data-ttu-id="a9c21-107">类型</span><span class="sxs-lookup"><span data-stu-id="a9c21-107">Type</span></span>      | <span data-ttu-id="a9c21-108">说明</span><span class="sxs-lookup"><span data-stu-id="a9c21-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="a9c21-109">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="a9c21-109">upgradeAvailable</span></span>  | <span data-ttu-id="a9c21-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9c21-110">Boolean</span></span>   | <span data-ttu-id="a9c21-111">指示是否有更高的存储配额计划可用。</span><span class="sxs-lookup"><span data-stu-id="a9c21-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="a9c21-112">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c21-112">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": [
    "Error: /api-reference/beta/resources/storageplaninformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

