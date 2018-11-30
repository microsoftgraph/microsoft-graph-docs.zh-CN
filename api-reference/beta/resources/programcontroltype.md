---
title: programControlType 资源类型
description: '在 Azure AD 中访问审阅功能，为关联到程序，以指示类型的访问审阅控件控件时使用的程序控件类型。  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045454"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="1481f-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="1481f-103">programControlType resource type</span></span>

> <span data-ttu-id="1481f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1481f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1481f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1481f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1481f-106">在 Azure AD[访问审阅](accessreviews-root.md)功能中的程序控件类型用于将控件与程序相关联时指示的访问查看该控件的类型。</span><span class="sxs-lookup"><span data-stu-id="1481f-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="1481f-107">全局管理员 onboards 租户用于访问审阅功能时，将自动生成的程序控件类型对象。</span><span class="sxs-lookup"><span data-stu-id="1481f-107">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="1481f-108">可以不创建任何其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="1481f-108">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="1481f-109">方法</span><span class="sxs-lookup"><span data-stu-id="1481f-109">Methods</span></span>

| <span data-ttu-id="1481f-110">方法</span><span class="sxs-lookup"><span data-stu-id="1481f-110">Method</span></span>           | <span data-ttu-id="1481f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1481f-111">Return Type</span></span>    |<span data-ttu-id="1481f-112">说明</span><span class="sxs-lookup"><span data-stu-id="1481f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1481f-113">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="1481f-113">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="1481f-114">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="1481f-114">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="1481f-115">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="1481f-115">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="1481f-116">属性</span><span class="sxs-lookup"><span data-stu-id="1481f-116">Properties</span></span>
| <span data-ttu-id="1481f-117">属性</span><span class="sxs-lookup"><span data-stu-id="1481f-117">Property</span></span>     | <span data-ttu-id="1481f-118">类型</span><span class="sxs-lookup"><span data-stu-id="1481f-118">Type</span></span>   |<span data-ttu-id="1481f-119">说明</span><span class="sxs-lookup"><span data-stu-id="1481f-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="1481f-120">程序控件类型的功能指派的标识符</span><span class="sxs-lookup"><span data-stu-id="1481f-120">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="1481f-121">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="1481f-121">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="1481f-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="1481f-122">Relationships</span></span>

<span data-ttu-id="1481f-123">无。</span><span class="sxs-lookup"><span data-stu-id="1481f-123">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="1481f-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1481f-124">See also</span></span>

| <span data-ttu-id="1481f-125">方法</span><span class="sxs-lookup"><span data-stu-id="1481f-125">Method</span></span>           | <span data-ttu-id="1481f-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="1481f-126">Return Type</span></span>    |<span data-ttu-id="1481f-127">说明</span><span class="sxs-lookup"><span data-stu-id="1481f-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1481f-128">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="1481f-128">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="1481f-129">programControl</span><span class="sxs-lookup"><span data-stu-id="1481f-129">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="1481f-130">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="1481f-130">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1481f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1481f-131">JSON representation</span></span>

<span data-ttu-id="1481f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1481f-132">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
