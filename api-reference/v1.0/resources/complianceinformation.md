---
title: complianceInformation 资源类型
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ef62f6df73c24f9e6b3884921865c28ea152a3dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533037"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="b5eee-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5eee-103">complianceInformation resource type</span></span>

<span data-ttu-id="b5eee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5eee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5eee-105">包含与安全得分控制相关联的合规性数据。</span><span class="sxs-lookup"><span data-stu-id="b5eee-105">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="b5eee-106">属性</span><span class="sxs-lookup"><span data-stu-id="b5eee-106">Properties</span></span>

|<span data-ttu-id="b5eee-107">属性</span><span class="sxs-lookup"><span data-stu-id="b5eee-107">Property</span></span> |<span data-ttu-id="b5eee-108">类型</span><span class="sxs-lookup"><span data-stu-id="b5eee-108">Type</span></span> |<span data-ttu-id="b5eee-109">说明</span><span class="sxs-lookup"><span data-stu-id="b5eee-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="b5eee-110">certificationName</span><span class="sxs-lookup"><span data-stu-id="b5eee-110">certificationName</span></span>|<span data-ttu-id="b5eee-111">字符串</span><span class="sxs-lookup"><span data-stu-id="b5eee-111">String</span></span>| <span data-ttu-id="b5eee-112">合规性认证名称（例如，ISO 27018:2014、GDPR、FedRAMP、NIST 800-171）</span><span class="sxs-lookup"><span data-stu-id="b5eee-112">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="b5eee-113">certificationControls</span><span class="sxs-lookup"><span data-stu-id="b5eee-113">certificationControls</span></span>|<span data-ttu-id="b5eee-114">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="b5eee-114">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="b5eee-115">与证书关联的证书控制的集合</span><span class="sxs-lookup"><span data-stu-id="b5eee-115">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5eee-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5eee-116">JSON representation</span></span>

<span data-ttu-id="b5eee-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5eee-117">The following is a JSON representation of the resource.</span></span>

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
