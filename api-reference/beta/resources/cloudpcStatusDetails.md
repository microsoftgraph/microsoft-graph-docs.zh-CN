---
title: cloudPcStatusDetails 资源类型
description: 云电脑状态的详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61260bc7f3437fe1f10575afc616462eec2e47dc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563834"
---
# <a name="cloudpcstatusdetails-resource-type"></a><span data-ttu-id="6a7b9-103">cloudPcStatusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a7b9-103">cloudPcStatusDetails resource type</span></span>

<span data-ttu-id="6a7b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a7b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a7b9-105">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a7b9-105">The details of the cloud PC status.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="6a7b9-106">属性</span><span class="sxs-lookup"><span data-stu-id="6a7b9-106">Properties</span></span>

|<span data-ttu-id="6a7b9-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a7b9-107">Property</span></span>|<span data-ttu-id="6a7b9-108">类型</span><span class="sxs-lookup"><span data-stu-id="6a7b9-108">Type</span></span>|<span data-ttu-id="6a7b9-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a7b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7b9-110">code</span><span class="sxs-lookup"><span data-stu-id="6a7b9-110">code</span></span>|<span data-ttu-id="6a7b9-111">String</span><span class="sxs-lookup"><span data-stu-id="6a7b9-111">String</span></span>|<span data-ttu-id="6a7b9-112">与云电脑状态关联的代码。</span><span class="sxs-lookup"><span data-stu-id="6a7b9-112">The code associated with the cloud PC status.</span></span>|
|<span data-ttu-id="6a7b9-113">message</span><span class="sxs-lookup"><span data-stu-id="6a7b9-113">message</span></span>|<span data-ttu-id="6a7b9-114">String</span><span class="sxs-lookup"><span data-stu-id="6a7b9-114">String</span></span>|<span data-ttu-id="6a7b9-115">状态邮件。</span><span class="sxs-lookup"><span data-stu-id="6a7b9-115">The status message.</span></span>|
|<span data-ttu-id="6a7b9-116">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="6a7b9-116">additionalInformation</span></span>|<span data-ttu-id="6a7b9-117">[KeyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a7b9-117">[KeyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="6a7b9-118">有关云电脑状态的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="6a7b9-118">Any additional information about the cloud PC status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a7b9-119">关系</span><span class="sxs-lookup"><span data-stu-id="6a7b9-119">Relationships</span></span>

<span data-ttu-id="6a7b9-120">无。</span><span class="sxs-lookup"><span data-stu-id="6a7b9-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a7b9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a7b9-121">JSON representation</span></span>

<span data-ttu-id="6a7b9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a7b9-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcStatusDetails",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcStatusDetails",
  "code": "String",
  "message": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
