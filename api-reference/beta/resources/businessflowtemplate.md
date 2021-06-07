---
title: businessFlowTemplate 资源类型
description: 在 Azure AD 访问评审功能中，表示 `businesFlowTemplate` Azure AD 业务流程模板。 模板的标识符（如查看组的来宾成员）由调用方在创建访问评审时提供。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b1fce9de1c2f21d4a5c918985028acfee50dc390
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751242"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="1d861-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d861-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="1d861-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d861-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d861-106">在 Azure AD [访问评审](accessreviews-root.md) 功能中 **，businesFlowTemplate** 表示 Azure AD 业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="1d861-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the **businesFlowTemplate** represents an Azure AD business flow template.</span></span> <span data-ttu-id="1d861-107">模板的标识符（如查看组的来宾成员）由调用方在创建访问评审时提供。</span><span class="sxs-lookup"><span data-stu-id="1d861-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="1d861-108">当全局管理员载入租户以使用访问评审功能时，将自动生成业务流程模板对象。</span><span class="sxs-lookup"><span data-stu-id="1d861-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="1d861-109">业务流程模板包括对应用程序的分配的访问评审、组的成员身份、Azure AD 角色的成员身份、组的来宾用户成员身份以及到应用程序的来宾用户分配。</span><span class="sxs-lookup"><span data-stu-id="1d861-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="1d861-110">无法创建其他业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="1d861-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="1d861-111">Methods</span><span class="sxs-lookup"><span data-stu-id="1d861-111">Methods</span></span>

| <span data-ttu-id="1d861-112">方法</span><span class="sxs-lookup"><span data-stu-id="1d861-112">Method</span></span>           | <span data-ttu-id="1d861-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d861-113">Return Type</span></span>    |<span data-ttu-id="1d861-114">说明</span><span class="sxs-lookup"><span data-stu-id="1d861-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d861-115">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="1d861-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="1d861-116">[businessFlowTemplate](businessflowtemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d861-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="1d861-117">获取适用于访问评论的业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="1d861-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d861-118">属性</span><span class="sxs-lookup"><span data-stu-id="1d861-118">Properties</span></span>
| <span data-ttu-id="1d861-119">属性</span><span class="sxs-lookup"><span data-stu-id="1d861-119">Property</span></span>     | <span data-ttu-id="1d861-120">类型</span><span class="sxs-lookup"><span data-stu-id="1d861-120">Type</span></span>   |<span data-ttu-id="1d861-121">说明</span><span class="sxs-lookup"><span data-stu-id="1d861-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d861-122">id</span><span class="sxs-lookup"><span data-stu-id="1d861-122">id</span></span>                     |<span data-ttu-id="1d861-123">String</span><span class="sxs-lookup"><span data-stu-id="1d861-123">String</span></span>                | <span data-ttu-id="1d861-124">业务流程模板的功能分配标识符。</span><span class="sxs-lookup"><span data-stu-id="1d861-124">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="1d861-125">这些值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1d861-125">These values are case sensitive.</span></span>                                      |
| <span data-ttu-id="1d861-126">displayName</span><span class="sxs-lookup"><span data-stu-id="1d861-126">displayName</span></span>            |<span data-ttu-id="1d861-127">String</span><span class="sxs-lookup"><span data-stu-id="1d861-127">String</span></span>                | <span data-ttu-id="1d861-128">业务流程模板的名称</span><span class="sxs-lookup"><span data-stu-id="1d861-128">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="1d861-129">关系</span><span class="sxs-lookup"><span data-stu-id="1d861-129">Relationships</span></span>

<span data-ttu-id="1d861-130">无。</span><span class="sxs-lookup"><span data-stu-id="1d861-130">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="1d861-131">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1d861-131">See also</span></span>

| <span data-ttu-id="1d861-132">方法</span><span class="sxs-lookup"><span data-stu-id="1d861-132">Method</span></span>           | <span data-ttu-id="1d861-133">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d861-133">Return Type</span></span>    |<span data-ttu-id="1d861-134">说明</span><span class="sxs-lookup"><span data-stu-id="1d861-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d861-135">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="1d861-135">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="1d861-136">accessReview</span><span class="sxs-lookup"><span data-stu-id="1d861-136">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="1d861-137">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1d861-137">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1d861-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d861-138">JSON representation</span></span>

<span data-ttu-id="1d861-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d861-139">Here is a JSON representation of the resource.</span></span>

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


