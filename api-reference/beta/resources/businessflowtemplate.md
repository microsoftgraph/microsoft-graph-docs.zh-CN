---
title: businessFlowTemplate 资源类型
description: 在 Azure AD access 评论功能中， `businesFlowTemplate`表示 azure ad 业务流模板。 模板的标识符（如审阅组的来宾成员）是由呼叫者在创建访问评审时提供的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 461fe34e0d572f910f15df9521d54660f0568ad1
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703789"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="85120-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="85120-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85120-105">在 Azure AD [access 评论](accessreviews-root.md)功能中， `businesFlowTemplate`表示 azure ad 业务流模板。</span><span class="sxs-lookup"><span data-stu-id="85120-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="85120-106">模板的标识符（如审阅组的来宾成员）是由呼叫者在创建访问评审时提供的。</span><span class="sxs-lookup"><span data-stu-id="85120-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="85120-107">当全局管理员 onboards 租户使用访问评论功能时，将自动生成业务流模板对象。</span><span class="sxs-lookup"><span data-stu-id="85120-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="85120-108">业务流模板包括对应用程序的工作分配的访问审核、组成员身份、Azure AD 角色的成员、组的来宾用户成员资格和应用程序的来宾用户分配。</span><span class="sxs-lookup"><span data-stu-id="85120-108">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="85120-109">无法创建其他业务流模板。</span><span class="sxs-lookup"><span data-stu-id="85120-109">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="85120-110">方法</span><span class="sxs-lookup"><span data-stu-id="85120-110">Methods</span></span>

| <span data-ttu-id="85120-111">方法</span><span class="sxs-lookup"><span data-stu-id="85120-111">Method</span></span>           | <span data-ttu-id="85120-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="85120-112">Return Type</span></span>    |<span data-ttu-id="85120-113">说明</span><span class="sxs-lookup"><span data-stu-id="85120-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85120-114">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="85120-114">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="85120-115">[businessFlowTemplate](businessflowtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="85120-115">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="85120-116">获取适用于访问评审的业务流模板。</span><span class="sxs-lookup"><span data-stu-id="85120-116">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="85120-117">属性</span><span class="sxs-lookup"><span data-stu-id="85120-117">Properties</span></span>
| <span data-ttu-id="85120-118">属性</span><span class="sxs-lookup"><span data-stu-id="85120-118">Property</span></span>     | <span data-ttu-id="85120-119">类型</span><span class="sxs-lookup"><span data-stu-id="85120-119">Type</span></span>   |<span data-ttu-id="85120-120">说明</span><span class="sxs-lookup"><span data-stu-id="85120-120">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="85120-121">功能分配的业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="85120-121">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="85120-122">这些值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="85120-122">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="85120-123">业务流模板的名称</span><span class="sxs-lookup"><span data-stu-id="85120-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="85120-124">关系</span><span class="sxs-lookup"><span data-stu-id="85120-124">Relationships</span></span>

<span data-ttu-id="85120-125">无。</span><span class="sxs-lookup"><span data-stu-id="85120-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="85120-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="85120-126">See also</span></span>

| <span data-ttu-id="85120-127">方法</span><span class="sxs-lookup"><span data-stu-id="85120-127">Method</span></span>           | <span data-ttu-id="85120-128">返回类型</span><span class="sxs-lookup"><span data-stu-id="85120-128">Return Type</span></span>    |<span data-ttu-id="85120-129">说明</span><span class="sxs-lookup"><span data-stu-id="85120-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85120-130">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="85120-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="85120-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="85120-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="85120-132">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="85120-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="85120-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85120-133">JSON representation</span></span>

<span data-ttu-id="85120-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85120-134">Here is a JSON representation of the resource.</span></span>

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
