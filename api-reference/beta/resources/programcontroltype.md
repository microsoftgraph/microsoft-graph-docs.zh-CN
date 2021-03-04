---
title: programControlType 资源类型
description: '在 Azure AD 访问评审功能中，将控件与程序关联时，会使用程序控件类型，以指示控件用于的访问评审类型。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 593d8a8fa36c03515dbad9a1ee1dd0b267f98577
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443942"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="24758-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="24758-103">programControlType resource type</span></span>

<span data-ttu-id="24758-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24758-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24758-105">在 Azure AD 访问 [评审](accessreviews-root.md) 功能中，将控件关联到程序时，会使用程序控件类型来指示控件所针对的访问评审类型。</span><span class="sxs-lookup"><span data-stu-id="24758-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="24758-106">当全局管理员载入租户以使用访问评审功能时，将自动生成程序控制类型对象。</span><span class="sxs-lookup"><span data-stu-id="24758-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="24758-107">无法创建任何其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="24758-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="24758-108">Methods</span><span class="sxs-lookup"><span data-stu-id="24758-108">Methods</span></span>

| <span data-ttu-id="24758-109">方法</span><span class="sxs-lookup"><span data-stu-id="24758-109">Method</span></span>           | <span data-ttu-id="24758-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="24758-110">Return Type</span></span>    |<span data-ttu-id="24758-111">说明</span><span class="sxs-lookup"><span data-stu-id="24758-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24758-112">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="24758-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="24758-113">[programControlType](programcontroltype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24758-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="24758-114">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="24758-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="24758-115">属性</span><span class="sxs-lookup"><span data-stu-id="24758-115">Properties</span></span>
| <span data-ttu-id="24758-116">属性</span><span class="sxs-lookup"><span data-stu-id="24758-116">Property</span></span>     | <span data-ttu-id="24758-117">类型</span><span class="sxs-lookup"><span data-stu-id="24758-117">Type</span></span>   |<span data-ttu-id="24758-118">说明</span><span class="sxs-lookup"><span data-stu-id="24758-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="24758-119">程序控件类型的功能分配标识符</span><span class="sxs-lookup"><span data-stu-id="24758-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="24758-120">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="24758-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="24758-121">关系</span><span class="sxs-lookup"><span data-stu-id="24758-121">Relationships</span></span>

<span data-ttu-id="24758-122">无。</span><span class="sxs-lookup"><span data-stu-id="24758-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="24758-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="24758-123">See also</span></span>

| <span data-ttu-id="24758-124">方法</span><span class="sxs-lookup"><span data-stu-id="24758-124">Method</span></span>           | <span data-ttu-id="24758-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="24758-125">Return Type</span></span>    |<span data-ttu-id="24758-126">说明</span><span class="sxs-lookup"><span data-stu-id="24758-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24758-127">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="24758-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="24758-128">programControl</span><span class="sxs-lookup"><span data-stu-id="24758-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="24758-129">将 programControl 添加到程序。</span><span class="sxs-lookup"><span data-stu-id="24758-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="24758-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24758-130">JSON representation</span></span>

<span data-ttu-id="24758-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24758-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


