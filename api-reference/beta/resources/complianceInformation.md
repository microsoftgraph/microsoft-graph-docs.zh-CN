---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b93e01bf6274591282fd5e486bebb878672d8cc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973228"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="52a1d-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="52a1d-103">complianceInformation resource type</span></span>

<span data-ttu-id="52a1d-104">包含与安全得分控制相关联的合规性数据。</span><span class="sxs-lookup"><span data-stu-id="52a1d-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="52a1d-105">属性</span><span class="sxs-lookup"><span data-stu-id="52a1d-105">Property</span></span> |<span data-ttu-id="52a1d-106">类型</span><span class="sxs-lookup"><span data-stu-id="52a1d-106">Type</span></span> |<span data-ttu-id="52a1d-107">说明</span><span class="sxs-lookup"><span data-stu-id="52a1d-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="52a1d-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="52a1d-108">certificationName</span></span> | <span data-ttu-id="52a1d-109">string</span><span class="sxs-lookup"><span data-stu-id="52a1d-109">string</span></span> | <span data-ttu-id="52a1d-110">合规性认证名称 (例如, ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="52a1d-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="52a1d-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="52a1d-111">certificationControls</span></span> | <span data-ttu-id="52a1d-112">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="52a1d-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="52a1d-113">与证书关联的证书控制的集合</span><span class="sxs-lookup"><span data-stu-id="52a1d-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52a1d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52a1d-114">JSON representation</span></span>

<span data-ttu-id="52a1d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52a1d-115">The following is a JSON representation of the resource.</span></span>

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
