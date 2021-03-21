---
title: programControlType 资源类型
description: '在 Azure AD 访问评审功能中，将控件关联到程序时，会使用程序控件类型来指示控件所针对的访问评审类型。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 58c9ee3ade6e3969de9653f54c5181a66f087ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960360"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="98ad6-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="98ad6-103">programControlType resource type</span></span>

<span data-ttu-id="98ad6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98ad6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98ad6-105">在 Azure [AD](accessreviews-root.md) 访问评审功能中，将控件关联到程序时，会使用程序控件类型来指示控件所针对的访问评审类型。</span><span class="sxs-lookup"><span data-stu-id="98ad6-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="98ad6-106">当全局管理员载入租户以使用访问评审功能时，将自动生成程序控制类型对象。</span><span class="sxs-lookup"><span data-stu-id="98ad6-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="98ad6-107">无法创建其他程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="98ad6-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="98ad6-108">Methods</span><span class="sxs-lookup"><span data-stu-id="98ad6-108">Methods</span></span>

| <span data-ttu-id="98ad6-109">方法</span><span class="sxs-lookup"><span data-stu-id="98ad6-109">Method</span></span>           | <span data-ttu-id="98ad6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="98ad6-110">Return Type</span></span>    |<span data-ttu-id="98ad6-111">说明</span><span class="sxs-lookup"><span data-stu-id="98ad6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98ad6-112">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="98ad6-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="98ad6-113">[programControlType](programcontroltype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98ad6-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="98ad6-114">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="98ad6-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="98ad6-115">属性</span><span class="sxs-lookup"><span data-stu-id="98ad6-115">Properties</span></span>
| <span data-ttu-id="98ad6-116">属性</span><span class="sxs-lookup"><span data-stu-id="98ad6-116">Property</span></span>     | <span data-ttu-id="98ad6-117">类型</span><span class="sxs-lookup"><span data-stu-id="98ad6-117">Type</span></span>   |<span data-ttu-id="98ad6-118">说明</span><span class="sxs-lookup"><span data-stu-id="98ad6-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="98ad6-119">id</span><span class="sxs-lookup"><span data-stu-id="98ad6-119">id</span></span>                     |<span data-ttu-id="98ad6-120">String</span><span class="sxs-lookup"><span data-stu-id="98ad6-120">String</span></span>                | <span data-ttu-id="98ad6-121">程序控件类型的功能分配的标识符</span><span class="sxs-lookup"><span data-stu-id="98ad6-121">The feature-assigned identifier of the program control type</span></span>                                      |
| <span data-ttu-id="98ad6-122">displayName</span><span class="sxs-lookup"><span data-stu-id="98ad6-122">displayName</span></span>            |<span data-ttu-id="98ad6-123">String</span><span class="sxs-lookup"><span data-stu-id="98ad6-123">String</span></span>                | <span data-ttu-id="98ad6-124">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="98ad6-124">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="98ad6-125">关系</span><span class="sxs-lookup"><span data-stu-id="98ad6-125">Relationships</span></span>

<span data-ttu-id="98ad6-126">无。</span><span class="sxs-lookup"><span data-stu-id="98ad6-126">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="98ad6-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="98ad6-127">See also</span></span>

| <span data-ttu-id="98ad6-128">方法</span><span class="sxs-lookup"><span data-stu-id="98ad6-128">Method</span></span>           | <span data-ttu-id="98ad6-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="98ad6-129">Return Type</span></span>    |<span data-ttu-id="98ad6-130">说明</span><span class="sxs-lookup"><span data-stu-id="98ad6-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98ad6-131">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="98ad6-131">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="98ad6-132">programControl</span><span class="sxs-lookup"><span data-stu-id="98ad6-132">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="98ad6-133">将 programControl 添加到程序。</span><span class="sxs-lookup"><span data-stu-id="98ad6-133">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="98ad6-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98ad6-134">JSON representation</span></span>

<span data-ttu-id="98ad6-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98ad6-135">Here is a JSON representation of the resource.</span></span>

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


