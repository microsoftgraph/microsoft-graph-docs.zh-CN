---
title: programControlType 资源类型
description: '在 Azure AD 中访问审阅功能，为关联到程序，以指示类型的访问审阅控件控件时使用的程序控件类型。  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519701"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="440c9-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="440c9-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="440c9-104">在 Azure AD[访问审阅](accessreviews-root.md)功能中的程序控件类型用于将控件与程序相关联时指示的访问查看该控件的类型。</span><span class="sxs-lookup"><span data-stu-id="440c9-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="440c9-105">全局管理员 onboards 租户用于访问审阅功能时，将自动生成的程序控件类型对象。</span><span class="sxs-lookup"><span data-stu-id="440c9-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="440c9-106">可以不创建任何其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="440c9-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="440c9-107">方法</span><span class="sxs-lookup"><span data-stu-id="440c9-107">Methods</span></span>

| <span data-ttu-id="440c9-108">方法</span><span class="sxs-lookup"><span data-stu-id="440c9-108">Method</span></span>           | <span data-ttu-id="440c9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="440c9-109">Return Type</span></span>    |<span data-ttu-id="440c9-110">说明</span><span class="sxs-lookup"><span data-stu-id="440c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="440c9-111">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="440c9-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="440c9-112">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="440c9-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="440c9-113">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="440c9-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="440c9-114">属性</span><span class="sxs-lookup"><span data-stu-id="440c9-114">Properties</span></span>
| <span data-ttu-id="440c9-115">属性</span><span class="sxs-lookup"><span data-stu-id="440c9-115">Property</span></span>     | <span data-ttu-id="440c9-116">类型</span><span class="sxs-lookup"><span data-stu-id="440c9-116">Type</span></span>   |<span data-ttu-id="440c9-117">说明</span><span class="sxs-lookup"><span data-stu-id="440c9-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="440c9-118">程序控件类型的功能指派的标识符</span><span class="sxs-lookup"><span data-stu-id="440c9-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="440c9-119">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="440c9-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="440c9-120">关系</span><span class="sxs-lookup"><span data-stu-id="440c9-120">Relationships</span></span>

<span data-ttu-id="440c9-121">无。</span><span class="sxs-lookup"><span data-stu-id="440c9-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="440c9-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="440c9-122">See also</span></span>

| <span data-ttu-id="440c9-123">方法</span><span class="sxs-lookup"><span data-stu-id="440c9-123">Method</span></span>           | <span data-ttu-id="440c9-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="440c9-124">Return Type</span></span>    |<span data-ttu-id="440c9-125">说明</span><span class="sxs-lookup"><span data-stu-id="440c9-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="440c9-126">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="440c9-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="440c9-127">programControl</span><span class="sxs-lookup"><span data-stu-id="440c9-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="440c9-128">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="440c9-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="440c9-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="440c9-129">JSON representation</span></span>

<span data-ttu-id="440c9-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="440c9-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontroltype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
