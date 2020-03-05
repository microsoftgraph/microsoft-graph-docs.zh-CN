---
title: businessFlowTemplate 资源类型
description: 在 Azure AD access 评论功能中， `businesFlowTemplate`表示 azure ad 业务流模板。 模板的标识符（如审阅组的来宾成员）是由呼叫者在创建访问评审时提供的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 00075813d011f6c6e66e0c853bfad6545bbc8c97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507857"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="246e8-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="246e8-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="246e8-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="246e8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="246e8-106">在 Azure AD [access 评论](accessreviews-root.md)功能中， `businesFlowTemplate`表示 azure ad 业务流模板。</span><span class="sxs-lookup"><span data-stu-id="246e8-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="246e8-107">模板的标识符（如审阅组的来宾成员）是由呼叫者在创建访问评审时提供的。</span><span class="sxs-lookup"><span data-stu-id="246e8-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="246e8-108">当全局管理员 onboards 租户使用访问评论功能时，将自动生成业务流模板对象。</span><span class="sxs-lookup"><span data-stu-id="246e8-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="246e8-109">业务流模板包括对应用程序的工作分配的访问审核、组成员身份、Azure AD 角色的成员、组的来宾用户成员资格和应用程序的来宾用户分配。</span><span class="sxs-lookup"><span data-stu-id="246e8-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="246e8-110">无法创建其他业务流模板。</span><span class="sxs-lookup"><span data-stu-id="246e8-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="246e8-111">方法</span><span class="sxs-lookup"><span data-stu-id="246e8-111">Methods</span></span>

| <span data-ttu-id="246e8-112">方法</span><span class="sxs-lookup"><span data-stu-id="246e8-112">Method</span></span>           | <span data-ttu-id="246e8-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="246e8-113">Return Type</span></span>    |<span data-ttu-id="246e8-114">说明</span><span class="sxs-lookup"><span data-stu-id="246e8-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="246e8-115">列出 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="246e8-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="246e8-116">[businessFlowTemplate](businessflowtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="246e8-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="246e8-117">获取适用于访问评审的业务流模板。</span><span class="sxs-lookup"><span data-stu-id="246e8-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="246e8-118">属性</span><span class="sxs-lookup"><span data-stu-id="246e8-118">Properties</span></span>
| <span data-ttu-id="246e8-119">属性</span><span class="sxs-lookup"><span data-stu-id="246e8-119">Property</span></span>     | <span data-ttu-id="246e8-120">类型</span><span class="sxs-lookup"><span data-stu-id="246e8-120">Type</span></span>   |<span data-ttu-id="246e8-121">说明</span><span class="sxs-lookup"><span data-stu-id="246e8-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="246e8-122">功能分配的业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="246e8-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="246e8-123">这些值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="246e8-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="246e8-124">业务流模板的名称</span><span class="sxs-lookup"><span data-stu-id="246e8-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="246e8-125">关系</span><span class="sxs-lookup"><span data-stu-id="246e8-125">Relationships</span></span>

<span data-ttu-id="246e8-126">无。</span><span class="sxs-lookup"><span data-stu-id="246e8-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="246e8-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="246e8-127">See also</span></span>

| <span data-ttu-id="246e8-128">方法</span><span class="sxs-lookup"><span data-stu-id="246e8-128">Method</span></span>           | <span data-ttu-id="246e8-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="246e8-129">Return Type</span></span>    |<span data-ttu-id="246e8-130">说明</span><span class="sxs-lookup"><span data-stu-id="246e8-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="246e8-131">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="246e8-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="246e8-132">accessReview</span><span class="sxs-lookup"><span data-stu-id="246e8-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="246e8-133">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="246e8-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="246e8-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="246e8-134">JSON representation</span></span>

<span data-ttu-id="246e8-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="246e8-135">Here is a JSON representation of the resource.</span></span>

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
