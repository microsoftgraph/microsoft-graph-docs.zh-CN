---
title: businessFlowTemplate 资源类型
description: 在 Azure AD 中访问审阅功能，`businesFlowTemplate`代表 Azure AD 业务流程模板。 创建访问检查时，将呼叫者提供模板，如查看来宾组的成员的标识符。
ms.openlocfilehash: 8faf1a1381f5cdcf4bfaab78adc7a6554479b427
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048210"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="da8f5-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="da8f5-104">businessFlowTemplate resource type</span></span>

> <span data-ttu-id="da8f5-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da8f5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da8f5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da8f5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da8f5-107">在 Azure AD[访问审阅](accessreviews-root.md)功能中，`businesFlowTemplate`代表 Azure AD 业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="da8f5-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="da8f5-108">创建访问检查时，将呼叫者提供模板，如查看来宾组的成员的标识符。</span><span class="sxs-lookup"><span data-stu-id="da8f5-108">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="da8f5-109">全局管理员 onboards 租户用于访问审阅功能时，将自动生成的业务流程模板对象。</span><span class="sxs-lookup"><span data-stu-id="da8f5-109">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="da8f5-110">可以不创建任何其他业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="da8f5-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="da8f5-111">方法</span><span class="sxs-lookup"><span data-stu-id="da8f5-111">Methods</span></span>

| <span data-ttu-id="da8f5-112">方法</span><span class="sxs-lookup"><span data-stu-id="da8f5-112">Method</span></span>           | <span data-ttu-id="da8f5-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="da8f5-113">Return Type</span></span>    |<span data-ttu-id="da8f5-114">说明</span><span class="sxs-lookup"><span data-stu-id="da8f5-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da8f5-115">列表 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="da8f5-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="da8f5-116">[businessFlowTemplate](businessflowtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="da8f5-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="da8f5-117">获取业务流程模板相应访问 reviews （英文）。</span><span class="sxs-lookup"><span data-stu-id="da8f5-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="da8f5-118">属性</span><span class="sxs-lookup"><span data-stu-id="da8f5-118">Properties</span></span>
| <span data-ttu-id="da8f5-119">属性</span><span class="sxs-lookup"><span data-stu-id="da8f5-119">Property</span></span>     | <span data-ttu-id="da8f5-120">类型</span><span class="sxs-lookup"><span data-stu-id="da8f5-120">Type</span></span>   |<span data-ttu-id="da8f5-121">说明</span><span class="sxs-lookup"><span data-stu-id="da8f5-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="da8f5-122">业务流程模板的功能指派的标识符</span><span class="sxs-lookup"><span data-stu-id="da8f5-122">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="da8f5-123">业务流程模板的名称</span><span class="sxs-lookup"><span data-stu-id="da8f5-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="da8f5-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="da8f5-124">Relationships</span></span>

<span data-ttu-id="da8f5-125">无。</span><span class="sxs-lookup"><span data-stu-id="da8f5-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="da8f5-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="da8f5-126">See also</span></span>

| <span data-ttu-id="da8f5-127">方法</span><span class="sxs-lookup"><span data-stu-id="da8f5-127">Method</span></span>           | <span data-ttu-id="da8f5-128">返回类型</span><span class="sxs-lookup"><span data-stu-id="da8f5-128">Return Type</span></span>    |<span data-ttu-id="da8f5-129">说明</span><span class="sxs-lookup"><span data-stu-id="da8f5-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da8f5-130">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="da8f5-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="da8f5-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="da8f5-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="da8f5-132">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="da8f5-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="da8f5-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da8f5-133">JSON representation</span></span>

<span data-ttu-id="da8f5-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da8f5-134">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
