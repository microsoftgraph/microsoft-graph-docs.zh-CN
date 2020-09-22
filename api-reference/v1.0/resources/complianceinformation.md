---
title: complianceInformation 资源类型
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 00447f134b2c54bdda92857c6c84c05e8c52b3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018933"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="78f48-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="78f48-103">complianceInformation resource type</span></span>

<span data-ttu-id="78f48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78f48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78f48-105">包含与安全得分控制相关联的合规性数据。</span><span class="sxs-lookup"><span data-stu-id="78f48-105">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="78f48-106">属性</span><span class="sxs-lookup"><span data-stu-id="78f48-106">Properties</span></span>

|<span data-ttu-id="78f48-107">属性</span><span class="sxs-lookup"><span data-stu-id="78f48-107">Property</span></span> |<span data-ttu-id="78f48-108">类型</span><span class="sxs-lookup"><span data-stu-id="78f48-108">Type</span></span> |<span data-ttu-id="78f48-109">说明</span><span class="sxs-lookup"><span data-stu-id="78f48-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="78f48-110">certificationName</span><span class="sxs-lookup"><span data-stu-id="78f48-110">certificationName</span></span>|<span data-ttu-id="78f48-111">String</span><span class="sxs-lookup"><span data-stu-id="78f48-111">String</span></span>| <span data-ttu-id="78f48-112">合规性认证名称 (例如，ISO 27018:2014、GDPR、FedRAMP、NIST 800-171) </span><span class="sxs-lookup"><span data-stu-id="78f48-112">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="78f48-113">certificationControls</span><span class="sxs-lookup"><span data-stu-id="78f48-113">certificationControls</span></span>|<span data-ttu-id="78f48-114">[certificationControl](certificationcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f48-114">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="78f48-115">与证书关联的证书控制的集合</span><span class="sxs-lookup"><span data-stu-id="78f48-115">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78f48-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78f48-116">JSON representation</span></span>

<span data-ttu-id="78f48-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78f48-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

