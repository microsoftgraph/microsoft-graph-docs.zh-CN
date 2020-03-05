---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 65eda1c24fee112ef18fc6682b537f92f924dcf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507574"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="65877-103">complianceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="65877-103">complianceInformation resource type</span></span>

<span data-ttu-id="65877-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="65877-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65877-105">包含与安全得分控制相关联的合规性数据。</span><span class="sxs-lookup"><span data-stu-id="65877-105">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="65877-106">属性</span><span class="sxs-lookup"><span data-stu-id="65877-106">Property</span></span> |<span data-ttu-id="65877-107">类型</span><span class="sxs-lookup"><span data-stu-id="65877-107">Type</span></span> |<span data-ttu-id="65877-108">说明</span><span class="sxs-lookup"><span data-stu-id="65877-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="65877-109">certificationName</span><span class="sxs-lookup"><span data-stu-id="65877-109">certificationName</span></span> | <span data-ttu-id="65877-110">string</span><span class="sxs-lookup"><span data-stu-id="65877-110">string</span></span> | <span data-ttu-id="65877-111">合规性认证名称（例如，ISO 27018:2014、GDPR、FedRAMP、NIST 800-171）</span><span class="sxs-lookup"><span data-stu-id="65877-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="65877-112">certificationControls</span><span class="sxs-lookup"><span data-stu-id="65877-112">certificationControls</span></span> | <span data-ttu-id="65877-113">[certificationControl](certificationcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="65877-113">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="65877-114">与证书关联的证书控制的集合</span><span class="sxs-lookup"><span data-stu-id="65877-114">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65877-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65877-115">JSON representation</span></span>

<span data-ttu-id="65877-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65877-116">The following is a JSON representation of the resource.</span></span>

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
