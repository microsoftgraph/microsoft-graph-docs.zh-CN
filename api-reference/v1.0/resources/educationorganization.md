---
title: educationOrganization 资源类型
description: 用于模型之间的教育扇区中的不同组织类型通用性抽象实体。
ms.openlocfilehash: ed7a01072fe3adf00cb09082ad17954b9a921083
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008485"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="befbf-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="befbf-103">educationOrganization resource type</span></span>

<span data-ttu-id="befbf-104">用于模型之间的教育扇区中的不同组织类型通用性抽象实体。</span><span class="sxs-lookup"><span data-stu-id="befbf-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="befbf-105">属性</span><span class="sxs-lookup"><span data-stu-id="befbf-105">Properties</span></span>
| <span data-ttu-id="befbf-106">属性</span><span class="sxs-lookup"><span data-stu-id="befbf-106">Property</span></span>     | <span data-ttu-id="befbf-107">类型</span><span class="sxs-lookup"><span data-stu-id="befbf-107">Type</span></span>   |<span data-ttu-id="befbf-108">说明</span><span class="sxs-lookup"><span data-stu-id="befbf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="befbf-109">说明</span><span class="sxs-lookup"><span data-stu-id="befbf-109">description</span></span>|<span data-ttu-id="befbf-110">字符串</span><span class="sxs-lookup"><span data-stu-id="befbf-110">String</span></span>| <span data-ttu-id="befbf-111">组织说明。</span><span class="sxs-lookup"><span data-stu-id="befbf-111">Organization description.</span></span>|
|<span data-ttu-id="befbf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="befbf-112">displayName</span></span>|<span data-ttu-id="befbf-113">字符串</span><span class="sxs-lookup"><span data-stu-id="befbf-113">String</span></span>| <span data-ttu-id="befbf-114">组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="befbf-114">Organization display name.</span></span>|
|<span data-ttu-id="befbf-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="befbf-115">externalSource</span></span>|<span data-ttu-id="befbf-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="befbf-116">educationExternalSource</span></span>| <span data-ttu-id="befbf-117">从在其中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="befbf-117">Source where this organization was created from.</span></span> <span data-ttu-id="befbf-118">可能的值为： `sis`， `manual`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="befbf-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="befbf-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="befbf-119">Relationships</span></span>
<span data-ttu-id="befbf-120">无。</span><span class="sxs-lookup"><span data-stu-id="befbf-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="befbf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="befbf-121">JSON representation</span></span>

<span data-ttu-id="befbf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="befbf-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->