---
title: synchronizationJobApplicationParameters 资源类型
description: 表示要设置的对象以及按需设置期间执行的规则。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2c17d67f766a398f94ab4962850a762fc62f6e53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133922"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="93fc5-103">synchronizationJobApplicationParameters 资源类型</span><span class="sxs-lookup"><span data-stu-id="93fc5-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="93fc5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93fc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93fc5-105">表示将设置的对象和执行同步规则。</span><span class="sxs-lookup"><span data-stu-id="93fc5-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="93fc5-106">资源主要用于按需预配。</span><span class="sxs-lookup"><span data-stu-id="93fc5-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="93fc5-107">属性</span><span class="sxs-lookup"><span data-stu-id="93fc5-107">Properties</span></span>
|<span data-ttu-id="93fc5-108">属性</span><span class="sxs-lookup"><span data-stu-id="93fc5-108">Property</span></span>|<span data-ttu-id="93fc5-109">类型</span><span class="sxs-lookup"><span data-stu-id="93fc5-109">Type</span></span>|<span data-ttu-id="93fc5-110">说明</span><span class="sxs-lookup"><span data-stu-id="93fc5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93fc5-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="93fc5-111">ruleId</span></span>|<span data-ttu-id="93fc5-112">字符串</span><span class="sxs-lookup"><span data-stu-id="93fc5-112">String</span></span>|<span data-ttu-id="93fc5-113">要应用的 synchronizationRule 的标识符。</span><span class="sxs-lookup"><span data-stu-id="93fc5-113">The identifier of a the synchronizationRule to be applied.</span></span>|
|<span data-ttu-id="93fc5-114">主题</span><span class="sxs-lookup"><span data-stu-id="93fc5-114">subjects</span></span>|<span data-ttu-id="93fc5-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93fc5-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="93fc5-116">要应用 synchronizationJob 的一个或多个对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="93fc5-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93fc5-117">关系</span><span class="sxs-lookup"><span data-stu-id="93fc5-117">Relationships</span></span>
<span data-ttu-id="93fc5-118">无。</span><span class="sxs-lookup"><span data-stu-id="93fc5-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93fc5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93fc5-119">JSON representation</span></span>
<span data-ttu-id="93fc5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93fc5-120">The following is a JSON representation of the resource.</span></span>
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


