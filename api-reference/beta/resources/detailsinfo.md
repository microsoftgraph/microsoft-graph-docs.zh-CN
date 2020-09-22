---
title: detailsInfo 资源类型
description: 可以包含有关关联的标识或系统的任何信息的属性包。
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c08dcb867f92bd65449be891bf0ae0e8a12a2459
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049870"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="c3617-103">detailsInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3617-103">detailsInfo resource type</span></span>

<span data-ttu-id="c3617-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3617-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3617-105">可以包含有关关联的标识或系统的任何信息的属性包。</span><span class="sxs-lookup"><span data-stu-id="c3617-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="c3617-106">这可能包括有关要预配的属性或源/目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c3617-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="c3617-107">属性</span><span class="sxs-lookup"><span data-stu-id="c3617-107">Properties</span></span>
<span data-ttu-id="c3617-108">**DetailsInfo**资源是一个 JSON 字符串，其中包含诸如**ApplicationId**、 **ObjectId**和**UPN**等其他属性。</span><span class="sxs-lookup"><span data-stu-id="c3617-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="c3617-109">属性集根据要设置的资源类型的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="c3617-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="c3617-110">[列表 provisioningObjectSummary](../api/provisioningobjectsummary-list.md) 显示了这种情况的示例。</span><span class="sxs-lookup"><span data-stu-id="c3617-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="c3617-111">关系</span><span class="sxs-lookup"><span data-stu-id="c3617-111">Relationships</span></span>
<span data-ttu-id="c3617-112">无</span><span class="sxs-lookup"><span data-stu-id="c3617-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3617-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3617-113">JSON Representation</span></span>
<span data-ttu-id="c3617-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3617-114">Here is a JSON representation of the resource.</span></span>
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


