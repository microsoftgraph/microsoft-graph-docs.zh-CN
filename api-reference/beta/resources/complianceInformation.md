---
title: " complianceInformation 资源类型"
description: 此资源包含合规性与关联数据安全分数控件。
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820599"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="3a59d-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a59d-103">complianceInformation resource type</span></span>

<span data-ttu-id="3a59d-104">包含合规性与关联数据安全分数控件。</span><span class="sxs-lookup"><span data-stu-id="3a59d-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="3a59d-105">属性</span><span class="sxs-lookup"><span data-stu-id="3a59d-105">Property</span></span> |<span data-ttu-id="3a59d-106">类型</span><span class="sxs-lookup"><span data-stu-id="3a59d-106">Type</span></span> |<span data-ttu-id="3a59d-107">Description</span><span class="sxs-lookup"><span data-stu-id="3a59d-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3a59d-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="3a59d-108">certificationName</span></span> | <span data-ttu-id="3a59d-109">string</span><span class="sxs-lookup"><span data-stu-id="3a59d-109">string</span></span> | <span data-ttu-id="3a59d-110">合规性证书名称 (如 ISO 27018:2014，GDPR FedRAMP、 NIST 800 171)</span><span class="sxs-lookup"><span data-stu-id="3a59d-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="3a59d-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="3a59d-111">certificationControls</span></span> | <span data-ttu-id="3a59d-112">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="3a59d-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="3a59d-113">与证书关联的证书控件集合</span><span class="sxs-lookup"><span data-stu-id="3a59d-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a59d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a59d-114">JSON representation</span></span>

<span data-ttu-id="3a59d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a59d-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
