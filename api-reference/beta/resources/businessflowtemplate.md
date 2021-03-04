---
title: businessFlowTemplate 资源类型
description: 在 Azure AD 访问评审功能中，表示 `businesFlowTemplate` Azure AD 业务流程模板。 模板的标识符（如查看组的来宾成员）由调用方在创建访问评审时提供。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 95a2723ee20777989ed1576d02c69adc649555ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433143"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="be81d-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="be81d-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="be81d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be81d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be81d-106">在 Azure AD [访问评审](accessreviews-root.md) 功能中，表示 `businesFlowTemplate` Azure AD 业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="be81d-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="be81d-107">模板的标识符（如查看组的来宾成员）由调用方在创建访问评审时提供。</span><span class="sxs-lookup"><span data-stu-id="be81d-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="be81d-108">当全局管理员载入租户以使用访问评审功能时，将自动生成业务流程模板对象。</span><span class="sxs-lookup"><span data-stu-id="be81d-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="be81d-109">业务流程模板包括对应用程序的分配的访问评审、组的成员身份、Azure AD 角色的成员身份、组的来宾用户成员身份以及向应用程序分配的来宾用户分配。</span><span class="sxs-lookup"><span data-stu-id="be81d-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="be81d-110">无法创建任何其他业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="be81d-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="be81d-111">Methods</span><span class="sxs-lookup"><span data-stu-id="be81d-111">Methods</span></span>

| <span data-ttu-id="be81d-112">方法</span><span class="sxs-lookup"><span data-stu-id="be81d-112">Method</span></span>           | <span data-ttu-id="be81d-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="be81d-113">Return Type</span></span>    |<span data-ttu-id="be81d-114">说明</span><span class="sxs-lookup"><span data-stu-id="be81d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be81d-115">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="be81d-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="be81d-116">[businessFlowTemplate](businessflowtemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be81d-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="be81d-117">获取适合访问评价的业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="be81d-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="be81d-118">属性</span><span class="sxs-lookup"><span data-stu-id="be81d-118">Properties</span></span>
| <span data-ttu-id="be81d-119">属性</span><span class="sxs-lookup"><span data-stu-id="be81d-119">Property</span></span>     | <span data-ttu-id="be81d-120">类型</span><span class="sxs-lookup"><span data-stu-id="be81d-120">Type</span></span>   |<span data-ttu-id="be81d-121">说明</span><span class="sxs-lookup"><span data-stu-id="be81d-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="be81d-122">业务流程模板的功能分配标识符。</span><span class="sxs-lookup"><span data-stu-id="be81d-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="be81d-123">这些值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="be81d-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="be81d-124">业务流程模板的名称</span><span class="sxs-lookup"><span data-stu-id="be81d-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="be81d-125">关系</span><span class="sxs-lookup"><span data-stu-id="be81d-125">Relationships</span></span>

<span data-ttu-id="be81d-126">无。</span><span class="sxs-lookup"><span data-stu-id="be81d-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="be81d-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="be81d-127">See also</span></span>

| <span data-ttu-id="be81d-128">方法</span><span class="sxs-lookup"><span data-stu-id="be81d-128">Method</span></span>           | <span data-ttu-id="be81d-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="be81d-129">Return Type</span></span>    |<span data-ttu-id="be81d-130">说明</span><span class="sxs-lookup"><span data-stu-id="be81d-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be81d-131">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="be81d-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="be81d-132">accessReview</span><span class="sxs-lookup"><span data-stu-id="be81d-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="be81d-133">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="be81d-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="be81d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be81d-134">JSON representation</span></span>

<span data-ttu-id="be81d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be81d-135">Here is a JSON representation of the resource.</span></span>

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


