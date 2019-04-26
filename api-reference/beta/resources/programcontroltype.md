---
title: programControlType 资源类型
description: '在 Azure AD access 评论功能中, 将控件与程序关联时使用程序控件类型, 以指示控件所针对的访问评审的类型。  '
localization_priority: Normal
ms.openlocfilehash: 489fa6e5cac31165fec9f7ce9939d58fa84cb1ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344042"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="5c3b6-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c3b6-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c3b6-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, 将控件与程序关联时使用程序控件类型, 以指示控件所针对的访问评审的类型。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="5c3b6-105">当全局管理员 onboards 租户使用访问评论功能时, 将自动生成程序控制类型对象。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="5c3b6-106">无法创建其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="5c3b6-107">方法</span><span class="sxs-lookup"><span data-stu-id="5c3b6-107">Methods</span></span>

| <span data-ttu-id="5c3b6-108">方法</span><span class="sxs-lookup"><span data-stu-id="5c3b6-108">Method</span></span>           | <span data-ttu-id="5c3b6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c3b6-109">Return Type</span></span>    |<span data-ttu-id="5c3b6-110">说明</span><span class="sxs-lookup"><span data-stu-id="5c3b6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c3b6-111">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="5c3b6-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="5c3b6-112">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c3b6-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="5c3b6-113">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c3b6-114">属性</span><span class="sxs-lookup"><span data-stu-id="5c3b6-114">Properties</span></span>
| <span data-ttu-id="5c3b6-115">属性</span><span class="sxs-lookup"><span data-stu-id="5c3b6-115">Property</span></span>     | <span data-ttu-id="5c3b6-116">类型</span><span class="sxs-lookup"><span data-stu-id="5c3b6-116">Type</span></span>   |<span data-ttu-id="5c3b6-117">说明</span><span class="sxs-lookup"><span data-stu-id="5c3b6-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="5c3b6-118">为程序控件类型分配的功能的标识符</span><span class="sxs-lookup"><span data-stu-id="5c3b6-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="5c3b6-119">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="5c3b6-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="5c3b6-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="5c3b6-120">Relationships</span></span>

<span data-ttu-id="5c3b6-121">无。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="5c3b6-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5c3b6-122">See also</span></span>

| <span data-ttu-id="5c3b6-123">方法</span><span class="sxs-lookup"><span data-stu-id="5c3b6-123">Method</span></span>           | <span data-ttu-id="5c3b6-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c3b6-124">Return Type</span></span>    |<span data-ttu-id="5c3b6-125">说明</span><span class="sxs-lookup"><span data-stu-id="5c3b6-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c3b6-126">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="5c3b6-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="5c3b6-127">programControl</span><span class="sxs-lookup"><span data-stu-id="5c3b6-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="5c3b6-128">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5c3b6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c3b6-129">JSON representation</span></span>

<span data-ttu-id="5c3b6-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c3b6-130">Here is a JSON representation of the resource.</span></span>

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
