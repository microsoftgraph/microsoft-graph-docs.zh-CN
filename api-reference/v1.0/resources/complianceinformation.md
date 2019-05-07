---
title: complianceInformation 资源类型
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 85fef478a8dcc0f3196355d89f0a20ef0cd7a5b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629304"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="89627-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="89627-103">complianceInformation resource type</span></span>

<span data-ttu-id="89627-104">包含与安全得分控制相关联的合规性数据。</span><span class="sxs-lookup"><span data-stu-id="89627-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="89627-105">属性</span><span class="sxs-lookup"><span data-stu-id="89627-105">Properties</span></span>

|<span data-ttu-id="89627-106">属性</span><span class="sxs-lookup"><span data-stu-id="89627-106">Property</span></span> |<span data-ttu-id="89627-107">类型</span><span class="sxs-lookup"><span data-stu-id="89627-107">Type</span></span> |<span data-ttu-id="89627-108">说明</span><span class="sxs-lookup"><span data-stu-id="89627-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="89627-109">certificationName</span><span class="sxs-lookup"><span data-stu-id="89627-109">certificationName</span></span>|<span data-ttu-id="89627-110">字符串</span><span class="sxs-lookup"><span data-stu-id="89627-110">String</span></span>| <span data-ttu-id="89627-111">合规性认证名称 (例如, ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)</span><span class="sxs-lookup"><span data-stu-id="89627-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="89627-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="89627-112">certificationControls</span></span>|<span data-ttu-id="89627-113">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="89627-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="89627-114">与证书关联的证书控制的集合</span><span class="sxs-lookup"><span data-stu-id="89627-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89627-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89627-115">JSON representation</span></span>

<span data-ttu-id="89627-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89627-116">The following is a JSON representation of the resource.</span></span>

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
