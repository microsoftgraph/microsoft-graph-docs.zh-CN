---
title: businessFlowTemplate 资源类型
description: 在 Azure AD access 评论功能中, `businesFlowTemplate`表示 azure ad 业务流模板。 模板的标识符 (如审阅组的来宾成员) 是由呼叫者在创建访问评审时提供的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6890ed724c1a71c69a881ce0e2e70675b3537520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973487"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="b26f4-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="b26f4-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b26f4-105">在 Azure AD [access 评论](accessreviews-root.md)功能中, `businesFlowTemplate`表示 azure ad 业务流模板。</span><span class="sxs-lookup"><span data-stu-id="b26f4-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="b26f4-106">模板的标识符 (如审阅组的来宾成员) 是由呼叫者在创建访问评审时提供的。</span><span class="sxs-lookup"><span data-stu-id="b26f4-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="b26f4-107">当全局管理员 onboards 租户使用访问评论功能时, 将自动生成业务流模板对象。</span><span class="sxs-lookup"><span data-stu-id="b26f4-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="b26f4-108">无法创建其他业务流模板。</span><span class="sxs-lookup"><span data-stu-id="b26f4-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="b26f4-109">方法</span><span class="sxs-lookup"><span data-stu-id="b26f4-109">Methods</span></span>

| <span data-ttu-id="b26f4-110">方法</span><span class="sxs-lookup"><span data-stu-id="b26f4-110">Method</span></span>           | <span data-ttu-id="b26f4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b26f4-111">Return Type</span></span>    |<span data-ttu-id="b26f4-112">说明</span><span class="sxs-lookup"><span data-stu-id="b26f4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b26f4-113">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="b26f4-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="b26f4-114">[businessFlowTemplate](businessflowtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="b26f4-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="b26f4-115">获取适用于访问评审的业务流模板。</span><span class="sxs-lookup"><span data-stu-id="b26f4-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="b26f4-116">属性</span><span class="sxs-lookup"><span data-stu-id="b26f4-116">Properties</span></span>
| <span data-ttu-id="b26f4-117">属性</span><span class="sxs-lookup"><span data-stu-id="b26f4-117">Property</span></span>     | <span data-ttu-id="b26f4-118">类型</span><span class="sxs-lookup"><span data-stu-id="b26f4-118">Type</span></span>   |<span data-ttu-id="b26f4-119">说明</span><span class="sxs-lookup"><span data-stu-id="b26f4-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="b26f4-120">为业务流模板分配的功能的标识符</span><span class="sxs-lookup"><span data-stu-id="b26f4-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="b26f4-121">业务流模板的名称</span><span class="sxs-lookup"><span data-stu-id="b26f4-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="b26f4-122">关系</span><span class="sxs-lookup"><span data-stu-id="b26f4-122">Relationships</span></span>

<span data-ttu-id="b26f4-123">无。</span><span class="sxs-lookup"><span data-stu-id="b26f4-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="b26f4-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b26f4-124">See also</span></span>

| <span data-ttu-id="b26f4-125">方法</span><span class="sxs-lookup"><span data-stu-id="b26f4-125">Method</span></span>           | <span data-ttu-id="b26f4-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="b26f4-126">Return Type</span></span>    |<span data-ttu-id="b26f4-127">说明</span><span class="sxs-lookup"><span data-stu-id="b26f4-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b26f4-128">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="b26f4-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="b26f4-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="b26f4-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="b26f4-130">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="b26f4-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b26f4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b26f4-131">JSON representation</span></span>

<span data-ttu-id="b26f4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b26f4-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
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
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
