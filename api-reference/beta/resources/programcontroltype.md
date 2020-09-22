---
title: programControlType 资源类型
description: '在 Azure AD access 评论功能中，将控件与程序关联时使用程序控件类型，以指示控件所针对的访问评审的类型。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: ddf5ee29c01770d06c9725413f362bd0f0e18bee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029057"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="e51f6-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="e51f6-103">programControlType resource type</span></span>

<span data-ttu-id="e51f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e51f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e51f6-105">在 Azure AD [access 评论](accessreviews-root.md) 功能中，将控件与程序关联时使用程序控件类型，以指示控件所针对的访问评审的类型。</span><span class="sxs-lookup"><span data-stu-id="e51f6-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="e51f6-106">当全局管理员 onboards 租户使用访问评论功能时，将自动生成程序控制类型对象。</span><span class="sxs-lookup"><span data-stu-id="e51f6-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="e51f6-107">无法创建其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="e51f6-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="e51f6-108">方法</span><span class="sxs-lookup"><span data-stu-id="e51f6-108">Methods</span></span>

| <span data-ttu-id="e51f6-109">方法</span><span class="sxs-lookup"><span data-stu-id="e51f6-109">Method</span></span>           | <span data-ttu-id="e51f6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e51f6-110">Return Type</span></span>    |<span data-ttu-id="e51f6-111">说明</span><span class="sxs-lookup"><span data-stu-id="e51f6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e51f6-112">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="e51f6-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="e51f6-113">[programControlType](programcontroltype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e51f6-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="e51f6-114">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="e51f6-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="e51f6-115">属性</span><span class="sxs-lookup"><span data-stu-id="e51f6-115">Properties</span></span>
| <span data-ttu-id="e51f6-116">属性</span><span class="sxs-lookup"><span data-stu-id="e51f6-116">Property</span></span>     | <span data-ttu-id="e51f6-117">类型</span><span class="sxs-lookup"><span data-stu-id="e51f6-117">Type</span></span>   |<span data-ttu-id="e51f6-118">说明</span><span class="sxs-lookup"><span data-stu-id="e51f6-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="e51f6-119">为程序控件类型分配的功能的标识符</span><span class="sxs-lookup"><span data-stu-id="e51f6-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="e51f6-120">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="e51f6-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="e51f6-121">关系</span><span class="sxs-lookup"><span data-stu-id="e51f6-121">Relationships</span></span>

<span data-ttu-id="e51f6-122">无。</span><span class="sxs-lookup"><span data-stu-id="e51f6-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="e51f6-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e51f6-123">See also</span></span>

| <span data-ttu-id="e51f6-124">方法</span><span class="sxs-lookup"><span data-stu-id="e51f6-124">Method</span></span>           | <span data-ttu-id="e51f6-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="e51f6-125">Return Type</span></span>    |<span data-ttu-id="e51f6-126">说明</span><span class="sxs-lookup"><span data-stu-id="e51f6-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e51f6-127">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="e51f6-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="e51f6-128">programControl</span><span class="sxs-lookup"><span data-stu-id="e51f6-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="e51f6-129">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="e51f6-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e51f6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e51f6-130">JSON representation</span></span>

<span data-ttu-id="e51f6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e51f6-131">Here is a JSON representation of the resource.</span></span>

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


