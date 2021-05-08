---
title: detailsInfo 资源类型
description: 可以包含有关关联标识或系统的任何信息的属性包。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1841c513651131c4bf624c07ee117fae32df79f7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240763"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="01b52-103">detailsInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="01b52-103">detailsInfo resource type</span></span>

<span data-ttu-id="01b52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01b52-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01b52-105">可以包含有关关联标识或系统的任何信息的属性包。</span><span class="sxs-lookup"><span data-stu-id="01b52-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="01b52-106">这可能包括有关正在设置的属性或源/目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="01b52-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="01b52-107">属性</span><span class="sxs-lookup"><span data-stu-id="01b52-107">Properties</span></span>
<span data-ttu-id="01b52-108">**detailsInfo** 资源是一个 JSON 字符串，其中包含其他属性，如 **ApplicationId、ObjectId** 和 **UPN**。</span><span class="sxs-lookup"><span data-stu-id="01b52-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="01b52-109">属性集因所设置的资源类型而异。</span><span class="sxs-lookup"><span data-stu-id="01b52-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="01b52-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) 显示了这一点的示例。</span><span class="sxs-lookup"><span data-stu-id="01b52-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="01b52-111">关系</span><span class="sxs-lookup"><span data-stu-id="01b52-111">Relationships</span></span>
<span data-ttu-id="01b52-112">无</span><span class="sxs-lookup"><span data-stu-id="01b52-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01b52-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01b52-113">JSON Representation</span></span>
<span data-ttu-id="01b52-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01b52-114">Here is a JSON representation of the resource.</span></span>
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


