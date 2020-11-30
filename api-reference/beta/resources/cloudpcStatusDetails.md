---
title: cloudPcStatusDetails 资源类型
description: 云电脑状态的详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 647c13878e054fbac6c1f43f565bd2788d19a9de
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378327"
---
# <a name="cloudpcstatusdetails-resource-type"></a><span data-ttu-id="9779b-103">cloudPcStatusDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="9779b-103">cloudPcStatusDetails resource type</span></span>

<span data-ttu-id="9779b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9779b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9779b-105">云电脑状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9779b-105">The details of the cloud PC status.</span></span>

## <a name="properties"></a><span data-ttu-id="9779b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9779b-106">Properties</span></span>

|<span data-ttu-id="9779b-107">属性</span><span class="sxs-lookup"><span data-stu-id="9779b-107">Property</span></span>|<span data-ttu-id="9779b-108">类型</span><span class="sxs-lookup"><span data-stu-id="9779b-108">Type</span></span>|<span data-ttu-id="9779b-109">说明</span><span class="sxs-lookup"><span data-stu-id="9779b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9779b-110">code</span><span class="sxs-lookup"><span data-stu-id="9779b-110">code</span></span>|<span data-ttu-id="9779b-111">字符串</span><span class="sxs-lookup"><span data-stu-id="9779b-111">String</span></span>|<span data-ttu-id="9779b-112">与云电脑状态关联的代码。</span><span class="sxs-lookup"><span data-stu-id="9779b-112">The code associated with the cloud PC status.</span></span>|
|<span data-ttu-id="9779b-113">message</span><span class="sxs-lookup"><span data-stu-id="9779b-113">message</span></span>|<span data-ttu-id="9779b-114">String</span><span class="sxs-lookup"><span data-stu-id="9779b-114">String</span></span>|<span data-ttu-id="9779b-115">状态邮件。</span><span class="sxs-lookup"><span data-stu-id="9779b-115">The status message.</span></span>|
|<span data-ttu-id="9779b-116">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="9779b-116">additionalInformation</span></span>|<span data-ttu-id="9779b-117">[KeyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9779b-117">[KeyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="9779b-118">有关云电脑状态的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="9779b-118">Any additional information about the cloud PC status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9779b-119">关系</span><span class="sxs-lookup"><span data-stu-id="9779b-119">Relationships</span></span>

<span data-ttu-id="9779b-120">无。</span><span class="sxs-lookup"><span data-stu-id="9779b-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9779b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9779b-121">JSON representation</span></span>

<span data-ttu-id="9779b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9779b-122">The following is a JSON representation of the resource.</span></span>
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
