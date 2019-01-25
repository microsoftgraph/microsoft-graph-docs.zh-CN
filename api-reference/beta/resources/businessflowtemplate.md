---
title: businessFlowTemplate 资源类型
description: 在 Azure AD 中访问审阅功能，`businesFlowTemplate`代表 Azure AD 业务流程模板。 创建访问检查时，将呼叫者提供模板，如查看来宾组的成员的标识符。
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529577"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="f161c-104">businessFlowTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="f161c-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f161c-105">在 Azure AD[访问审阅](accessreviews-root.md)功能中，`businesFlowTemplate`代表 Azure AD 业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="f161c-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="f161c-106">创建访问检查时，将呼叫者提供模板，如查看来宾组的成员的标识符。</span><span class="sxs-lookup"><span data-stu-id="f161c-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="f161c-107">全局管理员 onboards 租户用于访问审阅功能时，将自动生成的业务流程模板对象。</span><span class="sxs-lookup"><span data-stu-id="f161c-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f161c-108">可以不创建任何其他业务流程模板。</span><span class="sxs-lookup"><span data-stu-id="f161c-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f161c-109">方法</span><span class="sxs-lookup"><span data-stu-id="f161c-109">Methods</span></span>

| <span data-ttu-id="f161c-110">方法</span><span class="sxs-lookup"><span data-stu-id="f161c-110">Method</span></span>           | <span data-ttu-id="f161c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f161c-111">Return Type</span></span>    |<span data-ttu-id="f161c-112">说明</span><span class="sxs-lookup"><span data-stu-id="f161c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f161c-113">列表 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="f161c-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="f161c-114">[businessFlowTemplate](businessflowtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="f161c-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="f161c-115">获取业务流程模板相应访问 reviews （英文）。</span><span class="sxs-lookup"><span data-stu-id="f161c-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="f161c-116">属性</span><span class="sxs-lookup"><span data-stu-id="f161c-116">Properties</span></span>
| <span data-ttu-id="f161c-117">属性</span><span class="sxs-lookup"><span data-stu-id="f161c-117">Property</span></span>     | <span data-ttu-id="f161c-118">类型</span><span class="sxs-lookup"><span data-stu-id="f161c-118">Type</span></span>   |<span data-ttu-id="f161c-119">说明</span><span class="sxs-lookup"><span data-stu-id="f161c-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f161c-120">业务流程模板的功能指派的标识符</span><span class="sxs-lookup"><span data-stu-id="f161c-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f161c-121">业务流程模板的名称</span><span class="sxs-lookup"><span data-stu-id="f161c-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f161c-122">关系</span><span class="sxs-lookup"><span data-stu-id="f161c-122">Relationships</span></span>

<span data-ttu-id="f161c-123">无。</span><span class="sxs-lookup"><span data-stu-id="f161c-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="f161c-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f161c-124">See also</span></span>

| <span data-ttu-id="f161c-125">方法</span><span class="sxs-lookup"><span data-stu-id="f161c-125">Method</span></span>           | <span data-ttu-id="f161c-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="f161c-126">Return Type</span></span>    |<span data-ttu-id="f161c-127">说明</span><span class="sxs-lookup"><span data-stu-id="f161c-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f161c-128">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="f161c-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="f161c-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="f161c-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="f161c-130">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="f161c-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f161c-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f161c-131">JSON representation</span></span>

<span data-ttu-id="f161c-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f161c-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
