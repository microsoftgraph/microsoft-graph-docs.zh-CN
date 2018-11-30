---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
ms.openlocfilehash: 07552f405ec8c5d6ae8345a8238cd8aec3763b11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046481"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="ca111-102">storagePlanInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca111-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="ca111-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca111-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca111-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca111-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca111-105">**StoragePlanInformation**资源提供有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="ca111-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="ca111-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca111-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="ca111-107">属性</span><span class="sxs-lookup"><span data-stu-id="ca111-107">Properties</span></span>

| <span data-ttu-id="ca111-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="ca111-108">Property name</span></span>     | <span data-ttu-id="ca111-109">类型</span><span class="sxs-lookup"><span data-stu-id="ca111-109">Type</span></span>      | <span data-ttu-id="ca111-110">说明</span><span class="sxs-lookup"><span data-stu-id="ca111-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="ca111-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="ca111-111">upgradeAvailable</span></span>  | <span data-ttu-id="ca111-112">布尔</span><span class="sxs-lookup"><span data-stu-id="ca111-112">Boolean</span></span>   | <span data-ttu-id="ca111-113">指示是否有较高的存储配额规划可用。</span><span class="sxs-lookup"><span data-stu-id="ca111-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="ca111-114">只读。</span><span class="sxs-lookup"><span data-stu-id="ca111-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

