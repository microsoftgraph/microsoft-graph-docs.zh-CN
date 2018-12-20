---
title: " complianceInformation 资源类型"
description: 此资源包含合规性与关联数据安全分数控件。
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380957"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="f8e0e-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8e0e-103">complianceInformation resource type</span></span>

<span data-ttu-id="f8e0e-104">包含合规性与关联数据安全分数控件。</span><span class="sxs-lookup"><span data-stu-id="f8e0e-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="f8e0e-105">属性</span><span class="sxs-lookup"><span data-stu-id="f8e0e-105">Property</span></span> |<span data-ttu-id="f8e0e-106">类型</span><span class="sxs-lookup"><span data-stu-id="f8e0e-106">Type</span></span> |<span data-ttu-id="f8e0e-107">说明</span><span class="sxs-lookup"><span data-stu-id="f8e0e-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="f8e0e-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="f8e0e-108">certificationName</span></span> | <span data-ttu-id="f8e0e-109">string</span><span class="sxs-lookup"><span data-stu-id="f8e0e-109">string</span></span> | <span data-ttu-id="f8e0e-110">合规性证书名称 (如 ISO 27018:2014，GDPR FedRAMP、 NIST 800 171)</span><span class="sxs-lookup"><span data-stu-id="f8e0e-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="f8e0e-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="f8e0e-111">certificationControls</span></span> | <span data-ttu-id="f8e0e-112">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8e0e-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="f8e0e-113">与证书关联的证书控件集合</span><span class="sxs-lookup"><span data-stu-id="f8e0e-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8e0e-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8e0e-114">JSON representation</span></span>

<span data-ttu-id="f8e0e-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8e0e-115">The following is a JSON representation of the resource.</span></span>

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
