---
title: programControlType 资源类型
description: '在 Azure AD access 评论功能中，将控件与程序关联时使用程序控件类型，以指示控件所针对的访问评审的类型。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7321e4394e5e2a87d4ff51f71bc1589b5e1688cb
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125300"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="2c314-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c314-103">programControlType resource type</span></span>

<span data-ttu-id="2c314-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c314-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c314-105">在 Azure AD [access 评论](accessreviews-root.md)功能中，将控件与程序关联时使用程序控件类型，以指示控件所针对的访问评审的类型。</span><span class="sxs-lookup"><span data-stu-id="2c314-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="2c314-106">当全局管理员 onboards 租户使用访问评论功能时，将自动生成程序控制类型对象。</span><span class="sxs-lookup"><span data-stu-id="2c314-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="2c314-107">无法创建其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="2c314-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="2c314-108">方法</span><span class="sxs-lookup"><span data-stu-id="2c314-108">Methods</span></span>

| <span data-ttu-id="2c314-109">方法</span><span class="sxs-lookup"><span data-stu-id="2c314-109">Method</span></span>           | <span data-ttu-id="2c314-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c314-110">Return Type</span></span>    |<span data-ttu-id="2c314-111">说明</span><span class="sxs-lookup"><span data-stu-id="2c314-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c314-112">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="2c314-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="2c314-113">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c314-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="2c314-114">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="2c314-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c314-115">属性</span><span class="sxs-lookup"><span data-stu-id="2c314-115">Properties</span></span>
| <span data-ttu-id="2c314-116">属性</span><span class="sxs-lookup"><span data-stu-id="2c314-116">Property</span></span>     | <span data-ttu-id="2c314-117">类型</span><span class="sxs-lookup"><span data-stu-id="2c314-117">Type</span></span>   |<span data-ttu-id="2c314-118">说明</span><span class="sxs-lookup"><span data-stu-id="2c314-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="2c314-119">为程序控件类型分配的功能的标识符</span><span class="sxs-lookup"><span data-stu-id="2c314-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="2c314-120">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="2c314-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="2c314-121">关系</span><span class="sxs-lookup"><span data-stu-id="2c314-121">Relationships</span></span>

<span data-ttu-id="2c314-122">无。</span><span class="sxs-lookup"><span data-stu-id="2c314-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="2c314-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2c314-123">See also</span></span>

| <span data-ttu-id="2c314-124">方法</span><span class="sxs-lookup"><span data-stu-id="2c314-124">Method</span></span>           | <span data-ttu-id="2c314-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c314-125">Return Type</span></span>    |<span data-ttu-id="2c314-126">说明</span><span class="sxs-lookup"><span data-stu-id="2c314-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c314-127">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="2c314-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="2c314-128">programControl</span><span class="sxs-lookup"><span data-stu-id="2c314-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="2c314-129">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="2c314-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2c314-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c314-130">JSON representation</span></span>

<span data-ttu-id="2c314-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c314-131">Here is a JSON representation of the resource.</span></span>

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
