---
title: detailsInfo 资源类型
description: 可包含有关关联标识或系统的任何信息的属性包。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 25441071581af0b9e35ef941d8c82998bdea7b38
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135651"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="5b0c7-103">detailsInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b0c7-103">detailsInfo resource type</span></span>

<span data-ttu-id="5b0c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b0c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b0c7-105">可包含有关关联标识或系统的任何信息的属性包。</span><span class="sxs-lookup"><span data-stu-id="5b0c7-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="5b0c7-106">这可能包括有关要设置的属性或源/目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5b0c7-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="5b0c7-107">属性</span><span class="sxs-lookup"><span data-stu-id="5b0c7-107">Properties</span></span>
<span data-ttu-id="5b0c7-108">**detailsInfo** 资源是一个 JSON 字符串，其中包含其他属性，如 **ApplicationId、ObjectId** 和 **UPN。**</span><span class="sxs-lookup"><span data-stu-id="5b0c7-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="5b0c7-109">属性集因所设置的资源类型而异。</span><span class="sxs-lookup"><span data-stu-id="5b0c7-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="5b0c7-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) 显示了一个这样的示例。</span><span class="sxs-lookup"><span data-stu-id="5b0c7-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="5b0c7-111">关系</span><span class="sxs-lookup"><span data-stu-id="5b0c7-111">Relationships</span></span>
<span data-ttu-id="5b0c7-112">无</span><span class="sxs-lookup"><span data-stu-id="5b0c7-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b0c7-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b0c7-113">JSON Representation</span></span>
<span data-ttu-id="5b0c7-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b0c7-114">Here is a JSON representation of the resource.</span></span>
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


