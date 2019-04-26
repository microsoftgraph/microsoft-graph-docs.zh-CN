---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议, 它是使用 azure Active Directory (azure AD) 创建和管理的。 您可以根据您的方案使用以下方法来创建和管理 Azure Active Directory 使用条款功能。
localization_priority: Normal
ms.openlocfilehash: d91cc8f8180ffb706639fb42a8c68d711991602c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339172"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="77a16-104">协议资源类型</span><span class="sxs-lookup"><span data-stu-id="77a16-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77a16-105">表示租户的可自定义使用条款协议, 它是使用 azure Active Directory (azure AD) 创建和管理的。</span><span class="sxs-lookup"><span data-stu-id="77a16-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="77a16-106">您可以根据您的方案使用以下方法来创建和管理[Azure Active Directory 使用条款功能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)。</span><span class="sxs-lookup"><span data-stu-id="77a16-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="77a16-107">方法</span><span class="sxs-lookup"><span data-stu-id="77a16-107">Methods</span></span>

| <span data-ttu-id="77a16-108">方法</span><span class="sxs-lookup"><span data-stu-id="77a16-108">Method</span></span>       | <span data-ttu-id="77a16-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="77a16-109">Return Type</span></span> | <span data-ttu-id="77a16-110">说明</span><span class="sxs-lookup"><span data-stu-id="77a16-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="77a16-111">创建协议</span><span class="sxs-lookup"><span data-stu-id="77a16-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="77a16-112">本</span><span class="sxs-lookup"><span data-stu-id="77a16-112">agreement</span></span>](agreement.md) | <span data-ttu-id="77a16-113">通过发布到协议集合创建新协议。</span><span class="sxs-lookup"><span data-stu-id="77a16-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="77a16-114">列出协议</span><span class="sxs-lookup"><span data-stu-id="77a16-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="77a16-115">[协议](agreement.md)集合</span><span class="sxs-lookup"><span data-stu-id="77a16-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="77a16-116">获取一个协议对象集合。</span><span class="sxs-lookup"><span data-stu-id="77a16-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="77a16-117">获取协议</span><span class="sxs-lookup"><span data-stu-id="77a16-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="77a16-118">本</span><span class="sxs-lookup"><span data-stu-id="77a16-118">agreement</span></span>](agreement.md) | <span data-ttu-id="77a16-119">读取协议对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77a16-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="77a16-120">更新协议</span><span class="sxs-lookup"><span data-stu-id="77a16-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="77a16-121">本</span><span class="sxs-lookup"><span data-stu-id="77a16-121">agreement</span></span>](agreement.md) | <span data-ttu-id="77a16-122">更新协议对象。</span><span class="sxs-lookup"><span data-stu-id="77a16-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="77a16-123">删除协议</span><span class="sxs-lookup"><span data-stu-id="77a16-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="77a16-124">无</span><span class="sxs-lookup"><span data-stu-id="77a16-124">None</span></span> | <span data-ttu-id="77a16-125">删除协议对象。</span><span class="sxs-lookup"><span data-stu-id="77a16-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="77a16-126">属性</span><span class="sxs-lookup"><span data-stu-id="77a16-126">Properties</span></span>
| <span data-ttu-id="77a16-127">属性</span><span class="sxs-lookup"><span data-stu-id="77a16-127">Property</span></span>     | <span data-ttu-id="77a16-128">类型</span><span class="sxs-lookup"><span data-stu-id="77a16-128">Type</span></span>        | <span data-ttu-id="77a16-129">说明</span><span class="sxs-lookup"><span data-stu-id="77a16-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77a16-130">displayName</span><span class="sxs-lookup"><span data-stu-id="77a16-130">displayName</span></span>|<span data-ttu-id="77a16-131">String</span><span class="sxs-lookup"><span data-stu-id="77a16-131">String</span></span>|<span data-ttu-id="77a16-132">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="77a16-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="77a16-133">id</span><span class="sxs-lookup"><span data-stu-id="77a16-133">id</span></span>|<span data-ttu-id="77a16-134">String</span><span class="sxs-lookup"><span data-stu-id="77a16-134">String</span></span>| <span data-ttu-id="77a16-135">只读。</span><span class="sxs-lookup"><span data-stu-id="77a16-135">Read-only.</span></span>|
|<span data-ttu-id="77a16-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="77a16-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="77a16-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="77a16-137">Boolean</span></span>|<span data-ttu-id="77a16-138">指示用户是否必须在接受前展开并查看协议。</span><span class="sxs-lookup"><span data-stu-id="77a16-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77a16-139">关系</span><span class="sxs-lookup"><span data-stu-id="77a16-139">Relationships</span></span>
| <span data-ttu-id="77a16-140">关系</span><span class="sxs-lookup"><span data-stu-id="77a16-140">Relationship</span></span> | <span data-ttu-id="77a16-141">类型</span><span class="sxs-lookup"><span data-stu-id="77a16-141">Type</span></span>        | <span data-ttu-id="77a16-142">说明</span><span class="sxs-lookup"><span data-stu-id="77a16-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77a16-143">files</span><span class="sxs-lookup"><span data-stu-id="77a16-143">files</span></span>|<span data-ttu-id="77a16-144">[agreementFile](agreementfile.md)集合</span><span class="sxs-lookup"><span data-stu-id="77a16-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="77a16-145">只读。</span><span class="sxs-lookup"><span data-stu-id="77a16-145">Read-only.</span></span> <span data-ttu-id="77a16-146">链接到此协议的 pdf。</span><span class="sxs-lookup"><span data-stu-id="77a16-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77a16-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77a16-147">JSON representation</span></span>

<span data-ttu-id="77a16-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77a16-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->
