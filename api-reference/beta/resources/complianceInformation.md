---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543362"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="52f0f-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="52f0f-103">complianceInformation resource type</span></span>

<span data-ttu-id="52f0f-104">包含与安全得分控制相关联的合规性数据。</span><span class="sxs-lookup"><span data-stu-id="52f0f-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="52f0f-105">属性</span><span class="sxs-lookup"><span data-stu-id="52f0f-105">Property</span></span> |<span data-ttu-id="52f0f-106">类型</span><span class="sxs-lookup"><span data-stu-id="52f0f-106">Type</span></span> |<span data-ttu-id="52f0f-107">说明</span><span class="sxs-lookup"><span data-stu-id="52f0f-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="52f0f-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="52f0f-108">certificationName</span></span> | <span data-ttu-id="52f0f-109">string</span><span class="sxs-lookup"><span data-stu-id="52f0f-109">string</span></span> | <span data-ttu-id="52f0f-110">合规性认证名称 (例如, ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="52f0f-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="52f0f-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="52f0f-111">certificationControls</span></span> | <span data-ttu-id="52f0f-112">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="52f0f-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="52f0f-113">与证书关联的证书控制的集合</span><span class="sxs-lookup"><span data-stu-id="52f0f-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52f0f-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52f0f-114">JSON representation</span></span>

<span data-ttu-id="52f0f-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52f0f-115">The following is a JSON representation of the resource.</span></span>

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
