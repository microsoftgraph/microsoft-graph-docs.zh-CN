---
title: programControlType 资源类型
description: '在 Azure AD access 评论功能中, 将控件与程序关联时使用程序控件类型, 以指示控件所针对的访问评审的类型。  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563300"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="fc177-103">programControlType 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc177-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc177-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, 将控件与程序关联时使用程序控件类型, 以指示控件所针对的访问评审的类型。</span><span class="sxs-lookup"><span data-stu-id="fc177-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="fc177-105">当全局管理员 onboards 租户使用访问评论功能时, 将自动生成程序控制类型对象。</span><span class="sxs-lookup"><span data-stu-id="fc177-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="fc177-106">无法创建其他程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="fc177-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="fc177-107">方法</span><span class="sxs-lookup"><span data-stu-id="fc177-107">Methods</span></span>

| <span data-ttu-id="fc177-108">方法</span><span class="sxs-lookup"><span data-stu-id="fc177-108">Method</span></span>           | <span data-ttu-id="fc177-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fc177-109">Return Type</span></span>    |<span data-ttu-id="fc177-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc177-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc177-111">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="fc177-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="fc177-112">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc177-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="fc177-113">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="fc177-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc177-114">属性</span><span class="sxs-lookup"><span data-stu-id="fc177-114">Properties</span></span>
| <span data-ttu-id="fc177-115">属性</span><span class="sxs-lookup"><span data-stu-id="fc177-115">Property</span></span>     | <span data-ttu-id="fc177-116">类型</span><span class="sxs-lookup"><span data-stu-id="fc177-116">Type</span></span>   |<span data-ttu-id="fc177-117">说明</span><span class="sxs-lookup"><span data-stu-id="fc177-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="fc177-118">为程序控件类型分配的功能的标识符</span><span class="sxs-lookup"><span data-stu-id="fc177-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="fc177-119">程序控件类型的名称</span><span class="sxs-lookup"><span data-stu-id="fc177-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="fc177-120">关系</span><span class="sxs-lookup"><span data-stu-id="fc177-120">Relationships</span></span>

<span data-ttu-id="fc177-121">无。</span><span class="sxs-lookup"><span data-stu-id="fc177-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="fc177-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fc177-122">See also</span></span>

| <span data-ttu-id="fc177-123">方法</span><span class="sxs-lookup"><span data-stu-id="fc177-123">Method</span></span>           | <span data-ttu-id="fc177-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="fc177-124">Return Type</span></span>    |<span data-ttu-id="fc177-125">说明</span><span class="sxs-lookup"><span data-stu-id="fc177-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc177-126">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="fc177-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="fc177-127">programControl</span><span class="sxs-lookup"><span data-stu-id="fc177-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="fc177-128">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="fc177-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fc177-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc177-129">JSON representation</span></span>

<span data-ttu-id="fc177-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc177-130">Here is a JSON representation of the resource.</span></span>

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
