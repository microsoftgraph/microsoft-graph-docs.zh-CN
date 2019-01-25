---
title: 协议资源类型
description: 表示一个租户的可自定义的创建和管理与 Azure Active Directory (Azure AD) 使用协议条款。 可以使用以下方法来创建和管理 Azure Active Directory 使用条款的功能，根据您的方案。
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513849"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="0b721-104">协议资源类型</span><span class="sxs-lookup"><span data-stu-id="0b721-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b721-105">表示一个租户的可自定义的创建和管理与 Azure Active Directory (Azure AD) 使用协议条款。</span><span class="sxs-lookup"><span data-stu-id="0b721-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="0b721-106">可以使用以下方法来创建和管理[Azure Active Directory 使用条款的功能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)，根据您的方案。</span><span class="sxs-lookup"><span data-stu-id="0b721-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="0b721-107">方法</span><span class="sxs-lookup"><span data-stu-id="0b721-107">Methods</span></span>

| <span data-ttu-id="0b721-108">方法</span><span class="sxs-lookup"><span data-stu-id="0b721-108">Method</span></span>       | <span data-ttu-id="0b721-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b721-109">Return Type</span></span> | <span data-ttu-id="0b721-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b721-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0b721-111">创建协议</span><span class="sxs-lookup"><span data-stu-id="0b721-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="0b721-112">协议</span><span class="sxs-lookup"><span data-stu-id="0b721-112">agreement</span></span>](agreement.md) | <span data-ttu-id="0b721-113">通过发布到协议集合中创建新的协议。</span><span class="sxs-lookup"><span data-stu-id="0b721-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="0b721-114">列表协议</span><span class="sxs-lookup"><span data-stu-id="0b721-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="0b721-115">[协议](agreement.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b721-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="0b721-116">获取协议对象集合。</span><span class="sxs-lookup"><span data-stu-id="0b721-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="0b721-117">获取协议</span><span class="sxs-lookup"><span data-stu-id="0b721-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="0b721-118">协议</span><span class="sxs-lookup"><span data-stu-id="0b721-118">agreement</span></span>](agreement.md) | <span data-ttu-id="0b721-119">读取属性和协议对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0b721-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="0b721-120">更新协议</span><span class="sxs-lookup"><span data-stu-id="0b721-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="0b721-121">协议</span><span class="sxs-lookup"><span data-stu-id="0b721-121">agreement</span></span>](agreement.md) | <span data-ttu-id="0b721-122">更新协议对象。</span><span class="sxs-lookup"><span data-stu-id="0b721-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="0b721-123">删除协议</span><span class="sxs-lookup"><span data-stu-id="0b721-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="0b721-124">无</span><span class="sxs-lookup"><span data-stu-id="0b721-124">None</span></span> | <span data-ttu-id="0b721-125">删除协议对象。</span><span class="sxs-lookup"><span data-stu-id="0b721-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="0b721-126">属性</span><span class="sxs-lookup"><span data-stu-id="0b721-126">Properties</span></span>
| <span data-ttu-id="0b721-127">属性</span><span class="sxs-lookup"><span data-stu-id="0b721-127">Property</span></span>     | <span data-ttu-id="0b721-128">类型</span><span class="sxs-lookup"><span data-stu-id="0b721-128">Type</span></span>        | <span data-ttu-id="0b721-129">说明</span><span class="sxs-lookup"><span data-stu-id="0b721-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b721-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0b721-130">displayName</span></span>|<span data-ttu-id="0b721-131">String</span><span class="sxs-lookup"><span data-stu-id="0b721-131">String</span></span>|<span data-ttu-id="0b721-132">协议中的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0b721-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="0b721-133">id</span><span class="sxs-lookup"><span data-stu-id="0b721-133">id</span></span>|<span data-ttu-id="0b721-134">String</span><span class="sxs-lookup"><span data-stu-id="0b721-134">String</span></span>| <span data-ttu-id="0b721-135">只读。</span><span class="sxs-lookup"><span data-stu-id="0b721-135">Read-only.</span></span>|
|<span data-ttu-id="0b721-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="0b721-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="0b721-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b721-137">Boolean</span></span>|<span data-ttu-id="0b721-138">指示用户是否能够展开和查看接受之前协议。</span><span class="sxs-lookup"><span data-stu-id="0b721-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b721-139">关系</span><span class="sxs-lookup"><span data-stu-id="0b721-139">Relationships</span></span>
| <span data-ttu-id="0b721-140">关系</span><span class="sxs-lookup"><span data-stu-id="0b721-140">Relationship</span></span> | <span data-ttu-id="0b721-141">类型</span><span class="sxs-lookup"><span data-stu-id="0b721-141">Type</span></span>        | <span data-ttu-id="0b721-142">说明</span><span class="sxs-lookup"><span data-stu-id="0b721-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b721-143">files</span><span class="sxs-lookup"><span data-stu-id="0b721-143">files</span></span>|<span data-ttu-id="0b721-144">[agreementFile](agreementfile.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b721-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="0b721-145">只读。</span><span class="sxs-lookup"><span data-stu-id="0b721-145">Read-only.</span></span> <span data-ttu-id="0b721-146">Pdf 链接到此协议。</span><span class="sxs-lookup"><span data-stu-id="0b721-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b721-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b721-147">JSON representation</span></span>

<span data-ttu-id="0b721-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b721-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
