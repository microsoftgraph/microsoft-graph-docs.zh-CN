---
title: serviceHealthIssuePost 资源类型
description: 表示服务运行状况问题的历史文章。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 910236d2059f951169bea314a0b38ae2516b1918
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107782"
---
# <a name="servicehealthissuepost-resource-type"></a><span data-ttu-id="29b5b-103">serviceHealthIssuePost 资源类型</span><span class="sxs-lookup"><span data-stu-id="29b5b-103">serviceHealthIssuePost resource type</span></span>

<span data-ttu-id="29b5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29b5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29b5b-105">表示服务运行状况问题 [中的历史文章](../resources/servicehealthissue.md)。</span><span class="sxs-lookup"><span data-stu-id="29b5b-105">Represents a historical post in a [service health issue](../resources/servicehealthissue.md).</span></span>

## <a name="properties"></a><span data-ttu-id="29b5b-106">属性</span><span class="sxs-lookup"><span data-stu-id="29b5b-106">Properties</span></span>
|<span data-ttu-id="29b5b-107">属性</span><span class="sxs-lookup"><span data-stu-id="29b5b-107">Property</span></span>|<span data-ttu-id="29b5b-108">类型</span><span class="sxs-lookup"><span data-stu-id="29b5b-108">Type</span></span>|<span data-ttu-id="29b5b-109">说明</span><span class="sxs-lookup"><span data-stu-id="29b5b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b5b-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29b5b-110">createdDateTime</span></span>|<span data-ttu-id="29b5b-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b5b-111">DateTimeOffset</span></span>|<span data-ttu-id="29b5b-112">文章的发布时间。</span><span class="sxs-lookup"><span data-stu-id="29b5b-112">The published time of the post.</span></span>|
|<span data-ttu-id="29b5b-113">description</span><span class="sxs-lookup"><span data-stu-id="29b5b-113">description</span></span>|[<span data-ttu-id="29b5b-114">itemBody</span><span class="sxs-lookup"><span data-stu-id="29b5b-114">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="29b5b-115">服务问题帖子的内容。</span><span class="sxs-lookup"><span data-stu-id="29b5b-115">The content of the service issue post.</span></span>|
|<span data-ttu-id="29b5b-116">postType</span><span class="sxs-lookup"><span data-stu-id="29b5b-116">postType</span></span>|<span data-ttu-id="29b5b-117">postType</span><span class="sxs-lookup"><span data-stu-id="29b5b-117">postType</span></span>|<span data-ttu-id="29b5b-118">服务问题历史文章的帖子类型。</span><span class="sxs-lookup"><span data-stu-id="29b5b-118">The post type of the service issue historical post.</span></span> <span data-ttu-id="29b5b-119">可取值为：`regular`、`quick`、`strategic`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="29b5b-119">Possible values are: `regular`, `quick`, `strategic`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29b5b-120">关系</span><span class="sxs-lookup"><span data-stu-id="29b5b-120">Relationships</span></span>
<span data-ttu-id="29b5b-121">无。</span><span class="sxs-lookup"><span data-stu-id="29b5b-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29b5b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29b5b-122">JSON representation</span></span>
<span data-ttu-id="29b5b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29b5b-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHealthIssuePost"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssuePost",
  "createdDateTime": "String (timestamp)",
  "postType": "String",
  "description": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

