---
title: detailsInfo 资源类型
description: 可以包含有关关联的标识或系统的任何信息的属性包。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349340"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="fe9f9-103">detailsInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe9f9-103">detailsInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe9f9-104">可以包含有关关联的标识或系统的任何信息的属性包。</span><span class="sxs-lookup"><span data-stu-id="fe9f9-104">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="fe9f9-105">这可能包括有关要预配的属性或源/目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fe9f9-105">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="fe9f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="fe9f9-106">Properties</span></span>
<span data-ttu-id="fe9f9-107">**DetailsInfo**资源是一个 JSON 字符串, 其中包含诸如**ApplicationId**、 **ObjectId**和**UPN**等其他属性。</span><span class="sxs-lookup"><span data-stu-id="fe9f9-107">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="fe9f9-108">属性集根据要设置的资源类型的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="fe9f9-108">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="fe9f9-109">[列表 provisioningObjectSummary](../api/provisioningobjectsummary-list.md)显示了这种情况的示例。</span><span class="sxs-lookup"><span data-stu-id="fe9f9-109">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="fe9f9-110">关系</span><span class="sxs-lookup"><span data-stu-id="fe9f9-110">Relationships</span></span>
<span data-ttu-id="fe9f9-111">无</span><span class="sxs-lookup"><span data-stu-id="fe9f9-111">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe9f9-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe9f9-112">JSON Representation</span></span>
<span data-ttu-id="fe9f9-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe9f9-113">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```
