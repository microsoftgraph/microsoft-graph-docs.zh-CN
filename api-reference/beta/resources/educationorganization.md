---
title: educationOrganization 资源类型
description: '用于模型之间的教育扇区中的不同组织类型通用性抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1e3f82e2d777b1d32cc445f543e7beed570a8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949519"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="edc94-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="edc94-103">educationOrganization resource type</span></span>

> <span data-ttu-id="edc94-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="edc94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edc94-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="edc94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="edc94-106">用于模型之间的教育扇区中的不同组织类型通用性抽象实体。</span><span class="sxs-lookup"><span data-stu-id="edc94-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="edc94-107">属性</span><span class="sxs-lookup"><span data-stu-id="edc94-107">Properties</span></span>
| <span data-ttu-id="edc94-108">属性</span><span class="sxs-lookup"><span data-stu-id="edc94-108">Property</span></span>     | <span data-ttu-id="edc94-109">类型</span><span class="sxs-lookup"><span data-stu-id="edc94-109">Type</span></span>   |<span data-ttu-id="edc94-110">说明</span><span class="sxs-lookup"><span data-stu-id="edc94-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edc94-111">说明</span><span class="sxs-lookup"><span data-stu-id="edc94-111">description</span></span>|<span data-ttu-id="edc94-112">字符串</span><span class="sxs-lookup"><span data-stu-id="edc94-112">String</span></span>| <span data-ttu-id="edc94-113">组织说明。</span><span class="sxs-lookup"><span data-stu-id="edc94-113">Organization description.</span></span>|
|<span data-ttu-id="edc94-114">displayName</span><span class="sxs-lookup"><span data-stu-id="edc94-114">displayName</span></span>|<span data-ttu-id="edc94-115">字符串</span><span class="sxs-lookup"><span data-stu-id="edc94-115">String</span></span>| <span data-ttu-id="edc94-116">组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="edc94-116">Organization display name.</span></span>|
|<span data-ttu-id="edc94-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="edc94-117">externalSource</span></span>|<span data-ttu-id="edc94-118">string</span><span class="sxs-lookup"><span data-stu-id="edc94-118">string</span></span>| <span data-ttu-id="edc94-119">从在其中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="edc94-119">Source where this organization was created from.</span></span> <span data-ttu-id="edc94-120">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="edc94-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edc94-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="edc94-121">Relationships</span></span>
<span data-ttu-id="edc94-122">无。</span><span class="sxs-lookup"><span data-stu-id="edc94-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="edc94-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edc94-123">JSON representation</span></span>

<span data-ttu-id="edc94-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc94-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
