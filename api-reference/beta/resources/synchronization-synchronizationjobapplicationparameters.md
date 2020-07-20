---
title: synchronizationJobApplicationParameters 资源类型
description: 表示要设置的对象以及在按需预配时执行的规则。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0f0b7cae5a3ce9c49ea64b603390ea65831144b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007153"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="516f1-103">synchronizationJobApplicationParameters 资源类型</span><span class="sxs-lookup"><span data-stu-id="516f1-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="516f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="516f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="516f1-105">表示将设置的对象和执行的同步规则。</span><span class="sxs-lookup"><span data-stu-id="516f1-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="516f1-106">资源主要用于按需预配。</span><span class="sxs-lookup"><span data-stu-id="516f1-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="516f1-107">属性</span><span class="sxs-lookup"><span data-stu-id="516f1-107">Properties</span></span>
|<span data-ttu-id="516f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="516f1-108">Property</span></span>|<span data-ttu-id="516f1-109">类型</span><span class="sxs-lookup"><span data-stu-id="516f1-109">Type</span></span>|<span data-ttu-id="516f1-110">说明</span><span class="sxs-lookup"><span data-stu-id="516f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="516f1-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="516f1-111">ruleId</span></span>|<span data-ttu-id="516f1-112">String</span><span class="sxs-lookup"><span data-stu-id="516f1-112">String</span></span>|<span data-ttu-id="516f1-113">要应用的 synchronizationRule 的标识符;对于具有单个 synchronizationRule 的 synchronizationJob 是可选的。</span><span class="sxs-lookup"><span data-stu-id="516f1-113">The identifier of a the synchronizationRule to be applied; optional for a synchronizationJob with a single synchronizationRule.</span></span>|
|<span data-ttu-id="516f1-114">聚焦</span><span class="sxs-lookup"><span data-stu-id="516f1-114">subjects</span></span>|<span data-ttu-id="516f1-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)集合</span><span class="sxs-lookup"><span data-stu-id="516f1-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="516f1-116">要应用 synchronizationJob 的一个或多个对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="516f1-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="516f1-117">关系</span><span class="sxs-lookup"><span data-stu-id="516f1-117">Relationships</span></span>
<span data-ttu-id="516f1-118">无。</span><span class="sxs-lookup"><span data-stu-id="516f1-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="516f1-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="516f1-119">JSON representation</span></span>
<span data-ttu-id="516f1-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="516f1-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobApplicationParameters",
  "ruleId": "String",
  "subjects": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```
